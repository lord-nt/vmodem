# vmodem
The Virtual Modem script for Raspberry Pi and Linux based systems

 --------------------------------
 VMODEM - Virtual Modem bootstrap
 --------------------------------
 Oliver Molini 2020 Billy Stoughton II/Lord_NT 2020

 Licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
 https://creativecommons.org/licenses/by-nc-sa/4.0/

 Tested working out of box with the following host configurations:

 o Most Standard VT100 terminals and terminal emulations

 o HyperTerminal

 o PuTTY

 PPP connectivity will initialize correctly under the following configurations:

 o Microsoft Windows 3.1
 - Generic
     - Standard 14400 or 28800 bps Modem
     - Trumpet Winsock (Dial ATDT1)

 o Microsoft Windows 95,98?
 - Generic
     - Standard 28800 bps Modem
     - Trumpet Winsock (Dial ATDT1)

 o Microsoft Windows 9x.ME - Windows 10
   - Generic
     - Standard 28800 bps Modem
     - Standard 33600 bps Modem <-- Win2k and UP use this modem
     (::NOTE:: dial ATDT2 to disable fake login if needed WinNT 3.51 - 10)

 o Serial Line Setup
   - Baud 57600 8,N,1 'No Flow Control'

 o Lynx
   - Type lynx to start a Lynx Web Browser session from your terminal. (!!if lynx is installed on your pi!!)

 o Local Login
   - Type login to get a Linux Login Shell session from your terminal.

 o Telnet Session
   - Type telnet to get a telnet session (!!if telnet is installed on your pi!!)

 ::NOTE:: !!if you have a 8250 UART you must use speeds of 19200 baud or lower!!

Tested on Ubuntu and Debian based Linux but should work with some mods on other Unix/Linux based O/S

There is also a serial to telnet server that is in testing if you wish to try, please click on the experimental branch
and read the instructions in the file ser2telsvr.sh for more details.

[General Usage]
sudo ./vmodem
