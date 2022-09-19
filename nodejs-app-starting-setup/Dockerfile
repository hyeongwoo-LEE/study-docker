# 노드 이미지 구축
FROM node

# 앞으로 명령어는 /app 에서 실행
WORKDIR /app

# 첫번째 . - 복사 폴더 경로, 두번째 . - 저장 폴더 경로
# Dockerfile과 동일한 폴더에 있는 모든 파일과 하위 폴더가 컨테이너 내부의 app 폴더에 복사됨. 
COPY . ./

RUN npm install

# 컨테이너의 포트만 열어둔 상태이기 때문에 로컬 머신에도 특정 포트 열어둠.
EXPOSE 81

# CMD : 이미지가 생성될 때 실행되지 않고 이미지를 기반으로 컨테이너가 시작될 때 실행됨.
CMD ["node", "server.js"]