# Permissions

![permissions](/assets/images/permissions.jpeg)

### check permissions 

`ls -l /usr/share/hashcat `

***

### change file ownership 

`chown bob /tmp/bobsfile `

***

### changing group ownership 

`chgrp security file.fff` 

***

### changing permissions 

`chmod 774 hashcat.hcstat2` 

***

### changing permissions with UGO 

`chmod u-w hashcat.hcstat2` - disable "write" for user 

`chmod u+x,o+x hashcat.hcstat2` - enable "execute" for user, enable "execute" for owner 

`chmod a+x hashcat.hcstat2` - enable "execute" for all 

***

### changing umask default permissions 

`cat /home/user_name/.profile` 

***

### SUID bit 

`find / -user root -perm –4000` 

### SGID bit 