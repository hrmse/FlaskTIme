FROM python:alpine3.16
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
COPY . .

RUN pip3 install -r requirements.txt
RUN apk add python3-flask

CMD flask run