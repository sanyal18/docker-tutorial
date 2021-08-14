FROM ubuntu:latest

RUN mkdir /server

COPY script.sh /server/

RUN  apt update

RUN  apt install software-properties-common -y

RUN  add-apt-repository ppa:deadsnakes/ppa 

RUN  apt update

RUN  apt install python3.8 && python3 --version

RUN cd /server

RUN apt-get install redis-tools -y

CMD python3 -m http.server 3000
  
