# Network management & analysis

### `ifconfig` - system administration utility for network interface configuration

***

### `iwconfig` - dedicated for wireless interfaces 

***

### change IP address (static IP) 

`ifconfig eth0 192.168.181.115`  

***

### change IP with netmask and broadcast 

`ifconfig eth0 192.168.181.115 netmask 255.255.0.0 broadcast 192.168.1.255` 

***

### change MAC address (HWaddr) 

`ifconfig eth0 down` 

`ifconfig eth0 hw ether 00:11:22:33:44:55` 

`ifconfig eth0 up `

***

### get a new IP address from DHCP server 

`dhclient eth0 `

![dhcp-server-image](/assets/images/DHCP-server.jpeg)

***

### dig - Domain Information Groper

`dig portal.office.com ns` - ns - nameserver

`dig portal.office.com mx` 

***

### DNS configuration 

`nano /etc/resolv.conf` 

`echo "nameserver 8.8.8.8" > /etc/resolv.conf` 

If DHCP server defines DNS configuration, it replaces the resolv.conf file. 

### Using /etc/hosts file for custom domains 

`nano etc/hosts` 

***

`ip adress show`

`ip link show`  