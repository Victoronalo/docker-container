
# docker-container
Project: Docker Containers


Objective: To have more knowledge of docker containers.



-I created an EC2 instance named “docker-container”



-The instance is on Ubuntu AMI.


-I also created a key pair called docker-keys


-I ssh into the EC2 instance using
         *ssh -i "docker-keys.pem" ubuntu@ec2-18-207-174-255.compute-1.amazonaws.com


-The ssh was successful



-To install docker on the instance I used the below commands.



sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update



-To check the status, I ran the command “ docker info”



-I ran docker run Ubuntu



-I ran the command “docker start  optimistic_sanderson”



-I ran the command “docker stop  optimistic_sanderson”



-Then I ran the command “docker restart  optimistic_sanderson”



-To remove container, I ran the command “docker rm optimistic_sanderson”



-I checked the docker status.


This project has given me more insight into docker image and I learnt a lot.

