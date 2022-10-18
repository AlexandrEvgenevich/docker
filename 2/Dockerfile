FROM python:3.9

RUN mkdir /app

COPY requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip3 install -r requirements.txt

COPY . /app

EXPOSE 2222

ENTRYPOINT [ "python", "manage.py" ]

CMD [ "runserver", "0.0.0.0:2222" ]