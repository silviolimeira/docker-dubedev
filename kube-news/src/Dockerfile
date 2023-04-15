# node 16
FROM node:18.11.0
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . . 
EXPOSE 8080
CMD ["node", "server.js"]

# Criando a imagem:
# $ docker build -t sicemal/kube-news:v1 .

# dentro da pasta /src, onde está o Dockerfile este imagem será montada e 
# enviada para o Docker hub.

#Verificando:
# $ docker image ls

# Subir a imagem para o docker
# $ docker push sicemal/kube-news:v1

# Talvez tenha que logar com docker login

# Também é importante subir a última versão mesmo sendo a última
# $ docker tag sicemal/kube-news:v1 sicemal/kube-news:latest

# Verificando:
# $ docker image ls

# Colocando a última versão do Docker hub, também:
# $ docker push sicemal/kube-news:latest





