## Template to create a basic Flask app and run it using Docker

- This repository is meant to explain how to containerize a simple Flask Application using Docker

### Steps to run the code
- To run it without using docker, make sure to install all the packages within the requirements.txt file and then type ```python app.py```, you should see the link to the server.
#### Initial setup
- You would first need to install docker from here https://www.docker.com/get-started
- Clone this repository

#### Preliminray checks:
  - Open your terminal/command prompt
  - Go into the folder ****Docker_basics****
  - Type the command ```docker run hello-world``` to check to see if you have docker install correctly

#### Building the docker image
  - Make sure you are inside the folder ****Docker_basics**** which should have the ****Dockerfile****
  - Run the command ```docker build -t "image_name" .```
  - Wait for the image to be built
  - After this is complete run ```docker images``` and look for your image

#### Running the container
  - Once you have built your image its time to run the container
  - Run the command ```docker run -d -p 127.0.0.1:5000:5000 "image_name"```

#### Go to the link http://127.0.0.1:5000 and you should see your app running!

# Congrats you just containerized your first docker app!
