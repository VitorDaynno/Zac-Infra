FROM ubuntu:18.04

RUN apt-get update 
RUN apt-get install git -y
RUN apt install python3 -y && apt-get -y install python3-pip

WORKDIR /app

RUN git clone https://github.com/VitorDaynno/Zac.git /app && \
    cd /app && \
    chmod +x requirements.sh && \
    ./requirements.sh && \
    chmod +x start.sh

CMD ["/app/start.sh"]