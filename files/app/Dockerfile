FROM alexmbarbosa/flask-python3 AS flask-app

LABEL env="dev"
LABEL MANTAINER="alexmbarbosa"

WORKDIR /app
COPY . /app

EXPOSE 5000

CMD [ "python", "./app.py" ]