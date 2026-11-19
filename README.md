# PulDot.msg

[![Live Demo](https://img.shields.io/badge/demo-GitHub%20Pages-e63946?style=for-the-badge)](https://akitaandcaxap.github.io/PulDot.msg/)
[![Stack](https://img.shields.io/badge/stack-HTML%20%7C%20CSS%20%7C%20JS%20%7C%20Firebase-14080a?style=for-the-badge)](#architecture--архитектура)

> Dark/red glassmorphism web messenger with real-time chat rooms, mini-games & live "Playing" presence, friends status tracking, and WebRTC voice/video calls.

> Тёмно-красный веб-мессенджер в стиле glassmorphism с комнатами чата, мини-играми и статусом активности «Играет в...», списком друзей и голосовыми/видеозвонками по WebRTC.

---

## English

### ✨ Key Features

* **First-Visit Onboarding Wizard:** Clean welcome flow for setting a nickname and optional Firebase configuration, remembered via browser cookies and `localStorage`.
* **Multi-Room Real-Time Chat:** Jump between rooms (`#general`, `#games`, `#random`) or spin up new ones with instant message delivery and a local fallback when offline.
* **Games Hub & Live Presence:** Play built-in web games right inside a modal while automatically displaying a live `"Playing ..."` badge on your profile.
* **Friends & Activity Status:** Keep track of friends by nickname and see who is online or currently in a game.
* **WebRTC Voice & Video Calls:** Direct peer-to-peer audio and video calls powered by `RTCPeerConnection` with SDP/ICE signaling over Firebase Realtime Database.

### 🏗️ Architecture & Tech Stack

* **Single-File Client:** Self-contained `index.html` crafted with dark/red glassmorphism styling and native ES modules—no build step required.
* **Realtime Data & Signaling:** Firebase Realtime Database powers room messages (`messages/<room>`), user presence (`presence/<clientId>`), and call signaling (`calls/<room>`).
* **Client State:** Cookies and `localStorage` store user preferences, friend lists, and local fallback history.

---

## Русский

### ✨ Ключевые возможности

* **Приветственный настройщик:** Быстрый старт при первом визите с выбором никнейма и опциональной настройкой Firebase, сохраняемый в cookies и `localStorage`.
* **Комнаты общения в реальном времени:** Переключение между комнатами (`#general`, `#games`, `#random`), создание новых комнат и локальный запасной режим без подключения к сети.
* **Игры и статус «Играет в...»:** Запуск браузерных игр во всплывающем окне с автоматической плашкой активности в профиле.
* **Друзья и статусы:** Добавление друзей по нику с отображением статуса в сети и текущей игры.
* **Голосовые и видеозвонки (WebRTC):** Прямая аудио- и видеосвязь через `RTCPeerConnection` с обменом SDP/ICE-сигналами через Firebase Realtime Database.

### 🏗️ Архитектура и стек

* **Единый клиентский файл:** Весь интерфейс и логика собраны в одном `index.html` в тёмно-красном glassmorphism-дизайне на нативном HTML, CSS и JS (ES-модули).
* **Синхронизация и сигналинг:** Firebase Realtime Database хранит сообщения по комнатам (`messages/<room>`), статусы присутствия (`presence/<clientId>`) и сигналы звонков (`calls/<room>`).
* **Локальное состояние:** Cookies и `localStorage` хранят настройки пользователя, список друзей и локальную историю сообщений.
