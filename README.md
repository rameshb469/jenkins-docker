# jenkins-docker
Docker image for jenkins with docker support    
##Note-  Chnage the line `docker-ce=17.12.1~ce` depending on ther version of docker client you need to use.

Build the image using below command.
    docker image build -t jenkins-docker .

start Jenkin contianer 
    docker container run -d -p 8080:8080 -v /var/run/docker.sock:/var/run/docker.sock jenkins-docker
    
    
Then bowse <ip-address>:8080
