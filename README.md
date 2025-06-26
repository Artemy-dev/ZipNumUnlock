# 🚀 [ZipNumUnlock](https://github.com/Artemy-dev/ZipNumUnlock) — Numeric Password Cracker for Archives  
A simple Python CLI tool to brute-force numeric passwords (up to 6 digits) for ZIP, RAR, and 7z archives.  
(Простой CLI-инструмент на Python для подбора числовых паролей (до 6 цифр) к архивам ZIP, RAR и 7z.)
![Демо](demo.gif)
---

## 💻 Supported Platforms

- ✅ Windows  
- ✅ macOS  
- ✅ Linux  

---

## 📦 Features / Возможности

- 🔹 Supports numeric passwords from 1 to 6 digits with leading zeros / Поддержка числовых паролей от 1 до 6 цифр с ведущими нулями  
- 🔹 Automatically finds first ZIP, RAR or 7z archive in current directory / Автоматический поиск первого архива ZIP, RAR или 7z в текущей директории  
- 🔹 Checks passwords by extracting archive content (uses temporary folder for 7z) / Проверка паролей через попытку извлечения (для 7z — во временную папку)  
- 🔹 Uses `pyzipper`, `rarfile`, and `py7zr` libraries for archive handling / Использует библиотеки `pyzipper`, `rarfile` и `py7zr` для работы с архивами  

---

## ❓ Why this project? / Зачем этот проект?

This tool automates brute-force of numeric passwords for common archive formats with minimal setup and easy extensibility.  
Инструмент автоматизирует подбор числовых паролей к популярным архивам с минимальной настройкой и возможностью расширения.

---

## 🚀 Installation / Установка

```bash
git clone https://github.com/Artemy-dev/ZipNumUnlock.git
cd ZipNumUnlock
pip install -r requirements.txt
````

---

## ⚙️ Usage / Пример использования

```bash
python main.py
```

### Usage details / Применение

* Скрипт ищет первый архив с расширением `.zip`, `.rar` или `.7z` в текущей папке.
* Производит перебор числовых паролей от 1 до 6 цифр с ведущими нулями.
* Для ZIP и RAR пароли проверяются попыткой извлечения архива.
* Для 7z используется временная папка для распаковки с проверяемым паролем.
* При успешном подборе пароль выводится в консоль и перебор останавливается.
* Если архив не найден или пароль не подходит, скрипт завершится без результата.

---

## 📁 Project Structure / Структура проекта

```
├── main.py
├── requirements.txt
└── README.md
```

---

## 👤 Author / Автор

**Artem Grachev**<br>
Python/Golang Developer | ML & DevOps Enthusiast<br>
Telegram: [@Artemy\_Develop](https://t.me/Artemy_Develop)<br>
GitHub: [Artemy-dev](https://github.com/Artemy-dev)

---

## 🌍 SEO Keywords

* zip password cracker
* rar unlock
* 7z password recovery
* python zip unlock
* bruteforce zip
* cli archive unlocker
* extract password protected archive
* python bruteforce tool
* zipnumunlock
* archive password breaker
