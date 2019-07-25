# Homebrew Automation Board Rev A Reworks

* U1 silk is hard to understand. Doesn't _clearly_ indicate pin 1 / orientation.
* U1 address pins should probably get some thermal relief to make soldering easier
* I don't like the copper neck under F1. Looks like it could cause a short.
* While pin 1 is defined on board silk for A1, the A1 module doesn't indicate pin 1 very obviously or at all.
* I don't like the closeness of the pads for A1. Makes soldering pretty tricky when trying to avoid shorts.
* Silk on 3.3V power select is switched.
* Transistor pitch is very difficult to solder. To be honest, SOT23 would probably be easier
* Pull-downs on PWM signals are missing
* TX and RX is switched
* The male 1x14 pins I bought are too long and needed to be trimmed.
* ~Pull-down needed on romi shutdown pin~ Cut trace on shutdown pin to disable feature
* Real-time clock for Raspberry Pi
* EEPROM should always be powered from Raspberry Pi 3.3V
* In order to prevent undervolting the Pi, consider changing the 5V regulator's TRIM resistor to 255 ohm (1%)
* Add more bulk capacitance to prevent high internal resistance of Alkaline batteries from allowing VBAT 
* Button (force AP mode), shutdown button for pi, and LEDs (know if connected to wifi) specifically for PiFi
