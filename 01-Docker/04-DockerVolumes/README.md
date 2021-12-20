    1  ls
    2  cd 01-Docker/
    3  ls
    4  mkdir 04-DockerVolumes 
    5  ls
    6  cd 04-DockerVolumes/
    7  ls
    8  cd 
    9  docker volume ls 
   10  docker volume create my-vol 
   11  docker volume ls 
   12  docker volume inspect my-vol
   13  docker run -it --name volume-test-1 -v my-vol:/var/www/html/app ubuntu:16.04
   14  docker ps 
   15  docker kill $(docker ps -aq) 
   16  docker rm $(docker ps -aq) 
   17  docker ps 
   18  docker volume ls 
   19  docker volume inspect my-vol
   20  cd /var/lib/docker/volumes/my-vol/_data/
   21  ls
   22  cat hello.txt 
   23  cd 
   24  ls
   25  docker run -it --name volume-test-1 -v my-vol:/var/www/html/app ubuntu:16.04
   26  docker ps 
   27  docker run -it --name volume-test-2 -v my-vol:/app ubuntu:16.04
   28  docker ps 
   29  docker run -it --name volume-test-3 -v my-vol:/app:ro ubuntu:16.04
   30  docker ps 
   31  docker run -it --name volume-test-4 -v /var/www/amit ubuntu:16.04
   32  docker ps 
   33  docker volume ls 
   34  docker kill $(docker ps -qa ) 
   35  docker rm $(docker ps -qa )
   36  docker volume ls 
   37  docker volume rm my-vol 
   38  docker volume ls 
   39  docker volume rm 3dff731c936d9d73fee4ca549884f8b4a3e148bfcc145173a26d8cb6fc2c5983
   40  ls
   41  cd docker-kubernetes-ericsson-20-Dec-2021/
   42  ls
   43  cd 01-Docker/
   44  ls
   45  cd 04-DockerVolumes/
   46  ls
   47  history > README.md 
