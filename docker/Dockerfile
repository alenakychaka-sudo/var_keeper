FROM python:3.12.3-alpine
WORKDIR /app

# Копируем файл зависимостей из корня проекта в папку /app внутри контейнера
COPY requirements.txt ./

# Копируем содержимое вашей папки src/app в папку /app внутри контейнера
# Убираем начальный слэш перед src!
COPY src/app/ ./

RUN pip install --no-cache-dir -r requirements.txt
ENTRYPOINT [ "python" ]
CMD [ "app.py" ]
