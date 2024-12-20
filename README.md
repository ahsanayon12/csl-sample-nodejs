# csl-sample-nodejs

# Install Docker on your Ubuntu Machine 
# Step: 1
Add dependencies on you machine
````
# Add Docker's official GPG key:
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

````
# step:2
Install docker with updated docker file with docker compose plugins
````
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

````

# Step: 3
Build you image
````
docker build -t csl_testing .

````

# step: 4
check the docker image
````
docker images

````
````
docker image ls

````

# step : 5
run docker image on your PC
````
docker run -p 3000:3000 hello-docker
````


# Step : 6
 Install Nginx on your ubuntu machine

````
sudo apt-get install nginx
````
````
````
