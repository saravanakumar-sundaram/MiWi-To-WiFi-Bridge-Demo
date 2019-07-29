# MiWi to WiFi Bridge Demo with AWS

Create a Wi-Fi/ MiWi (15.4) / LoRa wireless sensor network to monitor the temperatures covering a wide area like a hotel or a plant.

## Introduction
This application notes describe the MiWi to WiFi bridge demo application with its test setup information. The MiWi to WiFi bridge application helps to monitor and control the MiWi network through Wi-Fi bridge and AWS EC2 instance provided Amazon Machine Image (AMI)  as an infrastructure service. WSN monitor tool will be used to monitor and control the network, connected through AWS cloud.

For MiWi network SAMR30 Xplained pro boards are used. In the MiWi network, only one PAN coordinator and N number of routers or coordinator and end-devices are used.
For WiFi bridge, SAMA5D2 Xplained pro board connected WILC1000 SD board in SDIO interfaces used to access the network connectivity.

AWS EC2 instance service is used to run the TCP server to connect with both WiFi bridge and WSN monitor tool through TCP clients.

The python script is used to develop the TCP server and client to connect and communicate with the MiWi network and WSN monitor tool. 

MiWi applications are used from ASF release and Linux kernel is used for WiFi connectivity

## Features

- Monitors sensor data (temperature, battery level and RSSI)
- Covers 34-35 locations over a vast area of approx. 1 km2
- Secure communication with AWS IoT for Wi-Fi and MiWi
- WSN Monitor tool will display the MiWi network with connections 
- More than one WSN Monitor tool could be connected remotely.
- Battery operated devices
- Showcase different technologies tackling the same task

## Hardware Platform

- ATSAMR34-XPRO – 3 Nos minimum (one PAN, one Router, one End-Device)
- ATSAMA5D2-Xplained Ultra board
- ATWILC1000 SD board
- Internet Gateway connectivity

## Software Platform

- Linux machine - Ubuntu 
- Windows machine
- BuildRoot image
- Linux Kernel 4.14.73 used from Linux4sam_6.0
- WILC1000 Driver and firmware 15.02 release
- Python 2.7
- AWS Cloud Server account 
- WSN monitor Tool 2.2.1
- ASF 3.46 MiWi Applications

   **Smart Secure Connected**
![](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)

## Demo Building Blocks & Flow

![GitHub Logo](/Images/Block-Daigram.png)


```bash
pip install foobar
```
