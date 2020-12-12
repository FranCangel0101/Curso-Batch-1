# Curso-Batch-1
rem // Aqui les dejo el codigo del curso 
rem // batch utilizado en el capitulo 1, 
rem // no se olviden de suscribir a mi 
rem // canal de YouTube: FranCangel 

@echo off
title Tutorial
:Main
mode 43,20
echo.
echo.
echo           --------------------
echo           ^|      Prueba      ^|
echo           --------------------
echo           ^| [1] Ir a SubMenu ^|
echo           ^| [2] Ver Mi Ip    ^|
echo           -------------------- 
echo.
set /p inicio= Comando: 

if "%inicio%"=="1" goto SubMenu
if "%inicio%"=="2" goto VerIp
goto Main


:SubMenu
mode 43,20
echo.
echo       hola
echo.
pause>nul
goto Main

:VerIp
mode 70,35
echo.
ipconfig
echo.
pause>nul
goto Main
