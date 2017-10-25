BootStrap: docker
From: mariadb:10.0


%runscript


%post
	sed -i  's/\/var\/lib/\/scratch/g' /etc/mysql/my.cnf
	sed -i  's/\/var\/log/\/scratch/g' /etc/mysql/my.cnf
	sed -i  's/\/var\/run/\/scratch/g' /etc/mysql/my.cnf
	sed -i  's/\/tmp/\/scratch/g' /etc/mysql/my.cnf
