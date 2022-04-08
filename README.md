# docker
sk_shieldus 데이터 보안 전문가 교육과정 내용


도커 기본 명령어

sudo docker ps\n
sudo docker ps -a\n

sudo docker images

sudo docker start [container ID or NAME]
sudo docker stop
sudo docker restart

sudo docker search [image NAME]
sudo docker pull
sudo docker push
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] image:tag
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] -v [volume NAME or static directory:/docker directory] image:tag

sudo docker volume create
sudo docker volume ls

sudo docker build -t image:tag

도커 네트워크 브릿지IP 설정
/etc/docker
vi daemon.json
{"bip":"172.17.0.1/16"}


도커 네트워크 생성
sudo docker network create [net-NAME]
sudo docker network ls

도커 로드밸런싱(nginx)
/etc/nginx
vi nginx.conf


