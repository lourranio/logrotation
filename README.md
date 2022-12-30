# logrotation



## CONFIGURACAO

Configure Log Rotation

```
FILE="/etc/logrotate.d/owncloud"
sudo cat <<EOM >$FILE
/var/www/owncloud/data/owncloud.log {
  size 10M
  rotate 12
  copytruncate
  missingok
  compress
  compresscmd /bin/gzip
}
EOM

```

```
https://doc.owncloud.com/server/next/admin_manual/installation/quick_guides/ubuntu_20_04.html
```
