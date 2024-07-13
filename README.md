# Exam
## Question 1
```
Dockerize a Wordpress application. Write a docker-compose.yml file to deploy wordpress applications using docker.
Download link for wordpress: https://wordpress.org/download/
```
Docker-compose file is created and kept in Question1 folder which will pull the wordpress docker and mySQL docker.

For making Wordpress running follow the command:
```shell
git clone https://github.com/Sukhilnair/Exam.git
cd Exam/Question1/
sudo docker-compose up -d
```
## Question 2
```
Create an architecture design for streaming application whose code is given below. Make sure the application scales from 0 to 100 million requests.
Link for the project: https://github.com/UnpredictablePrashant/StreamingApp
```
![Example Usage](./Question2/StreamingApp.drawio.png)

To create Docker containers for both the frontend and backend of the streaming application, Dockerfile, Docker Compose, and a shell script have been prepared. To build and run the Docker containers for the frontend and backend, execute the following command.

```shell
git clone https://github.com/Sukhilnair/Exam.git
cd Exam/Question2/
git clone https://github.com/UnpredictablePrashant/StreamingApp
cp Dockerfile_frontend ./StreamingApp/frontend/Dockerfile
cp start.sh ./StreamingApp/frontend
cp Dockerfile_authService ./StreamingApp/backend/authService/Dockerfile
cp Dockerfile_streamingService ./StreamingApp/backend/streamingService/Dockerfile
cp docker-compose.yml ./StreamingApp/
cd ./StreamingApp/
sudo docker-compose up -d
```