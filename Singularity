BootStrap: docker
From: mariadb:10.0


%runscript
    echo "This is what happens when you run the container..."


%post
	mount /scratch 
	sed -i  's/\/var\/lib/\/scratch\/lib/g' my.cnf
	sed -i  's/\/var\/log/\/scratch\/log/g' my.cnf
	sed -i  's/\/var\/run/\/scratch\/run/g' my.cnf
	sed -i  's/\/var\/lib/\/scratch\/lib/g' my.cnf
	sed -i  's/\/tmp/\/scratch\/tmp/g' my.cnf
