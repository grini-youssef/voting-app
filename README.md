# Voting app
voting-app is an application based on the microservices architecture and DevOps methodology. to create this application we used git, Docker, Jenkins, Kubernetes.
It allows everyone to vote for their preferred candidate, to change their vote if they feel they are wrong, as well as to see the number of votes cast and the approval rating of each candidate.
## Architecture
This application consists of 5 microservices:
* Voting-app : web application developed in python (Flask Framework) which lets you vote between two options
* Redis : queue which collects new votes
* Worker : which consumes votes and stores them in database
* Postgresql : database backed by a Docker volume
* Result-app : webapp which shows the results of the voting in real time

![Voting-app-architecture](https://user-images.githubusercontent.com/62344505/98979367-92aba800-251b-11eb-91a4-30e587ee7f2c.png)

## Voting interface
----
![interface vote](https://user-images.githubusercontent.com/62344505/98979777-0ea5f000-251c-11eb-89b8-8d9d00a7145a.PNG)

## Result interface
----
![interface resultat1](https://user-images.githubusercontent.com/62344505/98981416-339b6280-251e-11eb-9563-dafbe64d857e.PNG)

## Getting started
Download and install Docker Desktop for Mac or Windows. Docker Compose will be automatically installed. On Linux, install Docker and docker compose.

## Run the application
If you're using Docker Desktop on Windows, you can run the Linux version by switching to Linux containers

Run in this directory:
```bash
docker-compose up
```
The app will be running at http://localhost:5050 

and the results will be at http://localhost:5051

You can see a video explicative for this application by visit the following link:

https://youtu.be/cAIVa2CSpxs