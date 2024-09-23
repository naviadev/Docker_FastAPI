# Docker_FastAPI

ML 기반 관상 분석 팀 프로젝트에 앞서, FastAPI 학습과 Docker 실습을 진행해보기 위한 레포지토리

# 명령어 정리

## Server

> python -m venv env // 가상환경 추가

> source env/bin/activate // 가상환경 활성화

> uvicorn app.main:app --reload //서버 실행

## Docker

> docker run -d --name server -p 8000:8000 server //서버 실행 - Docker

> docker ps // 실행중인 docker 컨테이너 확인

> docker stop server // 서버 닫기.

> docker images // Docker 이미지 확인

> docker rmi server // Docker 이미지 삭제

> docker system df // Docker 시스템 사용량 체크
