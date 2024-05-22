FROM alpine
# Alpine
RUN apk add py3-pip 

# Debian
#FROM debian
#RUN apt -y update 
#RUN apt -y install python3-pip 
#RUN apt -y update ; apt -y install python3-pip 

#FROM python:slim-bullseye

ADD requirements.txt ./
RUN pip3 \
        install \
        -r requirements.txt \
        --break-system-packages ; \
    adduser \
        --home /app \
        --disabled-password app
#RUN adduser --home /app --disabled-password app
USER app
WORKDIR /app

COPY . .

EXPOSE 5000

CMD ["python3", "weather.app.py"]