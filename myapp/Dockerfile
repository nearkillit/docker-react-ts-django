#1
FROM node:14-alpine
#2
WORKDIR /app
#3
COPY package.json .
COPY package-lock.json .
#4
RUN npm install
#5
COPY . .
#6
EXPOSE 3000
#7
ENV CHOKIDAR_USEPOLLING=true
#8
CMD [ "npm", "start" ]