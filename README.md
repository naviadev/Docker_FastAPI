# Docker_FastAPI

ML 기반 관상 분석 팀 프로젝트에 앞서, FastAPI 학습과 Docker 실습을 진행해보기 위한 레포지토리

# 명령어 정리

## Server

> python -m venv env // 가상환경 추가

> source env/bin/activate // 가상환경 활성화

> uvicorn app.main:app --reload //서버 실행

> deactivate // 가상환경 종료

## Docker

- Docker 이름은 server로 지정해두었다.

### Docker 컨테이너 실행

> docker run -d --name server -p 8000:8000 server

### 실행중인 Docker Container 확인

> docker ps

### Docker 종료

> docker stop server

### Docker 이미지 목록 확인

> docker images

### Docker 이미지 삭제 (지정)

> docker rmi server

### Docker 모든 이미지 삭제

> docker rmi $(docker images -q)

### Docker 종료된 모든 컨테이너 삭제

> docker rm $(docker ps -a -q)

### Docker 시스템 사용량 체크

> docker system df
