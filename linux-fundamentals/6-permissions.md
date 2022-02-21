# Permissions

![permissions](/assets/images/permissions.jpeg)

### check permissions 

`ls -l /usr/share/hashcat `

### change file ownership 

`chown bob /tmp/bobsfile `

### changing group ownership 

`chgrp security file.fff` 

### changing permissions 

`chmod 774 hashcat.hcstat2` 

### changing permissions with UGO 

chmod 1u-w hashcat.hcstat2 

1 disable "write" for user 

chmod 1u+x,2o+x hashcat.hcstat2 

1 enable "execute" for user 

2 enable "execute" for owner 

chmod 1a+x hashcat.hcstat2 

1 enable "execute" for all 

changing umask default permissions 

cat /home/user_name/.profile 

SUID bit 

find / -user root -perm –4000 

SGID bit 