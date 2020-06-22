FROM alpine

COPY --from=library/docker:latest /usr/local/bin/docker /usr/bin/docker

FROM python:3.7
RUN apt-get update
RUN ln -s /usr/local/bin/docker /usr/bin/docker

COPY ./app /app
RUN pip install -r /app/requirements.txt

WORKDIR /app

