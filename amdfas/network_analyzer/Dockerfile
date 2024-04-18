FROM python:3.12.0-slim

WORKDIR /app

COPY ../../requirements.txt /app/requirements.txt

RUN pip install -r /app/requirements.txt

COPY . .

CMD ["python", "manage.py", "runserver", "0.0.0.0:8004"]
