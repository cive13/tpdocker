FROM debian:jessie

ADD api.py /
LABEL "hub_url"="https://cloud.docker.com/repository/docker/anbfree/frontend"
RUN apt-get update \
        && apt-get upgrade \
        && apt-get install -y \
                python-requests python-flask
ENV API_BACKEND_URL backend
ENV API_BACKEND_PORT 8001
#RUN pip install requests flask

CMD [ "python", "./api.py" ]
