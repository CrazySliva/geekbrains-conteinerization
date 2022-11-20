FROM alpine:3.17

RUN apk add --update --no-cache python3 py3-pip && ln -sf python3 /usr/bin/python

COPY . ./app

RUN pip3 install -r ./app/requirements.txt

EXPOSE 8080

ENTRYPOINT ["/usr/bin/python", "./app/app.py"]
