FROM python:3.10 as build-dep

ENV APP_NAME=mongo_exemple.env
COPY ${APP_NAME} .

COPY requirements.txt .

RUN mkdir /install
RUN pip3 install --upgrade pip \
    && pip3 install -r requirements.txt

CMD ["python3", "src/main.py"]

