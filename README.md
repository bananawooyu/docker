# docker
# sk_shieldus 데이터 보안 전문가 교육과정 내용


### 도커 기본 명령어

sudo docker ps <br>
sudo docker ps -a

sudo docker images

sudo docker start [container ID or NAME] <br>
sudo docker stop <br>
sudo docker restart

sudo docker search [image NAME] <br>
sudo docker pull <br>
sudo docker push <br>
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] image:tag <br>
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] -v [volume NAME or static directory:/docker directory] image:tag

sudo docker volume create <br>
sudo docker volume ls

sudo docker build -t image:tag

### 도커 네트워크 브릿지IP 설정 <br>
/etc/docker <br>
vi daemon.json <br>
{"bip":"172.17.0.1/16"}


### 도커 네트워크 생성 <br>
sudo docker network create [net-NAME] <br>
sudo docker network ls

### 도커 로드밸런싱(nginx) <br>
/etc/nginx <br>
vi nginx.conf


