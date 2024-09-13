

Prerequisite for Wazuh to be deployed on Docker. 

Increase max_map_count

#sysctl -w vm.max_map_count=262144

Install Docker

#curl -sSL https://get.docker.com/ | sh

Start Docker service

#systemctl start docker

Install Docker Compose

curl -L "https://github.com/docker/compose/releases/download/v2.12.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

Grant execution permissions

chmod +x /usr/local/bin/docker-compose

Test the installation

docker-compose --version
