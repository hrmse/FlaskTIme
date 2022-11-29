# start by pulling the python image
FROM python:3.8-alpine

RUN addgroup app && adduser -S -G app app
USER app

# switch working directory
WORKDIR /app


# copy the requirements file into the image

COPY . .

# install the dependencies and packages fro local
RUN python3 -m pip install -r wheelhouse/requirements.txt --no-index --find-links wheelhouse

#RUN pip3 install -r requirements.txt

CMD python3 app.py
