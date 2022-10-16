### [return main page](../README.md)

### Batch files :
**Batch** является языком программирования, используется для создания файлов сценарий(scripts files) которые можно выполнять на операционной системе Windows, обычно эти файлы имеют окончание **.bat** или **.cmd.** При выполнении они открывают окно "Command Prompt"

**Notes** Заметьте еще один язык похожий на batch, но использующийся для операционной системы Linux это Shell, с файлами сценарий с окончанием **.sh.**

**Notes** Там есть 2 вида открытие файлов bat. Через теримнл `cd documents/path` или нажатие мыши 2 раза.

### Syntax batch
* **@rem** or **::** Использует чтобы начать строку комментария.
* **@echo off** Sa nu vezi tot gunoiu ce nu itsi trebuie ... In plus trebuie sa steoe 1 linie din script.
* **echo** Вывод в консоли или распечатать строку на экране
* **pause** Делается для того чтобы не закрывалось автоматический окно консоли, терминал.

```bat
@echo off
set name="Nicolai"
echo My name is : %name%
```

### Links:
* [FAQ SHELL](http://www.classicshell.net/faq/#general_what)
