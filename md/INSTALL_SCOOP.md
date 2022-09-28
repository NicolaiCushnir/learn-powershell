# Install Scoop in PowerShell Windows 10
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
