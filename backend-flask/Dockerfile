FROM python:3.10-slim-buster

WORKDIR /backend-flask

COPY requirements.txt .

RUN python -m pip install -r requirements.txt

COPY . .

ENV FLASK_ENV=develop

EXPOSE ${PORT}

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]
