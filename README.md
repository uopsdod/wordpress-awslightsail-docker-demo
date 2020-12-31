
#### step01: create an AWS Lightsail instance 
#### step02: install docker & start it
* sudo yum install docker -y 
* sudo service docker start
* sudo docker --version
#### step03: install docker compose 
* sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
* sudo chmod +x /usr/local/bin/docker-compose
* sudo /usr/local/bin/docker-compose --version

#### step04: install git 
* sudo yum install git -y
#### step05: download git project
* sudo git clone https://github.com/uopsdod/wordpress-awslightsail-docker-demo.git

#### step06: start your git project with docker-compose 
* check network inbound rules on AWS Lightsail 
* cd ./wordpress-awslightsail-docker-demo/
* cat docker-compose.yml
* sudo /usr/local/bin/docker-compose up -d
* sudo docker container ls

#### step07: close it
* sudo /usr/local/bin/docker-compose down

#### other: 
* allocate static ip
* create DNS zone 

