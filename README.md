# 🚀 Название проекта

**[SoloBot]**!  
[Бот для API x-ray]  

## 📋 Оглавление
1. [Описание](#описание)
2. [Требования](#требования)
3. [Установка](#установка)
4. [Конфигурация](#конфигурация)
5. [Запуск](#запуск)
6. [Автор](#автор)

---

## 📖 Описание

[Бот предназначен для автоматизирования выдачи ключей, хранении их в базе данных и управления подключениями]  


---

## 💻 Требования

Для работы проекта необходимы следующие компоненты:

- **Python** версии 3.8 или выше
- **Git** для клонирования репозитория
- **Virtualenv** для создания виртуального окружения (рекомендуется)
- **postgresql** для работы базы данных

---

## ⚙️ Установка

### 1️⃣ Шаг 1: Клонирование репозитория

Клонируйте репозиторий и перейдите в его директорию:

```bash
git clone https://github.com/Vladless/Solo_bot.git
cd solo_bot
```

### 2️⃣ Шаг 2: Создание и активация виртуального окружения

```
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Шаг 3: Установка зависимостей

```
pip install -r requirements.txt
```

### 🛠️ Конфигурация

Для правильной работы вам нужно установить и запустить postgresql, создать пользователя для работы с базой данных и выдать ему права

Также создайте файл config.py в корневой папке проекта с вашими данными:

```
API_TOKEN = токен вашего бота телеграм
API_URL = домен вашего x-ray сервера с указанием порта и дополнительным путем панели вида "https://{domen}:{port}/{путь}" без слэша в конце
ADMIN_USERNAME = логин от вашей панели x-ray
ADMIN_PASSWORD = пароль от вашей панели x-ray
ADD_CLIENT_URL = f"{API_URL}/panel/api/inbounds/addClient"
GET_INBOUNDS_URL = f"{API_URL}/panel/api/inbounds/list/"
AUTH_URL = f"{API_URL}/login/"
DOMEN = "{ваш домен без https://}:443"
DATABASE_URL = путь к вашей базе данных, имеет вид "postgresql://{user}:{password}@{Ip-adress}:{port}/{имя базы данных}"
ADMIN_ID = ID телеграм профиля администратора
CHANNEL_URL = ссылка на ваш телеграм канал
```

### 🚀 Запуск

введите команду из виртуального окружения

```
python main.py
```






