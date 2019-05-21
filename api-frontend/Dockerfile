FROM debian:jessie

ADD api.py /

RUN apt-get update \
        && apt-get upgrade \
        && apt-get install -y \
                python-requests python-flask
ENV API_BACKEND_URL backend
ENV API_BACKEND_PORT 8001
#RUN pip install requests flask

CMD [ "python", "./api.py" ]
