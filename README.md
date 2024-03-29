Описание проекта

"Киттиграм" — сайт, на котором пользователи могут публиковать фотографии котиков и не только. Каждый котик помимо фото, имени, цвета имеет достижения, которых может быть несколько.

Авторизованные пользователи могут добавлять и редактировать своих котиков, чужие котики доступны только для чтения.

Как развернуть проект в Docker 

Для развертывания проекта на локальном сервере необходимо выполнить несколько шагов:
1. Сделать Fork репозитория gbolezin/kittygram_final с github
2. Установить и запустить Docker
3. В корневом каталоге проекта выполнить сборку проекта с указанием файла docker-compose.yml
    docker compose -f docker-compose.yml up -d

Для развертывания проекта на удаленном сервере необходимо выполнить несколько шагов:
1. Сделать Fork репозитория gbolezin/kittygram_final с github
2. Сформировать файл корневой_каталог_проекта/.github/worflows/main.yml (можно использовать дефолтный)
3. В разделе GitHub->Settings->Security->Secrets and Variables->Actions добавить необходимые переменные для передачи в workflow (наименование переменных можно посмотреть в файле main.yml, см. п.2)
4. Сделать push исходного кода в свой репозиторий в ветку "main", после чего проверить исполнение в разделе Github->Actions вашего проекта


Стек используемых технологий

В качестве бэкенда в проекте используется Django
API реализован на Django Rest Framework
Фронтэнд выполнени на стеке React
СУБД PostgreSQL, веб-сервер Nginx
Контейнеризация Docker
Для автоматизации деплоя использован GitHub Actions


Автор проекта - Болезин Георгий (Bolezin George)
e-mail: g.bolezin@zenith24.ru
tg: @gbolezin
https://kittygram.zenith24.ru
