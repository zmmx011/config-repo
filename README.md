# config-repo
Config, Docker Compose Repository

## Config Server Repository
Spring Boot 기반 어플리케이션의 설정파일을 보관하며, 설정파일 변경 시 웹훅으로 http://100.100.10.174:8888/monitor API를 호출하여 Config Server에게 업데이트가 있음을 알립니다.

## Portainer Stack Repository
포테이너의 스택은 이 레포지토리를 참조하여 docker-compose 파일을 불러옵니다.

## Docker Package
포테이너에서 사용하는 도커이미지 중 재 빌드가 필요하지만, 별도의 레포지토리를 갖고 있지 않은 Nginx 등의 이미지는 이 레포지토리에서 빌드하여 배포됩니다.
