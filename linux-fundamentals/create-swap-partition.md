# create a new partiition
`sudo dd if=/dev/zero bs=1M count=1024 of=/mnt/1GiB.swap`

# upgrade the permissions
`sudo chmod 600 /mnt/1GiB.swap`

# make partition into swap 
`sudo mkswap /mnt/1GiB.swap`

# turn it on 
`sudo swapon /mnt/1GiB.swap`

# verify
`cat /proc/swaps`

# add to filesystem table to be used at boot
`echo ‘/mnt/1GiB.swap swap swap defaults 0 0’ | sudo tee -a /etc/fstab`