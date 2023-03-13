# Web API для скачивания сообщений из Telegram-каналов
Репозиторий создан в рамках выполнения проекта по курсу "Введение в облачные технологии".

Выполнили: [Трохачев Андрей](https://github.com/akulen0k), [Пичугин Влад](https://github.com/wdfacfan), [Бекмамбетов Тимур](https://github.com/nbveh112112)

## Описание
Огромное количество людей уже пользуется мессенджером Telegram, и, кажется, его популярность будет только расти.  Велико также количество всевозможных телеграм-каналов: новостных, образовательных и проч. Иногда может возникнуть потребность сохранять себе контент телеграм-канала, но такой возможности мессенджер не предоставляет. Наш телеграм-бот и Web API помогут быстро и просто скачать посты из телеграм-канала за необходимый промежуток времени.

## Реализация

- телеграм-бот для доступа к телеграм-каналам написан на Python
- Web API написан на C# с использованием ASP.NET Core
- для взаимодействия бота и API используется база данных PostgreSQL
- используется Docker

## Функционал приложения
- начать отслеживать новый телеграм-канал
- получить список отслеживаемых телеграм-каналов с их id
- скачать сообщения из определённого телеграм-канала за определённый промежуток дат
- получить сообщения, скачанные из телеграм-канала

## Как устроен API
Реализована возможность работать с API с помощью Swagger. 

![image](https://user-images.githubusercontent.com/121407222/224692473-72375805-8299-4c96-b644-c37893a6a0c9.png)

На скриншоте представлены хэндлеры ("ручки"), реализующие заявленный функционал.
