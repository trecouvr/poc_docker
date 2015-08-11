from python:3.4

ENV PYTHONUNBUFFERED 1
RUN useradd -ms /bin/bash nemopay
RUN mkdir /webapp
WORKDIR /webapp
ADD . /webapp/
RUN pip install -r requirements.txt

RUN chown -R nemopay:nemopay /webapp
USER nemopay

EXPOSE 8000
