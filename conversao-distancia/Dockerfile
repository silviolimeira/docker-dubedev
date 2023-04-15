FROM python:3.9.10-alpine3.14
WORKDIR /srv
RUN pip install --upgrade pip
RUN pip install flask
COPY . /srv
ENV FLASK_APP=app
CMD ["python","app.py"]

# docker build -t sicemal/conversao-distancia:v1 .

# push no docker hub
# $ docker push sicemal/conversao-distancia:v1

# $ docker tag sicemal/conversao-distancia:v1 sicemal/conversao-distancia:latest

# push latest image to docker hub
# $ docker push sicemal/conversao-distancia:latest


# Executando e testando a imagem que foi construída
# $ docker container run -d -p 8080:8080 sicemal/conversao-temperatura:v1
