# aws-docker-django
Dockerized django setup on AWS


# steps to run boot2docker

1. RUN `boot2docker up`
2. RUN `boot2docker shellinit`
3. Copy paste and run the export lines
4. RUN `docker build -t <appname> .` # do this *once* after you make 
5. RUN `docker run --name <docker_instance_name> -d -p 80:80 <appname>`
6. RUN `boot2docker ip` #get the ip address

# steps to shut down the docker image
1. RUN `docker down <docker_instance_name>`
2. RUN `docker rm <docker_instance_name>`

# steps to shutdown the boot2docker
1. Shut down all running images
2. RUN `boot2docker down`

