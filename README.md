# MongoDB + Web GUI Setup Guide

This repository contains the setup files to run **MongoDB** alongside **Mongo Express** (a web interface) on your computer without installing MongoDB natively.

---

## Prerequisites

1. Download and install **Docker Desktop**:
   - [Windows / Mac / Linux Download Link](https://www.docker.com/products/docker-desktop/)
   - The installation is pretty straightforward. When asked whether you want to install Docker Desktop just for one user or system-wide, choose one user (the default option)
2. Make sure Docker Desktop is **running** in the background.
   - Start Docker Desktop from your applications. Just click on Accept in the initial screen, and then skip registration on the next screen. This should take you to the main Docker Desktop screen.

---

## How to Start the Database
1. Download the docker-compose.yml file from this repository to your computer, and remember where it is downloaded
1. Open your terminal or command prompt in the folder where the file was downloaded.
2. Run the following command to start the containers:

   docker compose up -d
