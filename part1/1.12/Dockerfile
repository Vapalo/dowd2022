FROM node:lts-alpine

EXPOSE 5000

RUN apk add --no-cache git 

RUN git clone https://github.com/docker-hy/material-applications.git /apps

WORKDIR /apps/example-frontend

RUN npm install && npm install -g serve && REACT_APP_BACKEND_URL=http://localhost:8080 npm run build

CMD ["serve", "-s", "-l", "5000", "build"]
