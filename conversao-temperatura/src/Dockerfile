# node 16
FROM node:18.13.0
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . . 
EXPOSE 8080
CMD ["node", "server.js"]

# docker build -t sicemal/conversao-temperatura:v1 .

# push no docker hub
# $ docker push sicemal/conversao-temperatura:v1

# $ docker tag sicemal/conversao-temperatura:v1 sicemal/conversao-temperatura:latest

# push latest image to docker hub
# $ docker push sicemal/conversao-temperatura:latest


# Executando e testando a imagem que foi construída
# $ docker container run -d -p 8080:8080 sicemal/conversao-temperatura:v1
