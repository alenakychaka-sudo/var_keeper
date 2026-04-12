FROM python:3.12.3-alpine
WORKDIR /app

# Копируем файл из корня контекста (репозитория) в текущую папку контейнера (.)
COPY requirements.txt .

# Копируем содержимое src/app в текущую папку контейнера (.)
COPY src/app/ .

RUN pip install -r requirements.txt
ENTRYPOINT [ "python" ]
CMD [ "app.py" ]
