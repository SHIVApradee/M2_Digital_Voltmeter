# ABSTRACT
* In this project we are going to design a 25V range digital voltmeter by using ATMEGA32A microcontroller. 
* In ATMEGA, we are going to use 10bit ADC (Analog to Digital Converter) to build a digital voltmeter.
* Now the ADC in ATMEGA can not take a input more than +5V, so for getting a higher range we are going to use a voltage divider circuit.
* This loading effect of resistance based voltage divider is important as the current drawn from Vout of voltage divider increases the error percentage, for now we         need not worry about loading effect.
* We are going to take two resistors and form a divider circuit so that for a 25Volts Vin, we get a 5Volt Vout. So all we have to do is multiply the Vout value with “5”     in the program in order to get the real input voltage.
