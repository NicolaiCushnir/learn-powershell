# Install Scoop in PowerShell Windows 10
1. Open the command line administrator (x32)

### Copy and write commands in cmd
* Set-ExecutionPolicy RemoteSigned -scope CurrentUser
* iex (new-object net.webclient).downloadstring('https://get.scoop.sh')
* iex "& {$(irm get.scoop.sh)} -RunAsAdmin" **дополнительно ! Если команда сверху не работает**
* set-executionpolicy -s cu Unrestricted
* scoop --help
* scoop --version
* scoop install curl
* scoop bucket add extras
* scoop install grep
* scoop install concfg
* concfg import solarized-dark
* scoop install pshazz
* scoop install touch
* scoop install sudo
* scoop search

### Errors which can appear :
* If you have errorat command : "Set-ExecutionPolicy RemoteSigned -scoop CurrentUser: `Set-ExecutionPolicy RemoteSigned -scope CurrentUser "Set-ExecutionPolicy" не является внутренней или внешней
командой, исполняемой программой или пакетным файлом.` Тогда напиши в cmd `powershell`.
* If you have so error: **Running the installer as administrator is disabled by default, see https://github.com/ScoopInstaller/Install#for-admin for details.** Than try: **iex "& {$(irm get.scoop.sh)} -RunAsAdmin"**
* ???

### Extern links :
* [Stack Overflow - Installing scoop fails: "Running the installer as administrator is disabled by default](https://stackoverflow.com/questions/74763204/installing-scoop-fails-running-the-installer-as-administrator-is-disabled-by-d)
