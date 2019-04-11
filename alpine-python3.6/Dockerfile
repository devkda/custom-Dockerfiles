
# Base_image arguments are mandatory
ARG base_image=python:3.6.8-alpine3.8

# Dependecies build stage
FROM ${base_image}

RUN apk update
RUN apk add --no-cache --virtual .build-deps gcc musl-dev make gfortran build-base wget freetype-dev libpng-dev openblas-dev 
RUN pip install cython 

ENV PYTHONUNBUFFERED 1
