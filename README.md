# VKCoinPy
A bot for vk.com (Russian social network) virtual currency (VKCoin) mining. All the further description is in Russian.

[![Группа ВКонтакте](https://img.shields.io/badge/%D0%93%D1%80%D1%83%D0%BF%D0%BF%D0%B0%20VK-VKCoinPy-green.svg)](https://vk.com/vkcoinpy)

# Требования
Для запуска бота необходимо установить Python 3.7.

Скачать можно здесь:
https://www.python.org/downloads/

После того, как Python установлен, необходимо установить зависимости. 


## Windows
Запустить `install.bat`.

## Linux
Команда в терминале:

```bash
pip install -r requirements/base.txt
```

# Настройка
Для работы бота нужен токен ВК. О том, как его получить, можно почитать [здесь](https://github.com/cursedseal/VCoinX#%D0%BF%D0%BE%D0%BB%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5-%D1%82%D0%BE%D0%BA%D0%B5%D0%BD%D0%B0)

Токен нужно вставить в config.ini:

```
VK_TOKEN = токен
```

Помимо этого, в `config.ini` также можно прописывать следующие настройки: 
- `CURRENT_PLACE_MESSAGE_INTERVAL` - интервал между выводами в консоль текущей позиции в ТОПе в секундах
- `AUTOBUY_ENABLED` - True, если автозакупка должна работать, иначе - False. 
- `AUTOBUY_INTERVAL` - интервал между закупками в секундах
- `AUTOBUY_ITEMS` - вещи для автозакупки.  Через запятую, например, `CURSOR,CPU`. 

| Параметр              | Описание                                         |
|-----------------------|--------------------------------------------------|
| VK_TOKEN              | Токен страницы пользователя                      |
| AUTOBUY_ENABLED       | Автозакупка (True - включена, False - выключена) |
| AUTOBUY_INTERVAL      | Интервал автозакупки в секундах                  |
| AUTOBUY_ITEMS         | Предметы для автозакупки                         |
| MISSED_MESSAGES_LIMIT | Лимит ошибок до переподключения                  |
| LOG_LEVEL             | Уровень логов                                    |

> AUTOBUY_ITEMS перечисляются через запятую, может быть CURSOR, CPU, CPU_STACK, COMPUTER, SERVER_VK, QUANTUM_PC, DATACENTER. 


# Запуск
Запуск бота осуществляется следующей командой из терминала или командной строки: 

## Windows
Запустить `start.bat`. 

## Linux
```
python vkcoin.py
```


# RoadMap
- [ ] Русский язык
- [ ] Переводы
- [ ] Доделать автозакупку предметов.
