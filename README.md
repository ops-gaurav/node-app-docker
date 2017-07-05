# Configuring Docker Node project #

This is a simple hello world project developed to demonstrate how to create nodeJS images in docker.

### Prerequisite installations ###

* Install docker by following instructions from here [https://www.docker.com/get-docker](https://www.docker.com/get-docker)
* Docker hub/ Docker Cloud account
* Cloud service (e.g AWS, DigitalOcean etc.)

### How do I get set up? ###

* Clone this repo using 
```
#!command

git clone https://sharma02gaurav@bitbucket.org/sharma02gaurav/node-app-docker.git
```

* switch to node-app-docker folder
* Run the following command to build the Image
```
#!command

docker build -t [your-image-name] .
```
This will build the image for you.
* Now you can run this image locally using
```
#!command

docker run -p [access-port]:[redirect-port] [your-image-name]
```

* How to run tests
* Deployment instructions

### Contribution guidelines ###

* Writing tests
* Code review
* Other guidelines

### Who do I talk to? ###

* Repo owner or admin
* Other community or team contact