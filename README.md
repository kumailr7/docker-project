# Containerizing a Slack Clone App Built with the MERN Stack




## Prerequisite

- MongoDB
- Express
- React.js
- Node
- Docker Desktop


## Getting Started



## Cloning the repository


```
 git clone https://github.com/dockersamples/slack-clone-docker
```

## Building the Service containers

Write the Dockefile For all the services 
- Backend (Node)
- Frontend (Node/Reactjs)
- Database (MongoDB)

- Create the Backend Dockerfile in the Server Directory
- Create the mongoDB Dockerfile in the MongoDB Directory OR mention it in the Docker Compose file
- Then Create a Docker Compose File to Build the containers from the images and run them 


![image](https://user-images.githubusercontent.com/313480/193378996-14ce3feb-5087-4e14-b07d-a350e6eb133c.png)


```
 docker compose ps
               Name                             Command               State            Ports        -----------------------------------------------------------------------------
docker_db_1              docker-entrypoint.sh mongod      Up      0.0.0.0:27017->27017/tcp
docker_nodebackend_1     docker-entrypoint.sh node  ...   Up      0.0.0.0:9000->9000/tcp 
docker_slackfrontend_1   docker-entrypoint.sh yarn  ...   Up 
```






