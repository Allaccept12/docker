## 컨테이너 실행
docker run [OPTIONS] IMAGE[:TAG|@DIGEST] [COMMAND] [ARG...]
- -d -> detached mode (백그라운드 모드)
- -p 호스트와 컨테이너의 포트를 연결
- -v 호스트와 컨테이너의 디렉토리를 연결
- -e 컨테이너 내에서 사용할 환경변수 설정
- --name 컨테이너 이름 설정
- --rm 프로세스 종료시 컨테이너 자동 제거
- -it -i와 -t를 동시에 사용한 것으로 터미널 입력을 위한 옵션
- --network 네트워크 연결

 

## ps 명령어

docker ps -> 실행중인 컨테이너 목록을 확인하는 명령어 입니다
docker ps -a  -> 중지된 컨테이너도 확인하려면 -a 옵션을 붙입니다

## stop 명령어
docker stop [OPTIONS] CONTAINER [CONTAINER...]
- 실행중인 컨테이너를 중지하는 명령어 입니다.
- 실행중인 컨테이너를 하나 또는 여러개 (띄어쓰기) 중지할 수 있습니다

## rm 명령어
docker rm [OPTIONS] CONTAINER [CONTAINER...]
- 종료된 컨테이너를 완전히 제거하는 명령어 입니다

## logs 명령어
docker logs [OPTIONS] CONTAINER
- 컨테이너가 정상적으로 동작하는지 확인하는 좋은 방법은 로그를 확인하는 것 입니다. 기본 옵션과 -f, --tail 옵션을 살펴보니다
