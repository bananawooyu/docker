# docker
# sk_shieldus 데이터 보안 전문가 교육과정 내용


### 도커 기본 명령어

#### 도커 프로세스 확인
sudo docker ps <br>
sudo docker ps -a <br>

#### 도커 이미지 확인
sudo docker images <br>

#### 도커 컨테이너 시작, 정지 , 재시작
sudo docker start [container ID or NAME] <br>
sudo docker pause [container ID or NAME] <br>
sudo docker stop [container ID or NAME] <br>
sudo docker restart [container ID or NAME] <br>
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] image:tag <br>
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] -v [volume NAME or static directory:/docker directory] image:tag <br>

#### 도커 이미지 검색, 다운로드, 업로드
sudo docker search [image NAME] <br>
sudo docker pull [image NAME] <br>
sudo docker push [image NAME] <br>
sudo docker login <br>

#### 도커 볼륨 생성, 리스트
sudo docker volume create <br>
sudo docker volume ls <br>

#### 도커 이미지 삭제, 컨테이너 삭제
sudo docker rmi [image ID] <br>
sudo docker rm [container ID or NAME] <br>
sudo docker rm $(sudo docker ps -aq) <br>
sudo docker rm $(sudo docker ps -q status:exited) <br>

#### 도커 네트워크 브릿지IP 설정
/etc/docker <br>
vi daemon.json <br>
{"bip":"172.17.0.1/16"} <br>

#### 도커 컨테이너 쉘 접속
sudo docker exec -it [docker PS NAME] <br>

#### 도커 네트워크 생성 <br>
sudo docker network create [net-NAME] <br>
sudo docker network ls <br>

#### 도커 로드밸런싱(nginx)
/etc/nginx <br>
vi nginx.conf <br>

#### 도커 파일
sudo docker build -t image:tag <br>
sudo docker run -dit --name=[NAME] -p [host PORT]:[docker PORT] image:tag <br>

#### 도커 컴포즈
sudo apt install docker-compose <br>
sudo vi docker-compose.yaml [-d , --build]<br>
sudo docker-compose up <br>
sudo docker-compose down <br>
sudo docker-compose ps <br>
sudo docker-compose pause <br>
sudo docker-compose unpause <br>
