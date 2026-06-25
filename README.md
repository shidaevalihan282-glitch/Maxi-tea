<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Кайфовый Чай</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@700&family=Inter:wght@400;600&display=swap" rel="stylesheet">
    <style>
        /* Основная палитра и сброс отступов */
        :root {
            --bg-color: #15131C;
            --accent-green: #A3FF00;
            --text-yellow: #FFF200;
            --text-purple: #BFA6F9;
            --text-gray: #888888;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: #FFFFFF;
            font-family: 'Inter', sans-serif;
            display: flex;
            justify-content: center;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            padding: 20px 40px;
            box-sizing: border-box;
        }

        /* Шапка сайта (Header) */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo-placeholder {
            background-color: white;
            color: #00A3E0;
            font-weight: 800;
            padding: 5px 15px;
            border-radius: 4px;
            text-align: center;
            line-height: 1;
            font-size: 20px;
            border: 2px solid #00A3E0;
        }

        .auth-buttons {
            display: flex;
            align-items: center;
            gap: 24px;
        }

        .auth-buttons a {
            color: var(--accent-green);
            text-decoration: none;
            font-size: 14px;
            font-weight: 600;
        }

        .auth-buttons button {
            background-color: var(--accent-green);
            color: var(--bg-color);
            border: none;
            padding: 10px 24px;
            border-radius: 6px;
            font-weight: 600;
            font-size: 14px;
            cursor: pointer;
            transition: opacity 0.2s;
        }

        .auth-buttons button:hover {
            opacity: 0.8;
        }

        /* Главный экран (Hero Section) */
        main {
            margin-top: 60px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .main-title {
            color: var(--text-yellow);
            font-family: Georgia, serif; 
            font-style: italic;
            font-weight: 700;
            font-size: 90px;
            margin: 0 0 50px 0;
            text-align: center;
        }

        .hero-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            gap: 40px;
        }

        .hero-text {
            flex: 1;
        }

        .hero-text h2 {
            font-family: 'Caveat', cursive;
            color: var(--text-purple);
            font-size: 56px;
            line-height: 1.2;
            margin: 0;
            font-weight: 700;
        }

        .hero-video-banner {
            flex: 1;
            position: relative;
            border: 4px solid #8A2BE2;
            border-radius: 8px;
            height: 350px;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            background-color: #000;
        }

        /* Подвал (Footer) */
        footer {
            margin-top: 100px;
            display: flex;
            justify-content: space-between;
            width: 100%;
            padding-bottom: 40px;
        }

        .footer-info {
            max-width: 300px;
        }

        .namedly-brand {
            color: var(--accent-green);
            font-weight: 600;
            margin-top: 20px;
            display: block;
        }

        .footer-info p {
            color: var(--text-gray);
            font-size: 12px;
            margin-top: 8px;
            line-height: 1.5;
        }

        .footer-nav {
            display: flex;
            gap: 80px;
        }

        .nav-column h4 {
            color: var(--accent-green);
            font-size: 14px;
            margin: 0 0 16px 0;
            font-weight: 600;
        }

        .nav-column ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        .nav-column li {
            margin-bottom: 12px;
        }

        .nav-column a {
            color: var(--text-gray);
            text-decoration: none;
            font-size: 13px;
            transition: color 0.2s;
        }

        .nav-column a:hover {
            color: white;
        }

        /* Адаптивность для мобильных экранов */
        @media (max-width: 900px) {
            .hero-content {
                flex-direction: column;
                text-align: center;
            }
            .main-title {
                font-size: 60px;
            }
            .hero-text h2 {
                font-size: 40px;
                margin-bottom: 30px;
            }
            .hero-video-banner {
                width: 100%;
            }
            footer {
                flex-direction: column;
                gap: 40px;
            }
            .footer-nav {
                flex-wrap: wrap;
                gap: 40px;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <div class="logo-placeholder">Maxi<br>Чай</div>
            <div class="auth-buttons">
                <a href="#">Зарегистрироваться</a>
                <button>Войти</button>
            </div>
        </header>

        <main>
            <h1 class="main-title">Макси чай</h1>
            
            <div class="hero-content">
                <div class="hero-text">
                    <h2>Самый<br>популярный<br>чайный напиток<br>в Казахстане</h2>
                </div>
                
                <div class="hero-video-banner">
                    <iframe 
                        width="100%" 
                        height="100%" 
                        src="https://www.youtube.com/embed/qn9ow6aXYuI" 
                        title="YouTube video player" 
                        frameborder="0" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
                        referrerpolicy="strict-origin-when-cross-origin" 
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </main>

        <footer>
            <div class="footer-info">
                <div class="logo-placeholder" style="display: inline-block;">Maxi<br>Чай</div>
                <span class="namedly-brand">Namedly</span>
                <p>Descriptive line about what your company does.</p>
            </div>

            <div class="footer-nav">
                <div class="nav-column">
                    <h4>Features</h4>
                    <ul>
                        <li><a href="#">Core features</a></li>
                        <li><a href="#">Pro experience</a></li>
                        <li><a href="#">Integrations</a></li>
                    </ul>
                </div>
                <div class="nav-column">
                    <h4>Learn more</h4>
                    <ul>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Case studies</a></li>
                        <li><a href="#">Customer stories</a></li>
                        <li><a href="#">Best practices</a></li>
                    </ul>
                </div>
                <div class="nav-column">
                    <h4>Support</h4>
                    <ul>
                        <li><a href="#">Contact</a></li>
                        <li><a href="#">Support</a></li>
                        <li><a href="#">Legal</a></li>
                    </ul>
                </div>
            </div>
        </footer>
    </div>

</body>
</html>

