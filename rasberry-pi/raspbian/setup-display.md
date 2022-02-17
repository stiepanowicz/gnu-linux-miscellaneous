## Waveshare DSI 7’ display configuration

##### If you are using the Buster branch system, the DSI LCD can work with Raspberry Pi directly after connecting and powering on. But if you are using the Bullseye branch system, you need to modify the `config.txt` as below:

##### Open the `config.txt` file in the root directory of the TF card(/boot), comment out the following lines:
`#camera_auto_detect=1`
`#dtoverlay=vc4-kms-v3d`

##### Add the following lines under `[all]`:
`dtoverlay=vc4-fkms-v3d`
`start_x=1` 

##### Then save the file and reboot the system:
`sudo reboot`

## Backlight controlling
`wget https://www.waveshare.net/w/upload/3/39/Brightness.tar.gz`
`tar -xzf Brightness.tar.gz`
`cd brightness`
`./install.sh`

##### Menu -> Accessories -> Brightness
