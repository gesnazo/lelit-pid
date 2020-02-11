# lelitpid

Lelit PL041EM PID using NODEMCU ESP8266

Based on:

Rancilio-Silvia PID für Arduino http://rancilio-pid.de

MASTER VERSION

Version 1.9.7

Using PlatformIO over Visual Studio Code

Changes:

* Using K-thermocouple and MAX6675, TEMPSENSOR = 3 in userConfig.h
* Using PCF8574 GPIO expansor (I2C), so MAX6675 uses SPI interface, it needs more GPIOS, and pump and valve are connected to this expansor
* Using an average from 3 readings to get temp, so it smooths values (RunningAverage.h)
* New smoking coffee icon