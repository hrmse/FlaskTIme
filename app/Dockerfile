# start by pulling the python image
FROM python:alpine3.16


# switch working directory
WORKDIR /app


# copy the requirements file into the image

COPY . .

# install the dependencies and packages 
RUN python3 -m pip install Flask==2.2.2



#RUN pip3 install -r requirements.txt

CMD python3 app.py
