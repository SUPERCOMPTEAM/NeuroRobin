# NeuroModule
IT Проект в рамках Цифровой Кафедры МАИ. Кейс от комапнии "СберТех" ```Применение нейронных сетей для балансировки нагрузки в веб-серверах (Nginx)```. Основной репозиторий проекта.

## Исполнители
- Иван Павлов - TeamLead  
- Фёдор Меркулов - Backend-разработчик 1  
- Денис Фадеев - Backend-разработчик 2  
- Вячеслав Климовец - Backend-разработчик 3  
- Илья Лютоев - ML Engineer 1  
- Артемий Крючков - ML Engineer 2  
- Иван Антипин - DevOps-Engineer  
- Даниил Желанов - Тестировщик  
- Карина Воробьева - Technical Writer  
- Егор Корсаков - Системный аналитик

## Технологии
Проект представляет из себя модуль для Nginx для балансировки нагрузки между серверами с использованием весов, полученных от нейросетевой модели. Сам модуль написан на языке программирования C.

## Структура проекта
- **ML** - содержит код, связанный с обучением и применением нейросетевой модели для расчёта весов.
- **config** - включает файлы конфигурации, необходимые для работы модуля.
- **docker** - содержит файлы для развертывания проекта в контейнерах Docker.
- **mysql** - включает скрипты и файлы для работы с базой данных MySQL.
- **ngx_http_upstream_sct_neuro_module** - непосредственно модуль для Nginx, написанный на языке C.
- **recalculator** - скрипты и файлы для перерасчёта весов на основе данных от нейросети.
- **docker-compose.yml** - файл для оркестрации Docker-контейнеров.

## Установка
Чтобы запустить проект локально, выполните следующие шаги:
1. Клонируйте репозиторий:  
  ```git clone https://github.com/SUPERCOMPTEAM/SCT_nginx.git```
2. Перейдите в директорию проекта:  
  ```cd SCT_nginx```
3. Собираем и запускаем все контейнеры, определённые в файле ```docker-compose.yml```  
  ```docker compose -f ./docker-compose.yml up —build```
