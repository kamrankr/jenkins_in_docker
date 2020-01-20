A test on running Jenkins in docker container and running docker in dockerize jenkins.



docker-compose up -d



Issues on docker socket permission

- login into container as root user
- groupadd docker
- usermod -a -G docker jenkins
- chown root:jenkins /var/run/docker.sock 

From host machine where docker is running restart docker