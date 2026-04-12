FROM python:3.12.3-alpine
WORKDIR /app

# Копируем из корня репозитория (без начального /)
COPY requirements.txt /app/
# Копируем содержимое папки src/app в текущую директорию контейнера
COPY src/app/ /app/

RUN pip install -r requirements.txt
ENTRYPOINT [ "python" ]
CMD [ "app.py" ]
