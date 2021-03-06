# Приложение для определения типа животного и его породы

### Один скрипт приложения подхватывает из БД животных, у которых не указан тип (кошка / собака), затем направляет ссылки на фото в ML приложение, определяющее тип. Полученный результат обрабатывается и заносится в БД.

### Второй срипт работает аналогично, но с определением породы.

Написано на Python с использованием библиотеки psycopg2 и requests

## Для запуска в контейнере
```
docker-compose up --build -d
```

## Для запуска локально

Создайте и запустите виртуальное окружение
```
(windows)
python -m venv venv
.\venv\Script\activate

(linux/macOS)
python3 -m venv venv
source venv/bin/activate
```
Установите зависимости
```
pip install -r req.txt
```
Запустите приложение
```
python main.py
```