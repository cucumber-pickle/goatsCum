# Real Goats Bot Telegram Automation Script

GoatsСum — это скрипт автоматизации для выполнения миссий в Telegram-боте Real Goats. 

[TELEGRAM CHANNEL](https://t.me/cucumber_scripts)

## Обновления
- **10.10.24** Исправлена ошибка добавления токенов в token.json.

## Регистрация

Чтобы использовать этого бота, необходимо зарегистрироваться в Goats Telegram Bot:

1. Откройте бота [t.me/Realgot_real](https://t.me/realgoats_bot/run?startapp=754d1e37-4a72-4a04-8a35-81eb362eba61)
2. Нажмите кнопку "[Start App](https://t.me/realgoats_bot/run?startapp=754d1e37-4a72-4a04-8a35-81eb362eba61)" or "[Open App]([url](https://t.me/realgoats_bot/run?startapp=754d1e37-4a72-4a04-8a35-81eb362eba61))" button
3. Установите этот бот автоматизации Real Goats.
4. Have Fun 

## Установка

### Шаг 1: Клонирование репозитория
```bash
git clone https://github.com/cucumber-pickle/goatsCum.git
cd goatsCum
```
**Создайте виртуальное окружение (не обязательно)**

 ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
 ```
### Step 2: Шаг 2: Установка зависимостей
Установите необходимые пакеты, выполнив следующую команду:

```bash
pip install -r requirements.txt
```

### Step 3: Изменение конфигураций (опционально)
Файл config.json позволяет изменять настройки скрипта:
account_delay: время (в секундах) между операциями с аккаунтами.
looping: время (в секундах) перед началом нового цикла операций с аккаунтами.


### Формат файла proxies.txt
Файл proxies.txt должен содержать один прокси на строку в следующем формате:

```ruby
username:password@ip:port
username:password@ip:port
```

## Где взять tgWebAppData (query_id / user_id)

1. Запустите телеграм portable или вэб версию
2. Запустите приложение, для которого хотите получить дату
3. Нажмите `F12` на клавиатуре (или правой кнопкой мыши и "проверить" в ТГ portable)
4. Откройте вкладку консоль
5. Вставьте этот код в консоль:

```javascript
copy(Telegram.WebApp.initData)
```

6. Вы получите tgWebAppData, которая выглядит вот так:

```
query_id=AA....
user=%7B%22id%....
```
7. Добавьте ее в файл `data.txt` 


## Этот бот был Вам полезен? Пожалуйста, подписывайтесь на канал или можете купить мне кофе: 
``` 0xc4bb02b8882c4c88891b4196a9d64a20ef8d7c36 ``` - BSC (BEP 20)

``` UQBiNbT2cqf5gLwjvfstTYvsScNj-nJZlN2NSmZ97rTcvKz0 ``` - TON

``` 0xc4bb02b8882c4c88891b4196a9d64a20ef8d7c36 ``` - Optimism

``` THaLf1cdEoaA73Kk5yiKmcRwUTuouXjM17 ``` - TRX (TRC 20)

## License
This project is licensed under the `MIT License`.

## Контакты
Если есть вопросы или предложения, пишите в Telegram  [CUCUMBER TG CHAT](https://t.me/cucumber_scripts_chat)