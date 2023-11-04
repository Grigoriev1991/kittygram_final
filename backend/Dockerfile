FROM python:3.9
WORKDIR /kittygram
COPY . .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "kittygram_backend.wsgi"]