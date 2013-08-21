linux.shell
=====
This is a group of installation script, it can achieve fast initialization of your server.

Nginx
-----

    curl -s https://raw.github.com/netkiller/linux.shell/master/centos6.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/modules/ntp.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/filesystem/btrfs.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/nginx/nginx.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/php/5.4.x.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/php/redis.sh | bash

Apache httpd
------------

    curl -s https://raw.github.com/netkiller/linux.shell/master/centos6.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/modules/ntp.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/filesystem/btrfs.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/apache/httpd-2.4.4.sh | bash
    curl -s https://raw.github.com/netkiller/linux.shell/master/php/httpd.5.3.x.sh | bash 

Database
--------

    # curl -s https://raw.github.com/netkiller/linux.shell/master/modules/mongodb.sh | bash 
    # curl -s https://raw.github.com/netkiller/linux.shell/master/modules/redis.sh | bash
    # curl -s https://raw.github.com/netkiller/linux.shell/master/database/postgresql.sh | bash
    
Node Install
------------

    if [ "$( hostname )" == "www.mydomain.com" ]; then
		curl -q -s https://raw.github.com/netkiller/linux.shell/master/centos6.sh | bash
		curl -q -s https://raw.github.com/netkiller/linux.shell/master/modules/nginx.sh | bash
        echo '====================================================================='
    fi

    if [ "$( hostname )" == "db.mydomain.com" ]; then
		curl -q -s https://raw.github.com/netkiller/linux.shell/master/centos6.sh | bash
		curl -q -s https://raw.github.com/netkiller/linux.shell/master/modules/mysql.sh | bash
        echo '====================================================================='
    fi
