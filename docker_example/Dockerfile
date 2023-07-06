FROM linuxserver/blender:latest

# RUN python3 -V

RUN apt update
RUN apt install git python3-pip -y

COPY requirements.txt .
RUN python3 -m pip install -r requirements.txt

USER abc

COPY requirements.txt .
RUN python3 -m pip install -r requirements.txt

USER root
