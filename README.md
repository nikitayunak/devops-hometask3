# devops-hometask3
docker build -t node-app:v1 . - білд зображення з докерфайлу
docker run -m 3g --cpus="2.0" -p 80:80 -d --rm node-app:v1 - запуск контейнера з обмеженням використання пам'яті та cpu, вказуванням порта
docker login - логін в аккаунт Docker Hub 
docker tag node-app:v1 nikitayunak25/node-app - додавання нового тегу
docker push nikitayunak25/node-app - завантаження готового зображення на Docker Hub з автоматичним створенням репозиторія
