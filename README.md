
# Install Scoop in PowerShell Windows 10
![Scoop-PowerShell](img/scoop.png)

1. Open the command line administrator (x32)
2. write in cmd `powershell`

# Copy and write commands in cmd
* Set-ExecutionPolicy RemoteSigned -scope CurrentUser
* iex (new-object net.webclient).downloadstring('https://get.scoop.sh')
* set-executionpolicy -s cu Unrestricted
* scoop help
* scoop install curl
* scoop bucket add extras
* scoop install grep
* scoop install concfg
* concfg import solarized-dark
* scoop install pshazz
* scoop install touch
* scoop install sudo
* scoop search

## Basic command PowerShell
* `Get-Childitem` - similar commands `ls` or `dir`
* `Get-Command -Name *dns*` - see list where is all commands with this word. Change word `*dns*` with word which you need.
* `Get-Process` - watch all processes in terminal
* `Get-Command ` - list commands PowerShell
* `Get-Command -verb Get` - commands which begin with get
* `?` - soon wil be more commands ...

## Questions
* How to chnage title PowerShell ? seem lik cmd `title` 
*