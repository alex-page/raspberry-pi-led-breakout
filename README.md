# Raspberry Pi LED Breakout

> 💡 Control Raspberry Pi [LED breakout](https://shop.pimoroni.com/collections/electronics?filter=LED+Displays)'s with Node JS


## You will need

- [A raspberry pi](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/)
- [Power supply](https://www.raspberrypi.org/products/type-c-power-supply/)
- [microSD card](https://shop.pimoroni.com/products/noobs-32gb-microsd-card-3-1)
- [microHDMI to HDMI cable](https://www.raspberrypi.org/products/micro-hdmi-to-standard-hdmi-a-cable/)
- An [LED breakout](https://shop.pimoroni.com/collections/electronics?filter=LED+Displays) connected to the raspberry pi


## Get started

### Set up the Raspberry Pi

1. Download [raspbian lite](https://www.raspberrypi.org/downloads/raspbian/)
1. Install the operating system by flashing the microSD card with the `.img` file. You can use [etcher](https://github.com/balena-io/etcher).
1. If you have ethernet cable, keyboard and monitor, plug them into your raspberry pi and skip to step 5. If you do not you can set up the [raspberry pi headless](https://www.raspberrypi.org/documentation/configuration/wireless/headless.md).
1. SSH into the raspberry PI `ssh pi@raspberrypi.local` (password: `raspberry`)
1. Run `sudo raspi-config` to finish setting up your Raspberry Pi


### Instal Node JS

1. Update and upgrade the installed packages `sudo apt-get update && sudo apt-get upgrade`
1. Install NVM to your Raspberry Pi `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash`
1. Restart `sudo reboot`
1. Reconnect with SSH `ssh pi@raspberrypi.local`
1. Check NVM is installed and working `nvm --version`
1. Install Node JS and NPM `nvm install node`.
1. Test that node and NPM work `node --version && npm --version`


### Set up Visual Studio Code to edit files remotely

1. Install the [Remote SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh) extension
1. Click the remote explorer icon in the side bar and input `pi@raspberrypi.local`
1. Click the folder icon next to `raspberrypi.local`
1. Enter the password in `raspberry`


### Control LED's with Javascript

1. Install this package `npm install raspberry-pi-led-breakout`
1. 


## Release history

- v0.0.0 - 
