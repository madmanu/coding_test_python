FROM python:3
ENV PYTHONUNBUFFERED 1

RUN mkdir /opt/lst
ENV PYTHONPATH /opt/lst:$PYTHONPATH
WORKDIR /opt/lst

ADD requirements.txt /opt/lst/
RUN pip install -r requirements.txt

ADD . /opt/lst
RUN python manage.py migrate

ENTRYPOINT ["python","manage.py"]
CMD ["runserver", "0.0.0.0:5678"]
