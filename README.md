# CAN_NETWORK
Implementation of CAN communication between two Hercules Safety MCUs - TMS570LS1224 and TMS570LS1227. Interrupts were employed on each node to notify successful transmission and reception of messages on the CAN network. 

The Loop-back folder was used during debugging to check if the CAN module of each NODE was functional - this helped in eliminating the nodes as source of errors in the CAN network. 

Initial Setup of CAN network: Blue = VCU - TMS570LS1227; RED = BMS - TMS570LS1224 

  Issues: VCU's on-baord tranceiver & BMS external transceiver were not able to translate bits from TTL to CAN bus logic.
  
![CAN_image1](https://user-images.githubusercontent.com/33042545/68287322-640d0e80-0037-11ea-99e4-64212b4508d0.jpg)

Improved Setup: Used external transceivers for both VCU and BMS: 
 
 ![CAN_Image3](https://user-images.githubusercontent.com/33042545/68286984-d6312380-0036-11ea-81a1-f03fc3cc43eb.jpg)
 
 
Tested same code with two TMS570LS1224s:
  ![CAN_image2](https://user-images.githubusercontent.com/33042545/68287107-0aa4df80-0037-11ea-8e69-27d1713e73ad.jpg)


