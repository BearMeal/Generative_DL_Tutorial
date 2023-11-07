## How to use Docker
-간단 설명 https://github.com/davidADSP/Generative_Deep_Learning_2nd_Edition/blob/main/docs/docker.md

- 패키지 사용에 있어 가상환경을 사용해서 맞추어 줬다면 도커는 일관된 OS,환경과 패키지 둘다 맞춰 줄수있다. 케이크 조각(컨테이너 안에서의 이미지를) 나누듯 효율적인 자원분배및 환경 사용이 가능하다.
- 만들어진 도커환경(=도커 이미지) .env 파일에 원하는 포트값과 캐글 api를
mapping 해준다.
터미널에 docker compose build 커맨드를 입력하여 빌드한다. 그러면 컨테이너 환경기반의 이미지가 만들어진 것이다.
- => build 시간이 너무 오래걸린다 어떻게 해결할 수 있을까
- docker images 커맨드를 입력하면 만들어진 이미지들을 확인 할수있다.
- docker rmi imageID 를 입력하면 이미지 삭제가능
- docker compose up 커맨드를 입력하면 도커에서 실행하는 주피터노트북 서버를 볼수있다 http://localhost:8888/lab (ctrl+c 하면 중지)
-자 이제 notebooks안의.ipynb 파일을 실행해도 환경문제없이 실행가능하다
- docker compose down 하면 컨테이너 중지

- docker ps:실행중인 도커 컨테이너확인

