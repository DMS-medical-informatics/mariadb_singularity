BootStrap: debootstrap
OSVersion: trusty
MirrorURL: http://us.archive.ubuntu.com/ubuntu/


%runscript
    echo "This is what happens when you run the container..."


%post
    sed -i 's/$/ universe/' /etc/apt/sources.list
    apt-get update
    cat > /usr/sbin/policy-rc.d < < EOF
    #!/bin/sh
    echo "runlevel denied" >&2
    exit 101
    EOF
    apt-get install -y mariadb-server-5.5
