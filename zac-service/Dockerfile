FROM python

WORKDIR /app

RUN git clone https://github.com/VitorDaynno/zac-service /app && \
    cd /app

RUN pip install -r requirements.txt

CMD ["python", "main.py"]