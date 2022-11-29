# start by pulling the python image
FROM python:3.8-alpine

RUN addgroup app && adduser -S -G app app
USER app

# switch working directory
WORKDIR /app


# copy the requirements file into the image

COPY . .

# install the dependencies and packages fro local

RUN python3 -m pip install /app/libs/Werkzeug-2.2.2.tar.gz
RUN python3 -m pip install /app/libs/MarkupSafe-2.1.1.tar.gz
RUN python3 -m pip install /app/libs/flask-2.2.2.tar.gz

RUN python3 -m pip install /app/libs/Jinja-1.2.tar.gz
RUN python3 -m pip install /app/libs/itsdangerous-2.1.2.tar.gz
RUN python3 -m pip install /app/libs/gunicorn-20.1.0.tar.gz
RUN python3 -m pip install /app/libs/colorama-0.4.6.tar.gz
RUN python3 -m pip install /app/libs/click-8.1.3.tar.gz


#RUN pip3 install -r requirements.txt

CMD python3 app.py
