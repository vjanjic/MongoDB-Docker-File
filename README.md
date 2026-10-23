# MongoDB + Web GUI Setup Guide

This repository contains the setup files to run **MongoDB** alongside **Mongo Express** (a web interface) on your computer without installing MongoDB natively.

---

## Prerequisites

1. Download and install **Docker Desktop**:
   - [Windows / Mac / Linux Download Link](https://www.docker.com/products/docker-desktop/)
   - The installation is pretty straightforward. When asked whether you want to install Docker Desktop just for one user or system-wide, choose one user (the default option)
2. Make sure Docker Desktop is **running** in the background.
   - Start Docker Desktop from your applications. Just click on Accept in the initial screen, and then skip registration on the next screen. This should take you to the main Docker Desktop screen.
   - Once you are in Docker Desktop, go to the Settings menu (the gear icon in the top panel, or click Settings in the side panel), and from there enable the Enable integrated terminal option. 

---

## How to Start the Database
1. Download the docker-compose.yml file from this repository to your computer, and remember where it is downloaded. You can download it by clicking on it from the GitHub repository, and then, once it is opened, clicking Download.
1. Open the terminal in Docker Desktop. It can be found in the lower right corner of your Docker Desktop, next to the version number in blue. The icon to launch it has >_ symbols in it.
2. Within the terminal, move to the directory where you have downloaded the docker-compose.yml file. If you haven't changed anything, this will be the Downloads folder, which you can move to by typing
   cd Downloads
3. Run the following command to start the containers:
   docker compose up -d
4. That's it! MongoDB as well as its front end should be running now. Exit the terminal by clicking X, and in the main Docker Desktop window, click Containers in the left panel. You should see one container running, with green light next to it. Expanding this container by clicking on > next to the green light should show mongodb and mongodb-express running.
5. NOTE: In future, whenever you want to start MongoDB, you just need to start it from the list of containers in Docker Desktop - no need to mess around with the terminal. Go ahead and try this: first, stop the container by clicking on the stop button (big blue square under Actions for your container), then restart it by clicking on start (the white triangle, again under Actions).
6. Once the container is started, check that MongoDB is running by opening your favourite web browser and entering localhost:8081 in the address tab. This should open Mongo Express interface, where you should see the databases (admin, config and local, by default), plus a bunch of information about the server settings. If this is the case, congratulations, you have MongoDB and interface to it up and running and you can start doing some serious document databasing.
