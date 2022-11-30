# start by pulling the python image
FROM python:3.10-alpine



# switch working directory
WORKDIR /app


# copy the requirements file into the image

COPY . .

# install the dependencies and packages fro local
RUN python3 -m pip install flask
#RUN pip3 install -r requirements.txt

CMD python3 app.py
