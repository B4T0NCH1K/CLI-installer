@echo off
echo %LG_WEBOS_TV_SDK_HOME%
echo 0
echo if it says "DiskLetter:\PATH\webOS_TV_SDK" CLI is already installed.
echo 0
echo if you want to reinstall it delete CLI from PATH that just said.
echo 0
echo delete CLI and restart this .bat file.
echo 0
pause
echo %LG_WEBOS_TV_SDK_HOME%
echo 0
echo if it says "LG_WEBOS_TV_SDK_HOME" you successfully deleted CLI.
echo 0
pause
echo Installing...
setx /m LG_WEBOS_TV_SDK_HOME "C:\webOS_TV_SDK"
setx /m WEBOS_CLI_TV "%LG_WEBOS_TV_SDK_HOME%\CLI\bin"
setx /m PATH "%PATH%;%WEBOS_CLI_TV%"
echo 0
pause
exit
