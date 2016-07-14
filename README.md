# Sulu Minimal Edition

Welcome to the Sulu Minimal Edition - a fully-functional Sulu application that you can use as the skeleton for your new
applications.

## Installation

__Mac:__

```
rm -rf var/cache/*
rm -rf var/logs/*
HTTPDUSER=`ps axo user,comm | grep -E '[a]pache|[h]ttpd|[_]www|[w]ww-data|[n]ginx' | grep -v root | head -1 | cut -d\  -f1`
sudo chmod +a "$HTTPDUSER allow delete,write,append,file_inherit,directory_inherit" var/cache var/logs var/uploads var/uploads/* web/uploads web/uploads/* var/indexes var/sessions var/sessions/*
sudo chmod +a "`whoami` allow delete,write,append,file_inherit,directory_inherit" var/cache var/logs var/uploads var/uploads/* web/uploads web/uploads/* var/indexes var/sessions var/sessions/*
```
