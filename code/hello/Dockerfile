# Pull base image
FROM python:3.7

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set work directory
WORKDIR /codeChapter 1: Docker

# Install dependencies
COPY Pipfile Pipfile.lock /code/
RUN pip3 install --upgrade pip
RUN pip3 install pipenv

# COPY Pipfile* /app/
RUN cd /code && pipenv install --system


# Copy project
COPY . /code/