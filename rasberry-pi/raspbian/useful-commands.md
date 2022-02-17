## Useful commands

#### check bootloader version

`vcgencmd bootloader_version`

#### force bootloader update

`sudo rpi-eeprom-update -a`

#### check bootloader configuration

`vcgencmd bootloader_config`

#### check connected usb devices

`lsusb -t`

## SSH into Raspberry Pi 

#### setup user password 
`passwd`

#### check ip

`hostname -I`

#### enable ssh

`sudo raspi-config`

#### enable ssh in terminal

`sudo systemctl status ssh.service` 

`sudo systemctl enable ssh.service`

`sudo systemctl start ssh.service`

#### Disable SSH Root Login

`nano /etc/ssh/sshd_config`

`#PermitRootLogin prohibit-password` -> `PermitRootLogin no`

#### restart ssh server

`/etc/init.d/sshd restart`

#### Connect

`ssh user@[address]`

