# Node.js interface for pan and tilt camera mechanism
## Hardware
Pan Servo SIG connected to GPIO 23

Tilt Servo SIG connected to GPIO 24

*Do not power the servos from the Raspberry Pi. Use external power supplies with common GND*

---
## Installation

From a clean Raspberry Pi image,

Install Node.js and npm

    https://docs.npmjs.com/downloading-and-installing-node-js-and-npm

Install the pigpio library for nice smooth pulse generation on the pi

    sudo apt install pigpio

Clone this github repository

    git clone https://github.com/rwlloyd/nodejs-panandtilt.git

Install the required node packages

    npm install https://github.com/rwlloyd/nodejs-panandtilt.git

Run the server. sudo is currently required to access the physical pins

    sudo node server.js

---

## Usage

Connect to the device from a web browser:

    http://<ipaddress>:3000

Control currently limited to controlling the pan and tilt mechanism.



