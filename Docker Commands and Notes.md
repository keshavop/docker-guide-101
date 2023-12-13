## Docker Commands and Notes

### Commands
```docker ps```
- to see all the images and their status

```docker kill {conatiner name}```
- to stop any container

```docker build . -t test-app```
- here -t is the tag name or id you can say

```docker images```
- to view all the images present in os

```docker run {container name}```
- to run that container

```docker run -p 3000:3000 {image-tag}```
- run the app and map 3000 port of os to 3000 port of container and run it



### Notes

#### dockerfile code explanation
![Screenshot from 2023-12-12 18-12-27](https://github.com/keshavop/docker-guide-101/assets/71931145/0fba4357-27be-4aea-8631-19d7035a800f)

FROM  ->Base image that you want to use

WORKDIR  ->the dir where you want to use to run the app

COPY ..  -> copy *everything* all the files from your project to container

RUN  -> the command to install packages

EXPOSE  -> the port which you want to expose or run at that port

CMD  -> this run when you want to start container
        For ex```CMD["node","index.js"]```


## > Create Volume to persist data in database
