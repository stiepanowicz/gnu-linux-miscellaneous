# Text operations

### `head` - displays first 10 lines (or more) 

`head /etc/snort/snort.conf` 

`head -20 /etc/snort/snort.conf`  

***

### `tail` - displays last 10 lines (or more) 

`tail /etc/snort/snort.conf` 

`tail -30 /etc/snort/snort.conf` 

***

### `nl` - numbering lines 

`nl /etc/snort/snort.conf` 

***

### `grep` - global regular expression print 

cat /etc/snort/snort.conf | grep output 

tail -n+507 /etc/snort/snort.conf | head -n 6 

sed - stream editor 

cat /etc/snort/snort.conf | grep mysql 

sed s/mysql/MySQL/g /etc/snort/snort.conf > snort2.conf 

cat snort2.conf | grep MySQL 

sed s/mysql/MySQL/2 snort.conf > snort2.conf 

more - scrolling file 

more /etc/snort/snort.conf 

/key_word 

n - next 

 

 

 

 