# Deploying Web Application using Dockerfile

This repository is created to help those who want to try deploying web applications using a Dockerfile.

So, if you find this repository helpful for deploying your application on Docker, please show your appreciation to me and my colleague on Instagram @ghiyarandhika_ and @luqmann.rasyid.

## How to Deploy

1. Create Docker images with this command.
   For image with python-flask
   < docker build -t -f  Dockerfile-flask things-image . >

   For image with python-apache
   < docker build -t -f  Dockerfile-apache things-image . >

4. Create Container using image that has been created, using this command.
   For web-application using python-flask
   < docker run --name things-web -p 8080:5000 things-image -d >

   For web-application using apache
   < docer run --name thinigs-web -p 8080:80 things-image -d >

5. Thats it, you should be can access your web application from http://localhost:8080/.
