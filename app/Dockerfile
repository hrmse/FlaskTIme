FROM python:alpine3.16
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
RUN mkdir data
RUN python3-flask
COPY . .
CMD flask run