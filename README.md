AlvDuino
========	
After breaking an Arduino Uno I decided to build one instead of buying one. Using CadSoft EAGLE I designed a PCB layout for a custom Arduino Uno R3 board which I named the AlvDuino. I read through the Uno schematic to understand the basic hardware and overall design. I removed USB functionality and used a simpler design that can be programmed through an external programmer (USBTinyISP).  

Arduino Uno design and information can be found here: http://arduino.cc/en/Main/ArduinoBoardUno   

Here is an image of the AlvDuino:  
<img src="https://raw.githubusercontent.com/a3alamgi/AlvDuino/master/images/AlvDuino.jpg"/>

Click here to see AlvDuino in use:  
<a href="https://youtu.be/0XYK6YoSBJY">https://youtu.be/0XYK6YoSBJY</a>


Materials:
---------
Researched into use of components in the schematic and selected appropriate packages for soldering and minimizing board space
-	x3, 0.1uF ceramic capacitor, package 1206
-	x2, 47uF aluminum capacitor, SMD
-	x1, 10kΩ resistor, package 1206
-	x2, 1kΩ resistor, package 1206
-	x1, 1MΩ resistor, package 1206
-	x1, green LED, SMD
-	x2, diode, package DO214AA 
-	x1, tactile switch
-	x1, 2x3 vertical pin header 
-	x1, 1x6 female connector header
-	x2, 1x8 female connector header
-	x1, 1x10 female connector header
-	x1, 2.1mm power connector jack
-	x1, 28 position IC socket 
-	x1, 5V regulator, package SOT223, [NCP1117ST50T3G](http://www.onsemi.com/pub_link/Collateral/NCP1117-D.PDF)
-	x1, ceramic 16MHz resonator, radial-3 lead, [CSTL16M0X53-A0](http://search.murata.co.jp/Ceramy/image/img/w_hinm/L0430E.pdf)
-	x1, ATMEGA328-P DIP chip, [ATMEGA328P-PU](http://www.atmel.com/Images/doc8161.pdf)
-	Soldering assembly (solder, iron, braid, etc.)  

Design & Assembly:
-----------------
-	Designed a PCB layout for an Arduino Uno board with Atmega328P to minimize size while retaining functionality (see Figure 1)
-	Rearranged output pin positions for easier board routing
-	Positioned all pins with 0.1” pitch (or a multiple of) so that any prototype board can be used as a custom shield
-	Ordered components from DigiKey/Newark and PCB from OSHPark
-	Soldered and assembled all the components to the board
-	Used ICSP headers used to upload program through an external programmer (USBTinyISP)

<img src="https://raw.githubusercontent.com/a3alamgi/AlvDuino/master/images/AlvDuinoBoard.jpg"/>  
Figure 1: AlvDuino PCB layout

<img src="https://raw.githubusercontent.com/a3alamgi/AlvDuino/master/images/AlvDuinoISP.jpg"/>  
Figure 2: Completed AlvDuino Board and USBTinyISP