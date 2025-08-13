### Set Execution Policy :

```error
Ошибки с командой Set-ExecutionPolicy и их исправление
=====================================================
```

1. Ошибка: "Set-ExecutionPolicy не является внутренней или внешней командой"
   - Причина: команда введена в cmd.exe вместо PowerShell.
   - Решение:
     а) Открой PowerShell, а не cmd:
        - Нажми Win + S, введи "PowerShell", нажми Enter.
     б) В PowerShell введи команду:
        Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

2. Ошибка: "Сбой выполнения программы Set-ExecutionPolicy: Указанному файлу не сопоставлено ни одно приложение..."
   - Причина: PowerShell пытается запустить внешний файл вместо встроенного cmdlet.
   - Решение:
     а) Проверить, что именно запускается:
        Get-Command Set-ExecutionPolicy
        - Если CommandType = Application, значит есть файл, мешающий команде.
     б) Найти мешающий файл:
        Get-Item C:\Windows\system32\Set-ExecutionPolicy*
     в) Переименовать файл (от имени администратора):
        Rename-Item -Path C:\Windows\system32\Set-ExecutionPolicy -NewName Set-ExecutionPolicy.bak -Force
     г) Закрыть и заново открыть PowerShell.
     д) Проверить команду:
        Get-Command Set-ExecutionPolicy
        - Должен быть Cmdlet.
     е) Выполнить:
        Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

3. Ошибка: "Set-ExecutionPolicy распознаётся как Application вместо Cmdlet"
   - См. пункт 2 выше: переименование мешающего файла.

---

Дополнительно:

Если установка политики всё равно проблематична, можно обойти политику временно при установке scoop:

powershell -ExecutionPolicy Bypass -NoProfile -Command "iwr -useb get.scoop.sh | iex"

---

Автор: NicolaiCushnir
Дата: 2025-08-13
