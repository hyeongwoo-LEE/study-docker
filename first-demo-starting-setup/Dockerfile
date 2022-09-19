
# nodeJS 사용
FROM node:14

# 컨테이너 파일 시스템 내 작업하고자 하는 디렉토리
WORKDIR /app

# package.json 파일을 작업 디렉토리에 복사
COPY package.json .

# npm install 실행
RUN npm install

# 나머지 코드 복사
COPY . .

EXPOSE 3000

# node 명령으로 app.mjs 실행
CMD ["node", "app.mjs"]