1. Git
Проверка версии:git -v
git version 2.45.1.windows.1

2. Клонирование репозитория

Команда:git clone https://github.com/kronusoff/nginx-grgu.git
cd nginx-grgu

---
Проверка версий Docker и Docker Compose

3. Docker

Проверка версии:docker -v
Docker version 28.0.1, build 068a01e
4. Docker Compose

Проверка версии:docker-compose -v
Docker Compose version v2.33.1-desktop.1

---

Запуск контейнера с Nginx

6. Подготовка файлов

index.html:GRGU

Dockerfile:FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html


7. Сборка и запуск контейнера

docker build -t grgu-nginx .
docker run -d -p 8080:80 grgu-nginx


8. Проверка

Открыть в браузере:
http://localhost:8080
На странице отображается текст: GRGU


Работа с Git

9. Сохранение и загрузка изменений

git checkout -b dev
git add .
git commit -m "123"

git push origin dev
