FROM node

RUN apt-get update

WORKDIR /app

RUN git clone https://github.com/VitorDaynno/zac-dashboard /app && \
    npm install

RUN npm run build

FROM nginx:1.15-alpine

COPY --from=0 /app/build /usr/share/nginx/html