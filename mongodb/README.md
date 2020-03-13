```
Mithuns-Air:mongodb mithunkhatri$ cat docker-compose.yml 
version: '3.1'
services:
  mongodb:
    image: mongo
    ports:
      - 27017:27017
Mithuns-Air:mongodb mithunkhatri$ docker-compose up -d
Creating network "mongodb_default" with the default driver
Pulling mongodb (mongo:)...
latest: Pulling from library/mongo
423ae2b273f4: Pull complete
de83a2304fa1: Pull complete
f9a83bce3af0: Pull complete
b6b53be908de: Pull complete
f3cc2fb4f0eb: Pull complete
f552d845039c: Pull complete
ba6e166a9814: Pull complete
dc2ba5bee263: Pull complete
828a1244f976: Pull complete
c63a86989a84: Pull complete
ebc2ee27e8bb: Pull complete
89a06e64657c: Pull complete
1ca7a5924304: Pull complete
Digest: sha256:a1f116a08f48359302d7b567bdccc8b047bb0e534044de91be908c39eb796707
Status: Downloaded newer image for mongo:latest
Creating mongodb_mongodb_1 ... done
Mithuns-Air:mongodb mithunkhatri$ docker ps
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS                      NAMES
704311d7d3b3        mongo               "docker-entrypoint.s…"   4 seconds ago       Up 3 seconds        0.0.0.0:27017->27017/tcp   mongodb_mongodb_1
Mithuns-Air:mongodb mithunkhatri$
```
