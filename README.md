# 🚀 [ZipNumUnlock](https://github.com/Artemy-dev/ZipNumUnlock)

---

## 📝 Description | Описание

A simple Python **CLI tool** to **brute-force** numeric passwords (up to 6 digits) for **ZIP**, **RAR**, and **7z** archives.<br>
(Простой **CLI-инструмент** на Python для **подбора числовых паролей** (до 6 цифр) к архивам **ZIP**, **RAR** и **7z**.)

---

## 📂 Contents | Оглавление

- [🛠 Install | Установка](#-install--установка)
- [🚀 Usage | Использование](#-usage--использование)
- [🧱 Stack | Технологии](#-stack--технологии)
- [📄 License | Лицензия](#-license--лицензия)
- [📬 Contacts / Автор](#-contacts--автор) 

---

## 🛠 Install | Установка

```bash
git clone https://github.com/Artemy-dev/ZipNumUnlock.git
```

```bash
cd ZipNumUnlock
```

```bash
pip install -r requirements.txt
```

### 🔧 Дополнительно (для работы с .rar архивами)

Для корректной работы с `.rar`-архивами необходимо установить внешнюю утилиту **unrar**:

* **Ubuntu:**

  ```bash
  sudo apt update && sudo apt install unrar
  ```

* **macOS (через Homebrew):**

  ```bash
  brew install unrar
  ```

* **Windows:**

  * Скачай `unrar.exe` с официального сайта: [https://www.rarlab.com/download.htm](https://www.rarlab.com/download.htm)
  * Добавь путь к `unrar.exe` в системную переменную PATH:
    * Нажми Win + R, введи sysdm.cpl, нажми Enter
    * Перейди во вкладку Дополнительно → нажми Переменные среды
    * В разделе Системные переменные найди Path и нажми Изменить
    * Нажми Создать и вставь путь к папке, где находится unrar.exe (например: C:\Tools\Unrar)
    * Подтверди изменения, нажав ОК во всех окнах
  * Перезапусти терминал или систему, чтобы изменения вступили в силу

---

## 🚀 Usage | Использование

1. Поместите архив с расширением `.zip`, `.rar` или `.7z` в директорию с проектом `ZipNumUnlock`.
2. Запустите скрипт.
```bash
python main.py
```
3. Скрипт ищет первый архив в текущей директории и производит перебор числовых паролей от 0 до 999999.

![Демо](demo.gif)

---

## 🧱 Stack | Технологии

* **Языки:** `Python 3.11`
* **Библиотеки:**
  * `pyzipper`
  * `rarfile`
  * `py7zr`

---

## 📄 License | Лицензия

MIT License — свободно использовать, изменять и распространять.

---

## 📬 Contacts / Автор

**Artem Grachev**
Python • Golang • Backend • AI/ML • Cybersecurity • Teaching

* Telegram: [@Artemy_Develop](https://t.me/Artemy_Develop)
* Telegram-канал: [Код.Просто](https://t.me/code_just)
* GitHub: [Artemy-dev](https://github.com/Artemy-dev)

---

## 🔍 Keywords

zip password cracker, rar unlock, 7z password recovery, python zip unlock, bruteforce zip, cli archive unlocker, extract password protected archive, python bruteforce tool, zipnumunlock, archive password breaker, cybersecurity, python script, password recovery, security audit tools
