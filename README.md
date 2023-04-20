In this project, we will deploy a 2048 game application.

Desired ouput image.png

Prerequisites:
1. Docker in local Machine (daemon is in running start)
2. AWS account to deploy application in Elastic Bean Stalk
3. Dockerfile


# Build the Image using Dockerfile and run it
Command 1: docker build -t 2048_game . 
// -t = tagging name for the image as 2048_game , Here periodic symbol(.) represent path of Dockerfile
Command 2: docker images
// list the images build by docker
Now, 
Command 3: docker run -d -p 80:80 2048_game
// deploy the application 2048_game image on port(-p) 80 in detach mode (-d)

# Aws Elastic bean Stalk deploy the application
Upload the file to aws elastic bean stalk and click on create . It will create application for you.

