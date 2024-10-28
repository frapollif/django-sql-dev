FROM python:3.10-bullseye

WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . ./app

EXPOSE 9999
CMD ["python", "manage.py", "runserver", "0.0.0.0:9999"]