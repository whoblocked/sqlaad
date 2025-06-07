Вот готовый текст для твоего README.md — просто скопируй и вставь в файл в корне проекта:

---

# SQLAD — Telegram WebApp для склада и продаж

## 🚀 Быстрый старт

1. **Установить зависимости:**
   ```bash
   npm install
   ```
2. **Запустить фронтенд:**
   ```bash
   npm run dev
   ```
3. **Запустить сервер:**
   ```bash
   node server/index.js
   ```

## 🧩 Интеграция с Google Sheets

- Получите credentials сервисного аккаунта Google (JSON) и положите в `server/credentials.json`.
- В файле `server/googleSheets.js` укажите свой `spreadsheetId`.

## 🤖 Интеграция с Telegram WebApp

- Зарегистрируйте бота через [@BotFather](https://t.me/BotFather).
- В настройках бота укажите ссылку на фронтенд (Vite dev-сервер через ngrok/localtunnel или деплой на Vercel).
- В коде уже есть поддержка Telegram WebApp API (user info, mainButton, close). Всё работает автоматически.

## 🌍 Деплой в облако (рекомендация)

- **Фронт**: [Vercel](https://vercel.com/) (бесплатно, идеально для Vite/React)
- **Бэкенд**: [Render](https://render.com/) или [Railway](https://railway.app/) (бесплатно для Node.js/Express)
- После деплоя укажи публичные ссылки в настройках бота и фронта.

## 📄 PDF с кириллицей

- Для PDF используется jsPDF + Roboto (кириллица поддерживается).
- Если PDF не отображает кириллицу — проверьте, что base64 Roboto корректно вставлен в `src/fonts/registerRoboto.js`.

## 🛠️ Структура проекта

```
telegram-warehouse-bot/
├─ public/
├─ src/
│  ├─ components/
│  ├─ context/
│  ├─ fonts/
│  ├─ pages/
│  ├─ utils/
│  ├─ App.jsx
│  ├─ main.jsx
├─ server/
│  ├─ index.js
│  ├─ googleSheets.js
│  ├─ resetData.js
│  ├─ pdfGenerator.js
├─ vite.config.js
└─ package.json
```

## 🧠 Возможные проблемы

- Если не работает Tailwind — проверьте `tailwind.config.js` и `postcss.config.js`.
- Для Google Sheets нужен рабочий сервисный аккаунт и права на таблицу.
- Для PDF с кириллицей — нужен корректный base64 Roboto.
- Для работы WebApp в Telegram нужен публичный адрес фронта (через ngrok/localtunnel или облако).

---

**Проект полностью готов для запуска и доработки!**

---
