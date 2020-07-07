# LAMP

## Version
- PHP7.4
- MySQL8.0

## PHP Extensions 
- bz2
- curl
- fileinfo
- gd
- gettext
- intl
- mbstring
- exif
- mysqli
- pdo_mysql
- pdo_sqlite
- openssl
- ftp
- xdebug

## Xdebug configure
- xdebug.idekey = "vscode"
- xdebug.default_enable = 1
- xdebug.remote_enable = 1
- xdebug.remote_autostart = 1
- xdebug.remote_host = host.docker.internal
- xdebug.remote_port = 9000

If you can't connect to the host from the container, set the IP address of the host to `xdebug.remote_host` instead of `host.docker.internal`.

## Port
- PHP: 80
- MySQL: 3306
- phpMyAdmin: 80
