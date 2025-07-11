# English‑Bot‑Telegram

**Telegram-бот для изучения английского языка** на Python 3.

### ⚙️ Возможности

- Сохранение и перевод новых слов  
- Отображение транскрипции (IPA)  
- Аудио‑произношение (через TTS‑API или локальные файлы)  
- Команды: `/start`, `/new`, `/list`, `/translate <слово>`, `/cancel`, и др.  
- Возможность отправки словарной карточки  
- (Опционально) Напоминания о повторении  
- Простая настройка через `.env`

---

## 🚀 Быстрый старт — запуск в VS Code

1. **Склонируйте репозиторий:**
   ```bash
   git clone https://github.com/RavilBoyukzade/english-bot-telegram.git
   cd english-bot-telegram
Создайте виртуальное окружение:

bash
Копировать
Редактировать
python -m venv venv
В Windows:

powershell
Копировать
Редактировать
.\venv\Scripts\activate
В macOS/Linux:

bash
Копировать
Редактировать
source venv/bin/activate
Установите зависимости:

bash
Копировать
Редактировать
pip install -r requirements.txt
Создайте файл .env в корне проекта (см. пример ниже):

ini
Копировать
Редактировать
TELEGRAM_TOKEN=ваш_токен_бота
DICTIONARY_API_KEY=...',
TTS_API_KEY=...
TELEGRAM_TOKEN: токен от @BotFather

DICTIONARY_API_KEY, TTS_API_KEY: (опционно) для API словаря и TTS

Откройте проект в VS Code (например, code .).

Настройте конфигурацию отладки (launch.json):
Пример для python:

json
Копировать
Редактировать
{
  "name": "Запуск бота",
  "type": "python",
  "request": "launch",
  "program": "${workspaceFolder}/bot.py",
  "envFile": "${workspaceFolder}/.env"
}
Запустите бота через Debug или терминал:

bash
Копировать
Редактировать
python bot.py
Откройте Telegram и начните диалог с вашим ботом.

