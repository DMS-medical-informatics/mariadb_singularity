BootStrap: debootstrap
OSVersion: trusty
MirrorURL: http://us.archive.ubuntu.com/ubuntu/


%runscript
    echo "This is what happens when you run the container..."


%post
    sed -i 's/$/ universe/' /etc/apt/sources.list
    apt-get update
    echo exit 101 > /usr/sbin/policy-rc.d
    chmod +x /usr/sbin/policy-rc.d
    apt-get install -y mariadb-server-5.5
