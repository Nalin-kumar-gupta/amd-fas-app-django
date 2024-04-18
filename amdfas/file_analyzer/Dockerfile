FROM python:3.12.0-slim

WORKDIR /app

COPY --from=amdfas-microserv /app/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["python", "manage.py", "runserver", "0.0.0.0:8002"]
