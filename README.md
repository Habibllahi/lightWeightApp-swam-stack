#service discovery
javabeanstack/light-weight-app-discovery:v1 



#deploy docker stack
docker stack deploy --compose-file docker-stack.yml light-weight-app

#create light-weight-app netwrok as attachable
docker network create light-weight-app --driver overlay --attachable

#Eureka discovery service
http://192.168.0.139:8761/
‣楬桧坴楥桧䅴灰猭慷⵭瑳捡੫