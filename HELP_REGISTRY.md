### return main page

### Работа с реестром в PowerShell 
**get-help Registry** (cmdlets) Для работы с реестром Windows не обязательно использовать графический редактор **regedit.exe**  или утилиту командной строки **reg.exe**.
* Get-Location
* Set-Location
* Get-Item
* Get-ChildItem
* Invoke-Item
* Move-Item
* New-Item
* Remove-Item
* Get-ItemProperty
* Set-ItemProperty
* Remove-ItemProperty
* Clear-ItemProperty
* Get-Acl
* Set-Acl

### Конвейер
Когда вы запускаете какой-либо командлет, то возвращаемые им значения преобразуются в текст и выводятся на экран. Write in powershell : `ls -filter "*.bat" | Get-Content` А вто тут мы  создали файл txt и скропировали вест текст : `Get-Help Registry | Set-Content reg.txt`

### links :
* [Работа с файлами, папками и разделами реестра](https://learn.microsoft.com/ru-ru/powershell/scripting/samples/working-with-files-folders-and-registry-keys?view=powershell-7.2)
* [Работа с ключами и записями реестра](https://winitpro.ru/index.php/2017/02/07/rabotaem-s-reestrom-windows-cherez-powershell/)