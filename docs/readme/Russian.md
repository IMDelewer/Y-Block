<div align="center"><h1>🧱 YBlock</h1></div>

<div align="center">
<h4>Многопользовательский игровой сервер на базе DDNet с системой аккаунтов, экономикой и мини-играми<h4>

![Версия](https://img.shields.io/badge/version-1.0.10-blue?style=for-the-badge&logo=appveyor)
![Лицензия](https://img.shields.io/badge/License-Close--Source-red?style=for-the-badge&logo=opensourceinitiative)
![Платформа](https://img.shields.io/badge/platform-Linux%20%7C%20Windows%20-lightgrey?style=for-the-badge&logo=appveyor)
![Язык Программирования](https://img.shields.io/badge/language-C++-blue?style=for-the-badge&logo=c%2B%2B)
![Предложения](https://img.shields.io/badge/issues-0-brightgreen?style=for-the-badge&logo=github)
![Контрибьютеры](https://img.shields.io/badge/contributors-5-lightgrey?style=for-the-badge&logo=github)
![Звезды](https://img.shields.io/github/stars/IMDelewer/Y-Block?style=for-the-badge&logo=github)
![Последний коммит](https://img.shields.io/github/last-commit/IMDelewer/Y-Block?style=for-the-badge&logo=github)
![Вики](https://img.shields.io/badge/wiki-Documentation-lightgrey?style=for-the-badge&logo=readthedocs)
</div>

---

<div align="center">
  <h2><strong style="color:red;">⚠️ Внимание:</strong> Этот проект имеет закрытый исходный код и является собственностью компании.
 Доступ ограничен. Чтобы запросить разрешение, свяжитесь с <strong>IMDelewer </strong>через 
   Дискорд (@delewer)</h2>
</div>

---

## 🌐 Поддерживаемые языки

- [🇺🇸 English](English.md)
- [🇷🇺 Русский](Russian.md)

---

## 🧭 Навигация

- [📋 О проекте](#-о-проекте)
- [✨ Возможности](#-возможности)
- [🚀 Установка](#-установка)
- [⚙️ Конфигурация](#%EF%B8%8F-конфигурация)
- [📦 Автоматическая сборка](#-автоматическая-сборка)
- [📚 Документация](#-документация)
- [🤝 Вклад в проект](#-вклад-в-проект)
- [📄 Лицензия](#-лицензия)
- [👨‍💻 Автор](#‍-автор)

---

## 📋 О проекте

YBlock — это модифицированный сервер на основе движка DDNet/DDRace с расширенными возможностями: 

- 🔐 Система аккаунтов с сохранением прогресса  
- 💰 Внутриигровая экономика и банковская система  
- 🏗️ Система участков (plots) с управлением объектами  
- 🎮 Встроенные мини-игры и дуэли  
- 🌍 Поддержка протоколов 0.6 и 0.7  
- 🌐 Мультиязычность (включая русский язык)

---

## ✨ Возможности

### Система аккаунтов
- Регистрация и авторизация игроков  
- Сохранение прогресса между сессиями  
- Файловое хранилище данных в формате `.acc`

### Экономическая система
- Внутриигровая валюта  
- Банковские операции (депозит/снятие)  
- Магазин с предметами  
- Система скидок и временных предметов

### Мини-игры
- Дуэли 1 на 1 с настраиваемыми аренами  
- Система приглашений  
- Отслеживание статистики

---

## 🚀 Установка

### Требования
- **Компилятор:** GCC 7+, Clang 5+ или MSVC 2017+  
- **CMake:** 3.12 или новее  
- **Python:** 3.x  
- **Библиотеки:** libcurl, OpenSSL, zlib  

### Быстрый старт

> ЭТО ЗАКРЫТЫЙ ПРОЕКТ, У ВАС НЕ ПОЛУЧИТЬСЯ СКОПИРОВАТЬ ЕГ


```bash
git clone https://github.com/IMDelewer/YBlock.git --recursive
cd YBlock
sudo apt update
sudo apt install cmake build-essential libcurl4-openssl-dev libfreetype6-dev python3
mkdir build && cd build
cmake ..
make -j$(nproc)
./yblock
```

---

## ⚙️ Конфигурация

Создайте файл `autoexec.cfg` в корневой директории:

```cfg
# Основные настройки
sv_name "My YBlock Server"
sv_map YBlock
sv_port 8303
sv_max_clients 16

# Система аккаунтов
sv_login_required 0
sv_acc_folder "data/accounts"

# Экономика
sv_bank_modes 1
sv_money_drop_file "data/moneydrops.txt"

# Участки
sv_plot_file "data/plots"
```

---

## 📦 Автоматическая сборка

Проект использует GitHub Actions для автоматической сборки:

- ✅ Автоматическая компиляция для Linux
    
- 📦 Создание релизов с бинарными файлами
    
- 🔄 Поддержка ручного запуска workflow
    
---

## 📚 Документация

Смотри [Основная страница](/docs/wiki/Main%20Page.md)

---

## 🤝 Вклад в проект

Мы приветствуем вклад!

1. Форкните репозиторий
    
2. Создайте ветку для новой функции (`git checkout -b feature/amazing-feature`)
    
3. Закоммитьте изменения (`git commit -m 'Add amazing feature'`)
    
4. Запушьте в ветку (`git push origin feature/amazing-feature`)
    
5. Создайте Pull Request
    

---

## 📄 Лицензия

MIT License — см. **[LICENSE](LICENSE)**

---

## 👨‍💻 Автор

- **[IMDelewer](https://github.com/IMDelewer)**