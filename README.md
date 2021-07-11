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



## Notes:
-	The system is using visual representation by using LEDs with the assumption that a physical dot output should be raised in replace of each ON LED.
	
-	Although we only need four outputs to represent the pattern of a number from 0 to 9; We are using six outputs, In case the system may developed to include the whole Braille alphanumeric system which needs all the six outputs.

