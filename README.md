# RasPad3

This repository is intended to collect resources, links and tips to configure your Raspad3 or correct problems.

# SD Image
* Flasher Image utility: www.balena.io/etcher
* Raspad3: https://raspad.com/pages/download
* RaspOS 32bit: https://www.raspberrypi.org/software/operating-systems/
* RaspOS 64bit: https://downloads.raspberrypi.org/raspios_arm64/images/

# User Manual
https://sunfounder.s3.us-east-1.amazonaws.com/Raspberry/RasPad-OS-User-Manual-20200824.pdf


# Accelerometer

cd ~

git clone https://github.com/sunfounder/python-sh3001

cd python-sh3001

sudo python3 install.py  

For how to use, you can refer to the auto-rotator.md file under the docs file in the python-sh3001 root directory (https://drive.google.com/file/d/1OoguOYlNk4iNunHv9ijh99rVqVEtWL_-/view?usp=sharing)

git clone https://github.com/sunfounder/python-sh3001.git

Then execute install.py installation program (reference picture: https://drive.google.com/file/d/1fc_519QyE2CeSjWHWDQKm9gzaF8dlgOW/view?usp=sharing).

According to the prompt of auto-rotator.md in the docs directory, you can turn on the rotating screen, turn off the rotating screen, or calibrate (refer to the picture: https://drive.google.com/file/d/1SiiyXDni3_NqCELY2GfISy-Uy5VRN8eE/view?usp=sharing).


Calibration procedure

https://raspad.readthedocs.io/en/latest/faq/RasPad3-FAQ.html#q-the-direction-of-the-display-does-not-change-with-the-direction-of-the-screen



# Fan speed

https://drive.google.com/file/d/1F-IQNld5OrlUfjvVT57f741fmzZzySto/view?usp=sharing



# Review

* MagPi : https://magpi.raspberrypi.org/articles/review-raspad-3?mc_cid=cbafa99eea&mc_eid=ea57cb1dcb
* Tom's Hardware : https://www.tomshardware.com/reviews/raspad-3


# Touchscreen

Are the two HDMI cables connected between the Raspberry Pi and the raspad3 motherboard in raspad3 connected? Is there an external screen?

Because the touch function cannot be used normally after the raspad is connected to the screen, we directly cancel the touch function when the screen is connected to the screen.

It is judged whether the external screen is connected with the voltage of HDMI. The voltage is the initial value when the two HDMI interfaces of the Raspberry Pi are connected to the radpad3 motherboard. Using the external HDMI interface on the raspad3 motherboard, or not connecting the HDMI cable between the Raspberry Pi HDMI1 interface and raspad3, will cause the voltage to deviate from the initial value, and the motherboard will make a judgment and turn off the touch.

If a longer HDMI cable is broken, it will also cause the voltage of the judgment state to deviate, thereby turning off the touch. You can exchange two hdmi cables for testing, refer to the attached video.

https://drive.google.com/file/d/1MMgZr508gCfPhtgimkBdnFgPQ1OWSHDO/view?usp=sharing

If the touch function does not work after checking step by step, please take a video about your checking process and effect so that the technician can better solve the problem. Please send the results to support@sunfounder.com, mark your backer number and problem description.

Thank you in advance.


# Virtual Keyboard

* florence  https://howtoraspberrypi.com/raspberry-pi-virtual-keyboard/
* matchbox https://thepihut.com/blogs/raspberry-pi-tutorials/matchbox-keyboard-raspberry-pi-touchscreen-keyboard

# File Manager
* Midnight Commander 


# YouTube Video

* ETA PRIME : https://www.youtube.com/watch?v=XPYfpia8OgE&t=13s 

# Sloeber (best Arduino IDE of ever)

`
sudo apt update

sudo apt install maven

git clone https://github.com/Sloeber/arduino-eclipse-plugin sloeber

cd sloeber

mvn clean verify -DskipTests=true
`
