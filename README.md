Docker syslog-ng Server
=======================

This installs Ubuntu 18.04 running a syslog-ng Server.

Syslog messages will be received to the console as well as saved on the Docker  host file 'syslog.log'.

Be sure to copy the supporting files to a new directory.  Easiest to do with:

```php
git clone https://github.com/ajoldham/syslog-ng
```

Download pre-built image from Docker Hub with:

```php
docker pull ajoldham/syslog-ng
docker tag ajoldham/syslog-ng syslog-ng
```

-or-

Build with:
```php
docker build -t syslog-ng .
```

Run with:
```php
docker-compose up
```

Notes:  You may need to disable/allow a local firewall to receive UDP 514 DNS requests in Docker.
