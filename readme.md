# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## Installation

### Reqirements

To run / install this project, you'll need:

* [Docker](https://docs.docker.com/get-docker/) - You can download and install Docker on multiple platforms.

#### **Linux**

 I followed these steps for setting up my environment in my linux machine.
 
Recommended approach to install Docker Desktop on Ubuntu:

1. Set up [Docker’s package repository](https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository).

2. Download latest [DEB package](https://desktop.docker.com/linux/main/amd64/docker-desktop-4.13.1-amd64.deb?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-linux-amd64).

3. Install the package with apt as follows

```bash
sudo apt-get update

sudo apt-get install ./docker-desktop-<version>-<arch>.deb
```
To start Docker run

    systemctl --user start docker-desktop

You can verify docker is ready by running the following commands in your terminal:&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: yellow">docker &nbsp;&nbsp;-v </span>&nbsp;and&nbsp;&nbsp;&nbsp;<span style="color: yellow">docker-compose &nbsp;&nbsp;-v </span>

Now Clone the repo to your local machine.

Then, run &nbsp;&nbsp;<span style="color: yellow">docker-compose  &nbsp;up </span>&nbsp;&nbsp;from the project root directory to load Anythink's backend and frontend.

If Docker is working correctly, the backend should be running and able to connect to your local database.
Let's test this by pointing your browser to http://localhost:3000/api/ping

Check the frontend and make sure it’s connected to the backend.
If everything is working properly, you’ll be able to create a new user on http://localhost:3001/register