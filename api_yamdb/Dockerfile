FROM python:3.7-slim

WORKDIR /app

COPY requirements.txt .
# вместо пути до папки теперь нужно что-то указывать или просто опускаем?

RUN pip3 install -r /requirements.txt --no-cache-dir

COPY . .

CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000"]
