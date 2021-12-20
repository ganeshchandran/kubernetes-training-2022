```
    1  ls
    2  git clone https://github.com/amitvashisttech/docker-kubernetes-ericsson-20-Dec-2021.git
    3  cd docker-kubernetes-ericsson-20-Dec-2021/
    4  ls
    5  cd 01-Docker/00-Setup/
    6  ls
    7  ./install-docker.sh 
    8  ls
    9  docker version 
   10  docker run ubuntu:16.04 echo "Hello World" 
   11  docker ps 
   12  cd 
   13  docker ps -a 
   14  docker run -it --name test-1 ubuntu:16.04 
   15  docker ps 
   16  docker ps -a 
   17  docker run --name test-2 ubuntu:16.04 echo "Hey Ubuntu" 
   18  docker run --name test-3 ubuntu:16.04 echo "Hey Ubuntu" 
   19  docker ps -a 
   20  docker start test-1
   21  docker ps 
   22  docker attach test-1
   23  docker ps 
   24  docker stop test-1
   25  docker ps 
   26  docker ps -a 
   27  docker ps 
   28  docker ps -a
   29  docker ps -aq
   30  docker kill $(docker ps -aq) 
   31  docker rm $(docker ps -aq) 
   32  docker ps -a 
   33  docker images 
   34  ls
   35  cd docker-kubernetes-ericsson-20-Dec-2021/
   36  ls
   37  cd 01-Docker/
   38  ls
   39  mkdir 01-Docker_Intro
   40  ls
   41  cd 01-Docker_Intro/
   42  ls
   43  history > README.md
   44  vim README.md 
   45  ls
   46  cd ..
   47  ls
   48  mkdir 02-Dockerfile/apache -p 
   49  cd 02-Dockerfile/apache/
   50  ls
   51  vim Dockerfile 
   52  ls
   53  vim index.html 
   54  ls
   55  docker build -t myapache-app:v1 . 
   56  ls
   57  docker images 
   58  ls
   59  cd 
   60  docker images 
   61  docker run -d --name test-apache-1 myapache-app:v1 
   62  docker ps 
   63  docker inspect test-apache-1
   64  curl "172.17.0.2"
   65  docker network ls 
   66  docker network inspect ec650ccca946
   67  ip addr 
   68  docker inspect test-apache-1
   69  docker run -d --name test-apache-2 myapache-app:v1 
   70  docker run -d --name test-apache-3 myapache-app:v1 
   71  docker ps 
   72  docker network inspect ec650ccca946
   73  docker ps 
   74  curl 172.17.0.2
   75  curl 172.17.0.3
   76  curl 172.17.0.4
   77  netstat -tulnp 
   78  ip addr 
   79  docker ps 
   80  docker run -d --name test-apache-4 -p 8080:80 myapache-app:v1 
   81  docker ps 
   82  netstat -tulnp 
   83  systemctl status docker 
   84  docker ps 
   85  docker inspect test-apache-4
   86  docker ps 
   87  docker run -d --name test-apache-5 -p 8080:80 myapache-app:v1 
   88  docker run -d --name test-apache-6 -p 8081:80 myapache-app:v1 
   89  docker ps 
   90  docker run -d --name test-apache-7 -P myapache-app:v1 
   91  docker ps 
   92  docker run -d --name test-apache-8 -P myapache-app:v1 
   93  docker run -d --name test-apache-9 -P myapache-app:v1 
   94  docker ps 
   95  ls
   96  cd docker-kubernetes-ericsson-20-Dec-2021/
   97  ls
   98  cd 01-Docker/
   99  ls
  100  cd 01-Docker_Intro/
  101  ls
  102  history > README.md 

```
