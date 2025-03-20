# 🚀 Server Monitoring & Telegram Alerts

![Project Status](https://img.shields.io/badge/status-active-brightgreen)

📡 **Автоматизированная система мониторинга серверов с отправкой уведомлений в Telegram**

## 📌 Описание проекта  
Этот проект позволяет отслеживать ключевые метрики серверов (нагрузку CPU, RAM, диск, сеть) и получать оповещения в Telegram при критических изменениях. Поддерживает развёртывание в Docker и интеграцию с CI/CD.

## 🔧 Стек технологий  
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)

## ⚙️ Функции  
✅ Мониторинг загрузки CPU, RAM, диска и сети  
✅ Запись данных в PostgreSQL  
✅ Отправка уведомлений в Telegram через Telegram Bot API  
✅ Развёртывание в Docker  
✅ Настройка через `.env` файл  

## 🚀 Быстрый старт  

### 1️⃣ Установка и запуск  
Клонируем репозиторий:  
```bash
git clone https://github.com/munez1919/server-monitoring.git
cd server-monitoring
```
  
### 2️⃣ Настройка окружения  
Создай `.env` файл и заполни его:  
```bash
TELEGRAM_BOT_TOKEN="your_token"
CHAT_ID="your_chat_id"
DB_HOST="localhost"
DB_PORT="5432"
DB_USER="your_user"
DB_PASS="your_password"
DB_NAME="monitoring"
```

### 3️⃣ Запуск сервиса  
Через Docker:  
```bash
docker-compose up -d
```
Без Docker (локально через Python):  
```bash
pip install -r requirements.txt
python monitor.py
```

## 📊 Логирование и мониторинг  
Данные хранятся в PostgreSQL. Можно подключиться через `psql` и выполнить запрос:  
```sql
SELECT * FROM metrics ORDER BY timestamp DESC LIMIT 10;
```

## 📢 Связь  
Автор: **munez1919**  
📌 GitHub: [munez1919](https://github.com/munez1919)  
✉️ Telegram: [@slav1k19](https://t.me/slav1k19)  

---

🔥 **Буду рад обратной связи и контрибьютам!** 🚀

