```
Mithuns-Air:elastic-apm mithunkhatri$ docker-compose up -d
Creating network "elastic-apm_default" with the default driver
Pulling elasticsearch (docker.elastic.co/elasticsearch/elasticsearch:7.6.1)...
7.6.1: Pulling from elasticsearch/elasticsearch
c808caf183b6: Pull complete
ab639412b262: Pull complete
8b89a61469c0: Pull complete
641adcee3431: Pull complete
e15a8fd0cc25: Pull complete
5c323c45cbe2: Pull complete
895d2a8c37d1: Pull complete
Digest: sha256:d74a4d9aa241cc7fda110a38f1208869407f1242e93c733281452cd9831a0064
Status: Downloaded newer image for docker.elastic.co/elasticsearch/elasticsearch:7.6.1
Pulling kibana (docker.elastic.co/kibana/kibana:7.6.1)...
7.6.1: Pulling from kibana/kibana
c808caf183b6: Already exists
130450edbebb: Pull complete
b9257098c1b8: Pull complete
9e9c065b7541: Pull complete
7f503a6f5f82: Pull complete
cfc6ffea6a82: Pull complete
830a672de7c2: Pull complete
db57b75450e1: Pull complete
a12a92ac9cc5: Pull complete
fc88e9333435: Pull complete
Digest: sha256:15601a0c7fc739fabce9c5db9b14416c6226cf2de77506837e6a1162043dffe1
Status: Downloaded newer image for docker.elastic.co/kibana/kibana:7.6.1
Pulling apm-server (docker.elastic.co/apm/apm-server:7.6.1)...
7.6.1: Pulling from apm/apm-server
c808caf183b6: Already exists
55a0089f857f: Pull complete
d5a787fae115: Pull complete
5963b6436949: Pull complete
42d54d37be46: Pull complete
35c5c8353980: Pull complete
a142f93323f6: Pull complete
Digest: sha256:93ade5943e58a0ae3f79dbc20dce9a2381b0669a5a10bcbd65e2dcd6ac8bd555
Status: Downloaded newer image for docker.elastic.co/apm/apm-server:7.6.1
Creating elastic-apm_elasticsearch_1 ... done
Creating elastic-apm_apm-server_1    ... done
Creating elastic-apm_kibana_1        ... done
Mithuns-Air:elastic-apm mithunkhatri$ docker ps
CONTAINER ID        IMAGE                                                 COMMAND                  CREATED             STATUS              PORTS                              NAMES
74d8d51934a8        docker.elastic.co/kibana/kibana:7.6.1                 "/usr/local/bin/dumb…"   6 seconds ago       Up 4 seconds        0.0.0.0:5601->5601/tcp             elastic-apm_kibana_1
002fbe6781dc        docker.elastic.co/apm/apm-server:7.6.1                "/usr/local/bin/dock…"   6 seconds ago       Up 4 seconds        0.0.0.0:8200->8200/tcp             elastic-apm_apm-server_1
bbaa141635f1        docker.elastic.co/elasticsearch/elasticsearch:7.6.1   "/usr/local/bin/dock…"   7 seconds ago       Up 6 seconds        0.0.0.0:9200->9200/tcp, 9300/tcp   elastic-apm_elasticsearch_1
Mithuns-Air:elastic-apm mithunkhatri$
```
