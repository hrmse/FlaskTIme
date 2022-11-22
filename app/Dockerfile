FROM python:alpine3.16
LABEL maintainer="HamidSoftDev@Gmail.com"
WORKDIR /app
COPY . .
RUN pip3 install -r requirements.txt
RUN apk add python3-flask
CMD flask run