
## Тестовое задание для Junior Developers

Привет!

Если вы видите это задание, значит вас заинтересовала вакансия самого крутого стартапа в России!

Это задание даст нам понимание ваших навыков (преимущественно Frontend), а также взаимодействие с движком Laravel.

Что от вас потребуется:
1) забрать файлы с этого репозитория и развернуть проект на своей локальной машине (если не понимаете, о чем идет речь, просто установите [Xampp](https://www.apachefriends.org/ru/index.html))
2) создать базу данных, чтобы сделать миграцию, и установить нужные зависимости composer и npm
3) создать в данном репозитории свою ветку (обязательно)
4) реализовать описанные в [макете](https://www.figma.com/file/vf1AkmViYYVGeeH2hRN7q9/Junior-For-Test) правки
5) сделать push своей ветки после завершения

Критерии успешного прохождения:
- ваш проект развернут на локальной машине
- вы поняли задачи и воплотили правки из макета
- вы создали отдельную ветку и сделали push со всеми доработками

Инструкция по работе с проектом:
- после того, как вы скачали файлы из репозитория к себе, их можно разместить в любой директории
- для работы на локальной машине вам потребуется установить [Xampp](https://www.apachefriends.org/ru/index.html) или его аналоги
- чтобы работать с Laravel, вам нужно поставить [Composer](https://getcomposer.org/download/)
- как только у вас появился Composer, нужно выполнить следующие команды:  
    `composer update`  
    `composer dump-autoload`  
- проект развернут, далее вам нужно создать у себя базу данных (в phpmyadmin, который поставляется из Xampp),
- данные о созданной базе нужно создать файл .env (копия .env.exapmle) и внести правки:  
    `DB_DATABASE` - имя базы  
    `DB_USERNAME` - имя пользователя (обычно root)  
    `DB_PASSWORD` - пароль (если не задавали, оставить пустым)  
- после создания базы, вам нужно сделать миграцию следующей командой:  
    `php artisan migrate`  
- все готово, теперь осталось запустить наш проект:  
    `php artisan serve`  
- если вы все сделали правильно, проект запущен на локалке и доступен по ссылке [localhost:8000](http://localhost:8000)
- для дальнейшних компиляций интерфейса вам потребуется пакет [npm](https://nodejs.org/en/download/)
- после его установки, вам необходимо сделать:  
    `npm install`  
- для последующей компиляции интерфейса используйте одну из следующих команд:  
    `npm run watch` - компиляция происходит в реальном времени, файлы создаются после любого изменения (решение для локальной разработки)  
    `npm run dev` - компиляция происходит один раз, создается несжатые файлы  
    `npm run prod` - компиляция происходит один раз, создается сжатые файлы (решение для продакшна)  

Подробности:
- это урезанная страница уже рабочего проекта
- задачи представляют собой похожий реальный кейс боевого проекта (над которым и нужно будет работать)
- весь необходимый backend уже написан, вам осталось дописать интерфейс для взаимодействия с ним
- модальное окно с добавлением трека уже готово, осталось сверстать второе модальное окно (с данными трека), баннер на странице (если нет добавленных треков) и список добавленных треков (данные можно получить из [/music_list](http://localhost:8000/music_list))
- треки обязательно должны добавляться в базу данных [/add_music](http://localhost:8000/add_music) (post-запрос)
- также нужно обязательно уделить внимание мобильной версии

Вы можете обращаться к автору задания с какими-либо вопросами или за подсказками: [на почту](mailto:maxmarok@gmail.com) и [в telegram](https://t.me/maxmarok)
