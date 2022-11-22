## Repo
Ansible Container

## Description
This project allows the user to build an image and run a container that will allow the user to run an ansible-playbook
The playbook will be created with multiple roles that should run an apache server and establish connection through your localhost

## Installation
You can build and run container from CLI or IDE
Below lays out instructions on how to build/run from both

## From CLI
The only time your working folder should be considered is when building your image
Since dockerfile sits inside of a .devcontainer please be sure to change directory into .devcontainer
The commands assume that you are in .devcontainer of the NGINX-ANSIBLE project
Please note that the term 'the user' is referencing you as the developer running the commands

## Building the Image
docker build -t  -f ansible .
    \n- NOTE:  is arbitrary but best practice is to follow semantic versioning format: imageName:0.0.1
## Running the Container
docker run -dit --name  
    \n- NOTE:  is arbitrary; it is to better help the user remember the container name which will be needed later
    \n- NOTE:  is the tag name the user assigned the image in the Build stage
## Execute the Container CLI
docker exec -it  ash
    \n- NOTE:  is name the user assigned in running the container