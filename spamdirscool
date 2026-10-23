
@echo off
setlocal
title MultiDir Launcher

set "DIR=%TEMP%\MultiDir_%RANDOM%"
mkdir "%DIR%" 2>nul

(
echo @echo off
echo color 2
echo title GREEN DIR
echo :loop
echo dir /s
echo goto loop
) > "%DIR%\green.bat"

(
echo @echo off
echo color 4
echo title RED DIR
echo :loop
echo dir /s
echo goto loop
) > "%DIR%\red.bat"

(
echo @echo off
echo color 3
echo title AQUA DIR
echo :loop
echo dir /s
echo goto loop
) > "%DIR%\aqua.bat"

start "GREEN DIR" cmd /k ""%DIR%\green.bat""
start "RED DIR" cmd /k ""%DIR%\red.bat""
start "AQUA DIR" cmd /k ""%DIR%\aqua.bat""

endlocal
exit /b
