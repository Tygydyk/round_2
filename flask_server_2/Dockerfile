FROM python:3
WORKDIR /task
COPY . /task
RUN apt update && apt install -y python3-pip && pip3 install flask
CMD python3 ./test.py
EXPOSE 55536/tcp
