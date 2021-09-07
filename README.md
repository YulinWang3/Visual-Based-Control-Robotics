# Visual-Based-Control-Robotics

This project contains two main parts: computer (client) and Raspberry Pi (server).

The main parts for the Raspberry Pi (server) program are:
1. Sends 'live' camera images to the computer (client)
2. Receives the direction instructions from the computer (client)
3. Executes the direction instructions by controlling the hardware through pins output

The main parts for the computer (client) program are:
1. Provides user interface to connect to the Raspberry Pi (server) with two modes: control mode and tracking mode
2. Receives the 'live' camera images from the Raspberry Pi (server) and display to user
3. Sends the direction instructions to the Raspberry Pi (server)

There are two modes for user to select from the computer (client) program:
1. Control mode: allow user to control the movement of the Raspberry Pi (car) using the keyboard arrow key inputs
2. Tracking mode: required user to select a rectangle from the image, use openCV to tracking the selected object, and send the directio instructions to the Raspberry Pi (server)