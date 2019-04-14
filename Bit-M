@echo off
title SMARTkom
color 

:meni
@echo off
cls
echo.
echo Witaj!
echo Jest godzina %time%
echo A, dzisiaj jest %date%
echo.
echo !!UWAGA!!
echo.
echo Aby uruchomic ktores z podanych dzialan nalezy uzywac DUZYCH liter.
echo.
echo Wybierz dzialanie:
echo A) Kalkulator
echo B) Przegladarka internetowa
echo D) GaduNET (Czat) //NIESTABILNA\\
echo G) Wyjscie
echo.
set /p opcja=Przejdz do:
if %opcja%==A goto kalkulator
if %opcja%==B goto przegladarka
if %opcja%==C goto ciekawe
if %opcja%==D goto menu
if %opcja%==F goto autorzy
if %opcja%==E goto ustawienia
if %opcja%==G exit
goto zly
:kalkulator
pause
goto poczatek
:poczatek
@echo off
cls
echo.
echo  Kalkulator  
echo.
echo  Wybierz porzadane dzialanie: 
echo .
echo  1) Dodawanie 
echo  2) Odejmowanie 
echo  3) Mnozenie 
echo  4) Dzielenie 
echo  5) Autor 
echo  6) Wroc
echo.
echo.
echo.
set /p opcja=Przejdz do:
if %opcja%==1 goto opcja1
if %opcja%==2 goto opcja2
if %opcja%==3 goto opcja3
if %opcja%==4 goto opcja4
if %opcja%==5 goto opcja5
if %opcja%==6 goto opcja6
goto zly_wybor
:zly_wybor
echo Error
pause
goto poczatek
:opcja1
cls
echo Wybrano Dodawanie!
echo.
echo.
echo.
set /p zmienna1="Prosze podac pierwsza liczbe:"
echo.
set /p zmienna2="Prosze podac druga liczbe:"
set /a wynik=%zmienna1% + %zmienna2%
echo.
echo %zmienna1% + %zmienna2% = %wynik%
echo.
echo Wynik: %wynik%
pause
goto poczatek
:opcja2
cls
echo Wybrano Odejmowanie!
echo.
echo.
echo.
set /p zmienna1="Prosze podac pierwsza liczbe:"
echo.
set /p zmienna2="Prosze podac druga liczbe:"
set /a wynik=%zmienna1% - %zmienna2%
echo.
echo %zmienna1% - %zmienna2% = %wynik%
echo.
echo Wynik: %wynik%
pause
goto poczatek
:opcja3
cls
echo Wybrano Mnozenie!
echo.
echo.
echo.
set /p zmienna1="Prosze podac pierwsza liczbe:"
echo.
set /p zmienna2="Prosze podac druga liczbe:"
set /a wynik=%zmienna1% * %zmienna2%
echo.
echo %zmienna1% x %zmienna2% = %wynik%
echo.
echo Wynik: %wynik%
pause
goto poczatek
:opcja4
cls
echo Wybrano Dzielenie!
echo.
echo.
echo.
set /p zmienna1="Prosze podac pierwsza liczbe:"
echo.
set /p zmienna2="Prosze podac druga liczbe:"
set /a wynik=%zmienna1% / %zmienna2%
echo.
echo %zmienna1% : %zmienna2% = %wynik%
echo.
echo Wynik: %wynik%
pause
goto poczatek
:opcja5
cls
echo By XvbStudios
pause
goto poczatek
:opcja6
goto meni
:przegladarka
start chrome.exe
exit
:ciekawe
cls
echo.
pause
goto meni
:zly
pause
goto meni
:menu
@echo off
md C:\GaduNET
cd C:\GaduNET
title GaduNET
cls
echo 2) Rejestracja
set/p "w=wybierz:"
if %w%== 2 goto rejestracja
if not %w%== w8dy7g goto menu
:rejestracja
cls
echo ###############
echo # REJESTRACJA #
echo ###############
echo.
set/p user=Nazwa Uzytkownika:
echo.
set/p Haslo=Haslo:
cd C:\Documents and Settings\Administrator\Pulpit\Login
md %Login%
cd C:\Documents and Settings\Administrator\Pulpit\Login\%Login%
md %Haslo%
echo Konto %Login% zostalo poprawnie utworzone
pause >nul
goto :login
:logowanie
cls
echo #############
echo # LOGOWANIE #
echo #############
echo.
set/p login1=Login:
echo.
set/p haslo1=Haslo:
cd C:\Documents and Settings\Administrator\Pulpit\Login
if exist %login1% goto XX
if not exist %login1% goto fail
:XX
cd C:\Documents and Settings\Administrator\Pulpit\Login\%login1%
if exist %haslo1% goto ok
if not exist %haslo1% goto fail
:fail
echo Nie udalo sie zalogowac. Haslo lub login sa nie prawidlowe.
pause >nul
goto menu
:ok
echo Udalo sie . Witamy!
goto :login
title GaduNET
:login
cls
set/p "user=Podaj nick: "
goto serwer
:serwer
cls
echo Podaj serwer. 
set/p "serwer=Podaj server: "
echo %user% dolaczyl do pokoju >> %serwer%.log
goto chat
:chat
cls
type %serwer%.log
echo.
echo Przyciski: Q wyjscie, T pisanie wiadomosci, C czyszczenie pokoju, W powrot do logowania
choice /c QTCW9 /D 9 /T 1 >nul
if %errorlevel% == 1 goto exit
if %errorlevel% == 2 goto msg
if %errorlevel% == 3 goto clear
if %errorlevel% == 4 goto login
if %errorlevel% == 9 goto chat
goto chat
:exit
cls
echo %user% wyszedl z pokoju >> %serwer%.log
exit
:msg
set/p "msg=>"
echo %user% napisal: %msg% >> %serwer%.log
goto chat
:clear
cls
color 9a
echo %user% wyczyscil pokoj > %serwer%.log
goto chat﻿
:autorzy
cls
echo.
echo Autorem tego programu jest:
echo XvbStudios
pause
goto meni
:ustawienia
cls
echo. 
pause
goto meni
