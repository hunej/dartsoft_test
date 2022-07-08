# Milsig Dartsoft Arduino Toolkit

## Summary
This repository contains the Arduino code which can can be built as a dartsoft or airsoft task props box. Two Arduino Uno Board are used as master board and slave board,  which are communicated via I2C. 

The master board needs some peripherals such as LED Display(TM1637), Internal Timer(Firmware Interrupt), RFID Sensor(RC522), Buzzer with Internal Oscillator, Photoresistor, IR Remote Control, Potentiometer(B10k).

The audio playback event is sent via I2C to trigger slave board's MP3 audio decoder(VS1053B). An AUX line and external speaker is needed. 

User can use master board alone without slave board if MP3 playback function is not required.


## Updates 

### 2022/07/08
* First Commit
* Add a Potentiometer for Photoresistor threshold controlling
* Add mounting stage timer compensation
* File path correction
* Timer input refinement

## TODO : 
* mp3 audio content rework, add coffin dance music
* external reset button
* add pin info documents
* code optimization, add comment, indent correction
* add rgb led light module
* change Photoresistor to PING Sensor
* add ENABLE_SLAVE_BOARD mode flag for master board used alone
* magic number elimination
* demo box installation tutorial
* 11.1v lipo for two Arduino Uno board powerining issue
* single Arduino Mega + DFPlayer w/ internal speaker demobox implementation
