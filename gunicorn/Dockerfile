FROM python:3.7

RUN git clone https://github.com/shutlle/dash
RUN pip3 install -r dash/requirements.txt gunicorn


RUN django-admin startproject project
RUN cp -R dash/* project
RUN rm -rf dash
RUN rm -rf project/.git

WORKDIR project


