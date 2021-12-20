```  
  115  docker network ls 
  116  docker network inspect ec650ccca946
  117  docker network create --driver=bridge --subnet=172.28.0.0/16 --ip-range=172.28.5.1/24 --gateway=172.28.5.254 mybr0
  118  docker network ls 
  119  ls
  120  docker inspect mybr0
  121  docker run -d --name test-apache-10 --network "mybr0" -P myapache-app:v1 
  122  docker run -d --name test-apache-11 --network "mybr0" -P myapache-app:v1 
  123  docker ps 
  124  docker inspect test-apache-11
  125  docker inspect test-apache-10
  126  docker run -d --name test-apache-13 --network "mybr0" -P myapache-app:v1 
  127  docker inspect test-apache-13
  128  ip addr 
  129  docker kill $(docker ps -qa ) 
  130  docker rm $(docker ps -qa ) 
  131  docker network ls 
  132  docker network inspect bridge
  133  docker network inspect mybr0
  134  docker run -d --name test-apache-1 --network "mybr0" -P myapache-app:v1 
  135  docker network inspect mybr0
  136  docker run -d --name test-apache-2 --network "mybr0" -P myapache-app:v1 
  137  docker run -d --name test-apache-3 --network "mybr0" -P myapache-app:v1 
  138  docker network inspect mybr0
  139  ls
  140  docker network ls 
  141  docker rm $(docker ps -qa ) 
  142  docker kill $(docker ps -qa ) 
  143  docker rm $(docker ps -qa ) 
  144  docker network rm mybr0
  145  docker network ls 
  146  docker ps 
  147  docker run -itd --name test-1 ubuntu:16.04 
  148  docker ps 
  149  docker exec -it test-1 ip addr 
  150  docker exec -it test-1 hostname -i 
  151  docker run -itd --name test-2 ubuntu:16.04 
  152  docker exec -it test-2 hostname -i 
  153  docker network ls 
  154  docker run -itd --name test-none-1 --network none ubuntu:16.04
  155  docker ps 
  156  docker exec -it test-none-1 hostname -i 
  157  docker inspect test-2
  158  docker ps 
  159  docker inspect  test-none-1
  160  docker run -itd --name test-host-1 --network host ubuntu:16.04
  161  docker ps 
  162  docker exec -it test-host-1 hostname -i 
  163  docker inspect test-host-1
  164  docker exec -it test-host-1 hostname -i 
  165  docker run -d --name test-apache-3  -P myapache-app:v1 
  166  docker ps 
  167  netstat -tulnp 
  168  systemctl status docker 
  169  docker run -d --name test-apache-4 --network none   -P myapache-app:v1 
  170  docker ps 
  171  docker run -d --name test-apache-5 --network host  -P myapache-app:v1 
  172  docker ps 
  173  netstat -tulnp 
  174  which apache2 
  175  curl localhost
  176  ls
  177  cd docker-kubernetes-ericsson-20-Dec-2021/
  178  ls
  179  cd 01-Docker/
  180  ls
  181  mkdir 03-DockerNetwork
  182  ls
  183  history > 03-DockerNetwork/README.md
```
