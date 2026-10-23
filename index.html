<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>MultiBox Premium App</title>
    <!-- Подключаем официальный скрипт Telegram WebApp -->
    <script src="https://telegram.org"></script>
    <!-- Подключаем иконки Lucide для красивого меню -->
    <script src="https://unpkg.com"></script>
    <style>
        :root {
            --bg-color: var(--tg-theme-bg-color, #0f0f16);
            --text-color: var(--tg-theme-text-color, #ffffff);
            --hint-color: var(--tg-theme-hint-color, #8e8e93);
            --accent-color: var(--tg-theme-button-color, #007aff);
            --card-bg: rgba(255, 255, 255, 0.05);
            --glass-blur: blur(15px);
            --glass-border: rgba(255, 255, 255, 0.08);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            user-select: none;
            -webkit-user-select: none;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background: linear-gradient(135deg, #0f0f16 0%, #151528 100%);
            color: var(--text-color);
            min-height: 100vh;
            overflow-x: hidden;
            padding-bottom: 90px;
        }

        /* Премиальный эффект матового стекла (Glassmorphism) */
        .glass-card {
            background: var(--card-bg);
            backdrop-filter: var(--glass-blur);
            -webkit-backdrop-filter: var(--glass-blur);
            border: 1px solid var(--glass-border);
            border-radius: 20px;
            padding: 20px;
            margin: 15px;
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.3);
        }

        header {
            padding: 20px 15px 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            font-size: 24px;
            font-weight: 800;
            background: linear-gradient(45deg, #007aff, #00ffcc);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .user-badge {
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 255, 255, 0.08); 
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 14px;
            border: 1px solid var(--glass-border);
        }

        /* Навигация (Нижнее меню) */
        nav {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(15, 15, 22, 0.85);
            backdrop-filter: var(--glass-blur);
            -webkit-backdrop-filter: var(--glass-blur);
            border-top: 1px solid var(--glass-border);
            display: flex;
            justify-content: space-around;
            padding: 12px 0 calc(12px + env(safe-area-inset-bottom));
            z-index: 1000;
        }

        .nav-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 4px;
            color: var(--hint-color);
            font-size: 11px;
            text-decoration: none;
            transition: all 0.3s ease;
            width: 20%;
        }

        .nav-item.active {
            color: var(--accent-color);
            transform: translateY(-2px);
        }

        .nav-item i {
            width: 24px;
            height: 24px;
        }

        /* Разделы приложения */
        .content-section {
            display: none;
            animation: fadeIn 0.4s ease forwards;
        }

        .content-section.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Стили кликера */
        .game-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px 0;
        }

        .score-display {
            font-size: 42px;
            font-weight: 800;
            margin-bottom: 5px;
            color: #ffd700;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.4);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .passive-income {
            font-size: 14px;
            color: #00ffcc;
            margin-bottom: 30px;
        }

        .click-circle {
            width: 220px;
            height: 220px;
            border-radius: 50%;
            background: radial-gradient(circle, #2c2c44 0%, #1a1a2e 100%);
            border: 6px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 0 40px rgba(0, 122, 255, 0.2);
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            position: relative;
            transition: transform 0.05s ease;
        }

        .click-circle:active {
            transform: scale(0.96);
            border-color: var(--accent-color);
        }

        .click-circle img {
            width: 120px;
            height: 120px;
            pointer-events: none;
        }

        .upgrade-btn {
            background: linear-gradient(45deg, var(--accent-color), #0051ff);
            color: white;
            border: none;
            padding: 12px 24px;
            border-radius: 14px;
            font-weight: 600;
            margin-top: 35px;
            width: 100%;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(0, 122, 255, 0.3);
        }

        /* Стили контента для Кино, Музыки, Книг */
        .grid-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin-top: 15px;
        }

        .media-card {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--glass-border);
            border-radius: 15px;
            overflow: hidden;
        }

        .media-thumb {
            width: 100%;
            aspect-ratio: 16/10;
            background: #232335;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--hint-color);
        }

        .media-info {
            padding: 10px;
        }

        .media-title {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 4px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }

        .media-subtitle {
            font-size: 12px;
            color: var(--hint-color);
        }

        /* Текст вылетающих цифр при клике */
        .floating-text {
            position: absolute;
            color: #ffd700;
            font-size: 28px;
            font-weight: 800;
            pointer-events: none;
            animation: floatUp 0.8s ease-out forwards;
        }

        @keyframes floatUp {
            0% { opacity: 1; transform: translateY(0) scale(1); }
            100% { opacity: 0; transform: translateY(-100px) scale(0.8); }
        }
    </style>
</head>
<body>

    <header>
        <h1>MultiBox</h1>
        <div class="user-badge">
            <i data-lucide="user" style="width:16px; height:16px;"></i>
            <span id="username-display">User</span>
        </div>
    </header>

    <!-- КИНО -->
    <div id="movies" class="content-section active">
        <div class="glass-card">
            <h2>🍿 Популярные фильмы</h2>
            <div class="grid-grid">
                <div class="media-card">
                    <div class="media-thumb"><i data-lucide="clapperboard"></i></div>
                    <div class="media-info"><div class="media-title">Интерстеллар</div><div class="media-subtitle">Фантастика</div></div>
                </div>
                <div class="media-card">
                    <div class="media-thumb"><i data-lucide="clapperboard"></i></div>
                    <div class="media-info"><div class="media-title">Начало</div><div class="media-subtitle">Триллер</div></div>
                </div>
            </div>
        </div>
    </div>

    <!-- МУЗЫКА -->
    <div id="music" class="content-section">
        <div class="glass-card">
            <h2>🎧 Тренды недели</h2>
            <div class="grid-grid">
                <div class="media-card">
                    <div class="media-thumb"><i data-lucide="music-4"></i></div>
                    <div class="media-info"><div class="media-title">Night Vibes</div><div class="media-subtitle">Lo-Fi Beats</div></div>
                </div>
                <div class="media-card">
                    <div class="media-thumb"><i data-lucide="music-4"></i></div>
                    <div class="media-info"><div class="media-title">Cyberpunk Drive</div><div class="media-subtitle">Synthwave</div></div>
                </div>
            </div>
        </div>
    </div>

    <!-- КНИГИ -->
    <div id="books" class="content-section">
        <div class="glass-card">
            <h2>📚 Топ книг</h2>
            <div class="grid-grid">
                <div class="media-card">
                    <div class="media-thumb"><i data-lucide="book-open"></i></div>
                    <div class="media-info"><div class="media-title">Атомные привычки</div><div class="media-subtitle">Саморазвитие</div></div>
                </div>
                <div class="media-card">
                    <div class="media-thumb"><i data-lucide="book-open"></i></div>
                    <div class="media-info"><div class="media-title">Дюна</div><div class="media-subtitle">Фантастика</div></div>
                </div>
            </div>
        </div>
