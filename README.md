# 🏆 World Cup 2026 Predictions App / ЧМ-2026 Прогнозы

An offline-first, mobile-designed progressive web application (PWA) made for predictions, friendly leagues, and leaderboard tracking during the **FIFA World Cup 2026**. 

Автономное прогрессивное веб-приложение (PWA), оптимизированное под мобильные экраны, созданное для спортивных прогнозов, дружеских лиг и отслеживания таблиц лидеров во время **Чемпионата мира по футболу 2026**.

<img width="1672" height="941" alt="ChatGPT Image 11 июн  2026 г , 12_28_45" src="https://github.com/user-attachments/assets/592f28b1-0bfd-4ede-af00-280d1df65cd9" />

---

## 🇺🇸 English Version

### 💡 Concept & Motivation
The goal of this project is to deliver the excitement, friendly rivalry, and adrenaline of sports forecasting of a real bookmaker, but without any financial risk. It is a form of **"eco-friendly gambling"** for friends and colleagues, where the primary driver is the pure competitive spirit and proving whose football intuition is supreme. 

Developed as a challenge to build a fully functional cloud-based product from scratch in just 48 hours.

### 🛠️ Architecture & Tech Stack
*   **Frontend:** React (Vite) + Tailwind CSS (Mobile-first, high-fidelity dark neon theme).
*   **Database & BaaS:** Supabase (User profiles, secure credentials, and real-time predictions).
*   **Automation:** Serverless cron automation using Deno Edge Functions & PostgreSQL `pg_cron` extensions. It fetches official live data from the **API-Sports (REST API)** and completely recalculates the global leaderboard every 10 minutes.
*   **Hosting:** Fully containerized and hosted on **Google Cloud**.

### 🌟 Key Features
*   **Dual-Language Support:** Instant toggle between English and Russian (RU/EN).
*   **Strict Anti-Cheat Time-Lock:** Predictions are hard-locked on both the client side and the server side exactly at the scheduled kickoff time (`match_date`) to prevent players from waiting for game progression or遅延 (updates latency) to submit winning bets.
*   **Exact Score Scoring Engine:** 
    *   **5 Points:** For guessing the exact full-time score (e.g., predicting 2-1 when the match ends 2-1).
    *   **2 Points:** For predicting the correct outcome (winning team or draw) but with a different scoreline (e.g., predicting 2-1 when the match ends 2-0).
*   **Installable App (PWA):** Install straight to the home screen with customizable icons and standalone viewports.

---

## 🇷🇺 Русская версия

### 💡 Концепция и мотивация
Этот проект был создан ради тех самых чистых эмоций, азарта и дофамина от футбольных прогнозов в кругу друзей и коллег, но без какого-либо риска для кошелька. Это своего рода **«экологичная лудомания»**, где главным драйвером выступает не страх потерять деньги, а спортивный интерес и желание доказать, что твоя интуиция круче всех.

Проект собран в качестве челленджа «с нуля до работающего облачного решения за 48 часов».

### 🛠️ Архитектура и стек технологий
*   **Фронтенд:** React (Vite) + Tailwind CSS (Mobile-first дизайн, стильный темный неоновый интерфейс).
*   **База данных и BaaS:** Supabase (профили пользователей, хранение прогнозов и мгновенный лидерборд).
*   **Автоматизация:** Deno Edge Functions + PostgreSQL `pg_cron`. Серверный сценарий автоматически обращается к REST-сервису **API-Sports**, стягивает текущие live-результаты и каждые 10 минут полностью пересчитывает таблицу результатов и очков.
*   **Хостинг:** Всё развернуто как отказоустойчивое PWA на инфраструктуре **Google Cloud**.

### 🌟 Основные фишки
*   **Двуязычный интерфейс:** Полная локализация на русский и английский языки (RU/EN).
*   **Защита от читерства (Time-Lock):** Жесткий лок прогнозов на клиенте и сервере по времени начала матча (`match_date`). Игрок не может держать форму открытой или отправить прогноз после стартового свистка, даже если статус live из API приходит с небольшой задержкой.
*   **Продуманная система начисления очков:**
    *   **5 очков:** За точно угаданный счет матча (например, ставка 2-1 при исходе 2-1).
    *   **2 очка:** За правильно угаданного победителя или ничью, но с другим счетом (например, ставка 2-1 при исходе 2-0).
*   **Поддержка PWA (Добавить на экран «Домой»):** Выглядит как нативное приложение благодаря отсутствию рамок браузера.

---

## 📱 Installation Instructions / Как установить

### iOS (Safari)
1. Open the preview link in your Safari browser. / Откройте ссылку приложения в браузере Safari.
2. Tap the **"Share"** button (share icon). / Нажмите кнопку **«Поделиться»**.
3. Select **"Add to Home Screen"** from the list. / Выберите пункт **«На экран "Домой"»**.
4. Launch the app from your home screen directly without browser bars! / Запускайте прямо с рабочего стола как полноценное приложение!

### Android (Chrome)
1. Open the preview link in Google Chrome. / Откройте ссылку в браузере Chrome.
2. Tap the **three vertical dots** in the upper right. / Нажмите на **три точки** в правом верхнем углу.
3. Select **"Install App"** or **"Add to Home Screen"**. / Выберите **«Установить приложение»** или **«Добавить на главный экран»**.
