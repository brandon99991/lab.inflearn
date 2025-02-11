▣ ■ ●

■ docker 빌드 및 실행

1) 빌드 (Dockerbuild 파일이 위치한 곳에서 빌드)
```
  $ sudo docker build -t brandon9999/hellodocker:latest ./
```

2) Docker image 조회
```
  $ sudo docker images
  $ sudo docker images ls
```

3) 실행
```
  $ docker run -it brandon9999/hellodocker:latest
```

4) 컨테이너 조회 (-a 옵션은 실행중이지 않은 컨테이너도 조회함)
```
  $ docker ps -a  
  ---------------------------------------------------------------
CONTAINER ID   IMAGE                        COMMAND                  CREATED         STATUS                      PORTS                                                                                      NAMES
f09c69857a37   brandon9999/hellodocker      "echo hello3"            2 minutes ago   Exited (0) 2 minutes ago
...<생략>...
  ---------------------------------------------------------------
```

5) docker 이미지 push (도커허브에 push)
```
  $ docker push brandon9999/hellodocker:latest
```

6) 실행
```
  $ docker run -it brandon9999/hellodocker:latest
```
