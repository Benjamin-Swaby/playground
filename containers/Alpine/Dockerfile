from alpine

#add edge testing branch
RUN echo "https://dl-cdn.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories

RUN apk update

#very important
RUN apk add bash 
RUN apk add neofetch fish

WORKDIR /