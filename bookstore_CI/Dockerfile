FROM python:3.11-slim

WORKDIR /usr/src/app

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000
CMD ["uvicorn", "bookstore.main:app", "--host", "0.0.0", "--port", "8000", "--reload"]
# --reload is for development purposes, remove it in production