FROM python:3.7
RUN apt-get update && apt-get install -y build-essential cmake git libboost-all-dev libgtk-3-dev

COPY ./app /app


RUN pip install -r /app/requirements.txt
WORKDIR /app
EXPOSE 8501

