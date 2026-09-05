@echo off
title Crusade Installer
cls

echo ========================================
echo          Crusade Installer
echo ========================================
echo.

:: Create folder (ignore errors)
mkdir "%USERPROFILE%\Downloads\Crusade" 2>nul

echo Downloading Crusade...
curl -L -o "%USERPROFILE%\Downloads\Crusade\Crusade.exe" ^
"https://github.com/ambrionsaves/Crusade/releases/download/External/Crusade.exe"

echo.
echo ========================================
echo          Crusade Downloaded!
echo ========================================
echo.
echo Location:
echo %USERPROFILE%\Downloads\Crusade\Crusade.exe
echo.

pause
