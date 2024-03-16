# Docker-Documentation
Step 1
Start my Virtual machine (I’m using Ubuntu) and run the sudo apt update command.

Step 2 
Uninstall conflicting packages
sudo apt-get remove docker docker-engine docker.io containerd runc

Step 3
Install pre requisites 
sudo apt-get update
sudo apt-get install -y apt-transport-https ca-certificates curl software-properties-common

Step 4
Add the Docker GPG key:
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

Step 5
Add the Docker repository:
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"

Step 6
Update package lists and install Docker Engine:
sudo apt-get update
sudo apt-get install docker-ce

Step 7
Add permission to user for docker group 
sudo chmod 666 /var/run/docker.sock

Step 8 
Verify Docker installation:
docker run hello-world


Step 9 
Pull the CentOS container image:
docker pull centos:latest 

Step 10
Run Centos container image and name it 
docker run -d -t --name mycent centos

Step 11
Run Kali Linux container and name it 
docker run -d -t --name mykali kalilinux/kali-rolling

Step 12
Check running containers 
docker ps


Step 13 
Go in to Centos container 
docker exec -it mycent bash

Step 14 
Leave container 
exit
 
Step 15 
Go into Kali container 
docker exec -it mykali bash

Step 16
Leave container 
exit
