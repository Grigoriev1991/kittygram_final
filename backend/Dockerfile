FROM python:3.9
RUN pip install gunicorn==20.1.0
WORKDIR /kittygram
COPY . .
RUN pip install -r requirements.txt --no-cache-dir
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "kittygram_backend.wsgi"]