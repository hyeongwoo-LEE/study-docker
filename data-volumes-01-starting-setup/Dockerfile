FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

ARG DEFAULT_PORT=81

ENV PORT $DEFAULT_PORT

EXPOSE $PORT

# 익명 볼륨 경로 지정
# VOLUME [ "/app/feedback" ]

# 명명된 볼륨 생성은 컨테이너 실행할 때 생성
# docker run -d -p {local port}:{docker port} --rm --name {container name 지정} -v {volume name}:{volume path} {image name}:{tag}

CMD ["node", "server.js"]

