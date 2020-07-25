# Tutorial

## 1. Clone

`git clone https://github.com/docker/getting-started.git`

## 1.1 Rename

`mv getting-started docker-getting-started`

`cd docker-getting-started`

## 1.2 Add Repository

`git remote remove origin`

`git remote add origin git@github.com:c5apple/docker-getting-started.git`

`git push origin master`

## 2. Build

`docker build -t docker101tutorial .`

## 3. Run

### docker

`docker run -d -p 80:80 --name docker-tutorial docker101tutorial`

`docker ps -a`

`docker images`

http://localhost:80

### docker-compose

`docker-compose up`

`docker-compose ps`

http://localhost:8000

## 3.1 Stop

`docker stop {CONTAINER ID}`

`docker-compose stop`

## 3.2 Remove

`docker rm {CONTAINER ID}`

`docker rmi {IMAGE ID}`

`docker-compose down`

## 4. Share

https://hub.docker.com

`docker tag docker101tutorial {userName}/docker101tutorial`

`docker push {userName}/docker101tutorial`
