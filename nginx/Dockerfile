FROM nginx:1

LABEL author "Andrê Reges <andre.reges@aluno.faculdadeimpacta.com.br>"
LABEL maintainer "Andrê Reges <andre.reges@aluno.faculdadeimpacta.com.br>"

USER root
WORKDIR /var/www/html

RUN apt-get update \
    && apt-get install -y \
    nano \
    iputils-ping

RUN apt-get clean && rm -rf /var/lib/apt/lists/* && apt-get clean

CMD nginx -g "daemon off;"

EXPOSE 80 443