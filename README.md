# SSACL
blacklist.acl https://raw.githubusercontent.com/AceLZG/SSACL/master/blacklist.acl

chnroute.acl white list, use 
```
curl 'http://ftp.apnic.net/apnic/stats/apnic/delegated-apnic-latest' | grep ipv4 | grep CN | awk -F\| '{ printf("%s/%d\n", $4, 32-log($5)/log(2)) }' > chnroute.txt
```
generate china ip
