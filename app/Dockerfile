# pull official base image
FROM python:3.11-rc-slim

# set work directory
WORKDIR /usr/src/app

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# install dependencies
RUN pip install --upgrade pip
COPY ./requirements .
RUN pip install -r dev.txt

# copy project
COPY . .