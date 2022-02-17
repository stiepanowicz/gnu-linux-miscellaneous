
#### invert screen

`sudo nano /boot/config.txt`

add lines:

`lcd_rotate=2`

`display_rotate=2`

#### Waveshare DSI 7’ display configuration and bluetooth fix

<https://github.com/goodtft/LCD-show/issues/278>

`sudo mount /dev/mmcblk0p1 /media`

`vim /media/cmdline.txt`

change `console=ttyAMA0,115200` to `console=serial0,115200`

`sudo reboot` 

#### bluetooth fix and enable on boot

`sudo apt-get install pi-bluetooth`

`sudo systemctl enable hciuart.service`

`sudo systemctl enable bluetooth.service`

`sudo systemctl enable bluemon`

`sudo nano /boot/config.txt`

add `dtoverlay=pi4-enable-bt`

`sudo reboot`





