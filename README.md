# Log Server Test Project

## Run application (development approach):
<img alt="docker" src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white"/>

### 1. Clone project repository.
### 2. Make sure you have docker and java(version 10 and later) installed.
#### * On Windows OS make sure that docker engine has started.
### 3. From the root directory of the project with root privileges run:
a.
```bash
$ docker-compose up -d
```
### 4. After that you can send the POST request with JSON info to <i>http://localhost:8090/api/v1/events</i>.
#### * For this action you can use postman
#### * JSON: {"message":"your message", "level":"level", "type":"type", "time":"0123456789"}
## Stop database and logserver:
### To stop database and remove the container run:
```bash
$ docker compose down
```
## Notice: 
####  Logserver working on port 80 in the docker container and access on port 8090 on the host machine. 
####  If you want to start logserver on other port you must change the parameter PORTS in the section LOGSERVER in the docker-compose.yml file.
