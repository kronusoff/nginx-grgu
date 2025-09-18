1. Git
Проверка версии:git -v

git version 2.45.1.windows.1

<img width="997" height="157" alt="изображение" src="https://github.com/user-attachments/assets/e25e117b-b041-4274-ad73-257b41f01458" />


3. Клонирование репозитория

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

<img width="766" height="289" alt="изображение" src="https://github.com/user-attachments/assets/ed02a89c-769a-4db9-bcf6-ad4e49d0b0a3" />

---

Запуск контейнера с Nginx

6. Подготовка файлов

index.html:GRGU

Dockerfile:FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html

<img width="809" height="516" alt="изображение" src="https://github.com/user-attachments/assets/bb5d5e29-78a3-43b6-abb9-48c1a5783530" />
<img width="817" height="151" alt="изображение" src="https://github.com/user-attachments/assets/c41dc1a6-7ad0-402f-99fc-b985ecee128b" />


7. Сборка и запуск контейнера

docker build -t grgu-nginx .

docker run -d -p 8080:80 grgu-nginx

<img width="1552" height="97" alt="изображение" src="https://github.com/user-attachments/assets/8b48709d-7be5-41a8-ba29-4275f2d900b3" />


8. Проверка

Открыть в браузере:

http://localhost:8080

На странице отображается текст: GRGU

<img width="997" height="59" alt="изображение" src="https://github.com/user-attachments/assets/463023ab-eb21-41ec-b286-89ad730a2160" />


Работа с Git

9. Сохранение и загрузка изменений

git checkout -b dev
git add .
git commit -m "123"

git push origin dev

<img width="997" height="556" alt="изображение" src="https://github.com/user-attachments/assets/a9613776-bb36-4f76-86aa-6a0e024a72da" />


