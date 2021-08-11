FROM python:3.9-buster

ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt /requirements.txt
    
RUN pip install --upgrade pip

RUN pip install -r /requirements.txt


RUN mkdir backend-repo
COPY . /backend-repo
RUN chmod 777 /backend-repo
WORKDIR /backend-repo
RUN chmod 777 /backend-repo
# Run the application:
# CMD python manage.py runserver 0.0.0.0:8000
