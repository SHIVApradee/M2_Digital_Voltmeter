# DIGITAL VOLTMETER
## ABSTRACT
This project "DIGITAL VOLTMETER" is to design a 25V range digital voltmeter by using ATMEGA32A microcontroller. In ATMEGA, we are going to use 10bit ADC (Analog to Digital Converter) to build a digital voltmeter. Now the ADC in ATMEGA can not take a input more than +5V, so for getting a higher range we are going to use a voltage divider circuit.Now important thing to note here is, the input taken by the controller for ADC conversion is as low as 50µAmp. This loading effect of resistance based voltage divider is important as the current drawn from Vout of voltage divider increases the error percentage, for now we need not worry about loading effect.
## INTRODUCTION
* Digital Voltmeter abbreviated as DVM is an instrument used to measure the electrical potential difference between two points in a circuit.
* The voltage could be an alternating current (AC) or direct current (DC).
* It measures the input voltage after converting the analog voltage to digital voltage and displays it in number format using a convertor.
* The usage of digital voltmeter has increased the speed and accuracy with which the readings are noted.
## COMPONENTS USED
1. ATMEGA32
2. Potentiometer
3. Power supply (5v)
4. AVR-ISP PROGRAMMER
5. JHD_162ALCD (16*2LCD)
6. 100uF capacitor, 100nF capacitor (5 pieces)
7. 10KΩ resistor, 2KΩresistor
## COMPONENTS DESCRIPTION
* ATmega328 is an Advanced Virtual RISC (AVR) microcontroller. It supports 8-bit data processing. ATmega-328 has 32KB internal flash memory. ATmega328 has 1KB Electrically Erasable Programmable Read-Only Memory (EEPROM).
* Potentiometers work by varying the position of a sliding contact across a uniform resistance. In a potentiometer, the entire input voltage is applied across the whole length of the resistor, and the output voltage is the voltage drop between the fixed and sliding contact as shown below.
* LCD (Liquid Crystal Display) is a type of flat panel display which uses liquid crystals in its primary form of operation. LEDs have a large and varying set of use cases for consumers and businesses, as they can be commonly found in smartphones, televisions, computer monitors and instrument panels.
## WORKING 
* Here PORTB of ATMEGA32 is connected to data port of LCD. One should remember to disable the JTAG communication in PORTC ot ATMEGA by changing the fuse bytes, if one wants to use the PORTC as a normal communication port. 
* In 16x2 LCD there are 16 pins total if there is a black light, if there is no back light there will be 14 pins. One can power or leave the back light pins. 
* Now in the 14 pins there are 8 data pins (7-14 or D0-D7), 2 power supply pins, 3rd pin for contrast control, and 3 control pins.
* In the circuit, you can observe that I have only took two control pins , this gives the flexibility of better understanding, the contrast bit and READ/WRITE are not often used so they can be shorted to ground. 
* This puts LCD in highest contrast and read mode. We just need to control ENABLE and RS pins to send characters and data accordingly.
* The complete digital voltmeter circuit diagram is shown in the above figure.
## CIRCUIT DIAGRAM
![circuitdiagram](https://user-images.githubusercontent.com/93831316/164976445-dcc07936-4e17-443f-9c5f-eee9007fd580.png)
## CONCLUSION
The digital multimeter is a reliable measurement tool which allows us to verify calculated values almost accurately and flawlessly.


 
