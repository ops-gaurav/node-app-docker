# Configuring Docker Node project #

This is a simple hello world project developed to demonstrate how to create nodeJS images in docker.

### Prerequisite installations ###

* Install docker by following instructions from here [https://www.docker.com/get-docker](https://www.docker.com/get-docker)
* Docker hub/ Docker Cloud account
* Cloud service (e.g AWS, DigitalOcean etc.)

### How do I get set up? ###

* Clone this repo using 
```

git clone https://sharma02gaurav@bitbucket.org/sharma02gaurav/node-app-docker.git
```

* switch to node-app-docker folder
* Run the following command to build the Image
```

docker build -t [your-image-name] .
```
This will build the image for you.
* Now you can run this image locally using
```

docker run -p [access-port]:[redirect-port] [your-image-name]
```

* You have to push this image into docker cloud using the following command. Make sure you have the docker account.

```

docker tags [your-image-name]:[label] [docker-user-name]/[repo-name]
docker push [docker-user-name]/[repo-name]
```

### Deployment Instructions ###

* Create DigitalOcean account. Use referral account to get 10$ credit. Here is mine [Sign up using this to get 10$ credit on Digital Ocean](https://m.do.co/c/3a65d5a3f890)

* Create a Docker droplet.
* Log into Docker from terminal using ssh.
* Run following command to start image in container
```

docker run -p [incoming-port]:[redirect-port] [docker-user-name]/[repo-name]
```
for example

```

docker run -p 80:4300 sharma02gaurav/my-node-app
```
