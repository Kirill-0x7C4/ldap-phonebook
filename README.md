# LDAP phonebook

# Корпоративный телефонный справочник с отображением контактов на карте офиса

Контакты делятся на два типа:
- Импортированные из AD
- Локальные

Импортированные контакты нельзя редактировать, их можно только скрывать из списка и указывать расположение на карте.
Все изменения нужно производить в AD, после чего провести повторную синхронизацию, при которой будут добавлены новые и обновлены существующие контакты.

Функциональные возможности:
- Импорт контактов из AD
- Показать/скрыть любой контакт
- Добавлять, редактировать и удалять локальные контакты
- Указать расположение контакта на плане офиса. Удобно для ориентирования в большой компании
- Экспорт в .xml файл для использования в приложении [PhoneBook](https://github.com/pfzim/PhoneBook) для Windows

Карты хранятся в файлах `templ/map[1-5].png`

## Системные требования
Apache, MySQL, PHP.

Подключить модули расширения в php.ini или скомпилировать PHP с поддержкой LDAP
- `extension=php_ldap.dll`
- `extension=php_fileinfo.dll`

## Установка
- Открыть в браузере `install.php` и заполнить предлагаемые параметры
- Заменить изображения карт `templ/map[1-5].png` своими схемами





This service import users info from LDAP/AD to MySQL DB

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_0.png)

Show all contacts on map

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_1.png)

Show selected contact on map

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_2.png)

Installation

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_3.png)

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_4.png)

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_5.png)

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_6.png)

![screenshot](https://raw.githubusercontent.com/pfzim/ldap-phonebook/master/other/screenshot_7.png)


Dmitry V. Zimin <pfzim@mail.ru>