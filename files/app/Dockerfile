FROM alexmbarbosa/flask-python3 AS flask-app

LABEL env="dev"
LABEL MANTAINER="alexmbarbosa"

WORKDIR /app
COPY . /app

RUN pip install -r requirements.txt

EXPOSE 5000

CMD [ "python", "./app.py" ]