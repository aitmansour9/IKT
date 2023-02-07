# IKT
# Выполнил работу
Аит Мансур Фарид Группа 035
# Проделанное в работе
- Изменил файлы пайчарма: Удалил api.py. Перенес часть кода в main.py

- Перед работой с Nginx, сначала создал файл requirements.txt, который содержит список предустановок и файл Dockerfile. С помощью Dockerfile автоматизировал создание окружения, установку зависимостей, запуск проекта.

- С помощью команды docker build -t main_app:0.0.1 . создал образ. С помощью команды docker run -p 8080:8080 main_app:0.0.1 запустил контейнер с пробросом портов. Удостоверился в создании и работе образа с помощью программы Docker Desktop.

- В корне директории проекта создал файл docker-compose.yaml. Вставил следующий код:

'''
version: '3.4'

services:
    web:
        build:
            context: .
        ports:
            - "8080-8081:8080" 
'''
