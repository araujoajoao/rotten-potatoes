FROM python:3.8-slim-buster
WORKDIR /app
COPY requirements.txt .
RUN python -m pip install -r requirements.txt
COPY . /app
EXPOSE 5001
CMD ["gunicorn", "--workers=1", "--bind", "0.0.0.0:5001", "-c", "config.py", "app:app"]

