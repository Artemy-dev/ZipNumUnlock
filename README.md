# Zip/RAR/7z Numeric Password Cracker — CLI Tool on Python

**ZipNumUnlock** — это простой CLI-инструмент на Python для подбора числовых паролей (от `000000` до `999999`) к архивам форматов `.zip`, `.rar` и `.7z`. Поддерживает автоматический поиск архива в директории, работает на Windows, Linux и macOS.

---

## Особенности

- Поддерживаются архивы с паролем длиной до 6 цифр (от `"0"` до `"999999"` с ведущими нулями).
- Работает с форматами ZIP, RAR и 7z.
- Для RAR используется библиотека `rarfile`, которая требует наличия системной утилиты `unrar` (особенно актуально для macOS и Linux).
- Для 7z извлечение происходит во временную папку для проверки пароля.
- Автоматически ищет первый архив с расширением `.zip`, `.rar` или `.7z` в текущей папке.
- Конфигурируемая максимальная длина пароля (`MAX_PASS_LENGTH`).
- Простой и понятный код, легко расширяемый и модифицируемый.

---

## Установка зависимостей

Рекомендуется использовать виртуальное окружение:

```bash
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows
```

## Установите зависимости из requirements.txt

```bash
pip install -r requirements.txt
```

---

## Системные требования для работы с RAR

Для корректной работы с RAR-архивами необходимо, чтобы в системе была установлена утилита unrar.

- macOS:<br>
Утилиту unrar нужно скачать вручную с официального сайта RARLab:
https://www.rarlab.com/rar_add.htm

- Linux (Debian/Ubuntu):<br>
Установить unrar можно через пакетный менеджер:

```bash
sudo apt-get install unrar
```
- Windows:
Обычно rarfile может работать без внешних утилит, но рекомендуется проверить.

---

## Использование

1. Поместите архив с неизвестным числовым паролем (до 6 цифр) в директорию со скриптом.
2. Запустите скрипт командой:

```bash
python your_script_name.py
```

3. При успешном подборе пароля в консоли появится сообщение:

```
Пароль найден: 012345
```

4. Если пароль не найден, скрипт завершится без вывода пароля.

---

## Ограничения и производительность

- Поддерживаются только числовые пароли длиной до `MAX_PASS_LENGTH` (по умолчанию 6).
- Время перебора растёт экспоненциально с увеличением длины пароля.
- Перебор для `7z` может быть заметно медленнее из-за распаковки во временную директорию.
- Для расширенного перебора рекомендуется использовать специализированные инструменты или параллельные вычисления.

---

## Структура проекта
```
.
├── main.py  # Основной скрипт перебора паролей
├── requirements.txt     # Зависимости проекта
├── README.md            # Текущий файл с описанием
└── .gitignore           # Файлы и папки, игнорируемые Git (если есть)
```

---

## Автор
Artem Grachev<br>
Дата: 06.2025<br>
Версия: 1.06.25<br>
Оригинальный проект: [github.com/Artemy-dev/ZipNumUnlock](https://github.com/Artemy-dev/ZipNumUnlock)


## Tags

bruteforce, zip, rar, 7z, password recovery, unlock, python, archive, brute force, script, CLI, unzip, 
numeric passwords, bruteforce zip password, 7z password cracker, extract encrypted archive, zip rar 7z brute, 
numeric password unlock

## SEO Keywords

zip password cracker, rar unlock, 7z password recovery, python zip unlock, bruteforce zip, cli archive unlocker, extract password protected archive, python bruteforce tool, zipnumunlock, archive password breaker
