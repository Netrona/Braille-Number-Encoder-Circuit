# Braille-Number-Encoder-Circuit

This project was done for PC/CP220 class at WLU, Fall 2016

## Description:
Braille Number Encoder Circuit is designed to help blind or visually damaged people. The system converts binary representation of number from 0 up to 9, to a visual pattern as shown in the figure below. 

Binary number to Braille Number conversion: 

![image](https://user-images.githubusercontent.com/47288950/125186076-8867b800-e228-11eb-8553-eadde9f2dda6.png)

## Inputs:

Using DIP switch, Braille Number Encoder Circuit will have four inputs, i_0 to i_3, in which they are used to provide the binary number representation from 0 to 9. 

According to Decimal-Binary conversion table:
 
![image](https://user-images.githubusercontent.com/47288950/125186090-9d444b80-e228-11eb-8ef2-93c829ec8d95.png)


## Outputs:
Using LEDs outputs, Braille Number Encoder Circuit will have six outputs, p0 to p5, like Figure 2 which is oriented in the patterns as seen in figure1. LEDs must light(ON) to give every number a distinct pattern as shown in the figure.


![image](https://user-images.githubusercontent.com/47288950/125186130-d4b2f800-e228-11eb-8c81-64ffed3c759f.png)



### Notes:
-	The system is using visual representation by using LEDs with the assumption that a physical dot output should be raised in replace of each ON LED.
	
-	Although we only need four outputs to represent the pattern of a number from 0 to 9; We are using six outputs, In case the system may developed to include the whole Braille alphanumeric system which needs all the six outputs.


## Logic Equations:
The project has six outputs from P_0 to P_5, but P_2 and P_3 are not in use. Therefore, we only have four logic equations to implement:

<img width="432" alt="Screen Shot 2021-07-11 at 3 20 24 AM" src="https://user-images.githubusercontent.com/47288950/125186210-45f2ab00-e229-11eb-953d-d68fee792cf1.png">

where i_3 is the most significant bit of the input, and i_0 is the least significant bit of the input. **We test the logic in file Logic_Testing.pdf 

## Circuit Diagram:

Altera Quartus II is used to draw our circuit, and is shown in the following figure. 

![image](https://user-images.githubusercontent.com/47288950/125186233-6cb0e180-e229-11eb-9e4a-0b9ff9fbd16c.png)


## Simulation Output:

For four bits combination we have 16 possibilities. Since we are only interested in the decimals from 0 to 9, we are going to ignore the possibilities which are 1010, 1011, 1100, 1101, 1110, and 1111.
Based on the simulation followed below, we can prove that all of results are true.

<img width="1025" alt="Screen Shot 2021-07-11 at 3 23 34 AM" src="https://user-images.githubusercontent.com/47288950/125186271-aeda2300-e229-11eb-87ed-53a20af8462d.png">


## Parts List: 
•	CPLD Board for prototyping the design

•	DIP switch for the inputs

•	1kΩ Resistor array for the DIP switch

•	6 LEDs for the outputs

•	6 of 510Ω Resistors for the LEDs




