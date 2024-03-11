## RFID Handheld

This is a small handheld device for reading and writing RFID tags. It has a TFT LCD, Wi-Fi module and SD card. MRFC522 is used as a RFID reader IC.



###### Design Features

- Custom RFID antenna design on PCB

- Wi-Fi Connection

- TFT LCD with FSMC connection

- Keyboard with full buttons

  

###### Featured Applications

- Read / Write RFID tags
- Retail
- Chain store



###### Block Diagram

Image ---> Fig 1

The overall view of designed system is shown in Fig.1.



![Block diagram](https://github.com/hosein-mokarian/RFID-Handheld/blob/main/Fig/RFID_Handheld.jpg)

<div style="text-align: center;">
    <p>Fig 1. Block Diagram</p>
</div>




###### Board Image

3D Image of Board ---> Fig.2

Fig.2 shows the 3d view of designed board on the Altium Designer software. 

![Block diagram](https://github.com/hosein-mokarian/RFID-Handheld/blob/main/Fig/RFID_Handhels_top.JPG)
![Block diagram](https://github.com/hosein-mokarian/RFID-Handheld/blob/main/Fig/RFID_Handhels_bottom.JPG)

<div style="text-align: center;">
    <p>Fig 2. Board Image</p>
</div>



###### Key System Specifications

- Battery: 3.7V
- Wi-Fi communication
- Supports MicroSD Card up to 16GB
- Read / Write Mifare RFID tags with frequency of 13.56 MHz



###### Introduction

This repository provides an open source RFID Handheld device. It is for reading and writing RFID tags. The device is portable and operates on battery. So it is suitable for retails, product tracks and chain stores. A Wi-Fi connection helps users to send or receive data to or from a server side. Also there is a MicroSD card which can be used to save data locally. A small keyboard with full buttons provides all users need to write something. A colorful TFT LCD is used to show UIs. All of those parts will be described in details in the following.



###### System Description

--->



###### Block Diagram





###### MCU:

STM32F427VIT6 is used as a brain of the whole system. It has some interesting features. FSMC connection helps to have a reliable and high speed connection with TFT LCD. Also FSMC controller makes the main core to be free from driving TFT LCD. So the MCU can show reaction to user events very fast. 4 bits SDIO connection for diving MicroSD card is really amazing. 4 lines data cause more speed for reading pr writing on MicroSD card. Maximum core frequency 168 MHz and 96 kB RAM are really enough to make a device with reasonable speed.



###### TFT LCD:

The resolution of TFT LCD is 240 * 240. It ls 2.4 inches. 16 bits parallel communication is used.



###### SD Card:

The high capacity SD card is used. It can have capacity up to 16 GB. FatFs is used as a firmware to handle file system formats. The connection with the MCU is through SDIO.



###### Wi-Fi Module:

ESP32 module is used as wireless communication with a server. It connects to the MCU through UART.



###### Keyboard:

a custom keyboard is designed for the device. It uses small tactile switches. They really good for situation which there is a limited space. They helps to have a keyboard with full buttons operation. a matrix network is used to read what buttons are pressed.



###### Power Supply:

The device can be supplied by USB and battery. Also there is a battery charger IC to recharge the battery. 



###### RFID Reader/Writer IC:

MRFC522 is used as controller IC. It is really conventional for reading and writing RFID tags. Here it is used with a custom antenna. 



###### RFID Antenna:

A custom antenna is designed based on our device and it is done by a tools which is released by NXP. It is a software to calculate impedance matching network component and also to set up the width, height and number of turns for antenna.



###### System Design Theory





###### Simulation





**Schematics**



**Bill of Materials**



**PCB Layout**



**Altium Project**



**Layout Guidelines**



**Test Setup**



**Test Data**



**References**



