#service discovery
javabeanstack/light-weight-app-discovery:v1 



#deploy docker stack
docker stack deploy --compose-file docker-stack.yml light-weight-app

#create light-weight-app netwrok as attachable
docker network create light-weight-app --driver overlay --attachable

#swarm-local-host 
run this on leader manager node:  docker swarm join-token manager
use the ip address specified by this leader manager join-toke as the <local-host> 
#Eureka discovery service
http://<local-host>:8761/

