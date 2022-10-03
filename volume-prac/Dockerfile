FROM node:12

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

# anonymous volume 은 특정 컨테이너의 라이프사이클과 같은 라이프사이클을 가진다.
# VOLUME [ "/app/feedback" ]  # 컨테이너 내부의 특정 경로 -> anonymous VOLUME

CMD ["node", "server.js"]

