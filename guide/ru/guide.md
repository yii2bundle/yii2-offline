Руководство
===

## Описание

При включенном режиме, пользователи увидят сообщение, наподобие:

> Сайт временно недоступен.
> Проводятся профилактические работы. Просим Вас зайти через несколько минут.

Режим оффлайн включают в следующих случаях:

* при деплое
* при миграциях в БД
* при устранении аварийных ситуаций

В АПИ-приложение приходит статус 500 и такое тело:

```json
{
    "title": "Сайт временно недоступен",
    "message": "Проводятся профилактические работы. Просим Вас зайти через несколько минут."
}
```

Страница на стороне пользователя периодически обновляется, 
так что пользователь сразу увидит, когда сайт заработает.

## Использование

Выбора режима:

```
php yii offline
```

после чего, Вам будет предложено: включить или выключить режим оффлайн.

Также, этот функционал доступен в админке.