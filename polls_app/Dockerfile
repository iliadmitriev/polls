FROM python

COPY requirements.txt /tmp

RUN mkdir /polls_app \
    && pip install -r /tmp/requirements.txt 

WORKDIR /polls_app

COPY . /polls_app

EXPOSE 8000

CMD python manage.py runserver 0:8000
