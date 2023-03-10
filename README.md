#service discovery
javabeanstack/light-weight-app-discovery:v1 



#deploy docker stack
docker stack deploy --compose-file docker-stack.yml light-weight-app

#create light-weight-app netwrok as attachable
docker network create light-weight-app --driver overlay --attachable

#swarm-local-host on my HP-Linux
192.168.0.139

#swarm-local-host on my Dell-Windows
192.168.65.4

#Eureka discovery service
http://<local-host>:8761/

