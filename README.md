<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>Алтарис · мир без вайпов</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    
    <!-- ИКОНКИ САЙТА (ТЕПЕРЬ ТУТ, ГДЕ НАДО) -->
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-icon-180x180.png">
    <link rel="icon" type="image/png" sizes="192x192" href="/android-icon-192x192.png">
    <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="96x96" href="/favicon-96x96.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            background-color: #0c0a14;
            background-image: url('https://images.unsplash.com/photo-1604871000636-074fa5117945?q=80&w=1887&auto=format&fit=crop');
            background-size: cover;
            background-attachment: fixed;
            background-position: center;
            background-blend-mode: overlay;
            color: #f0eaff;
            line-height: 1.6;
            position: relative;
            scroll-behavior: smooth;
        }
        body::before {
            content: '';
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle at 20% 30%, rgba(95, 30, 150, 0.7), rgba(15, 5, 30, 0.98));
            pointer-events: none;
            z-index: 0;
        }

        .wrapper {
            max-width: 1400px;
            margin: 0 auto;
            padding: 1.5rem 2rem 4rem;
            position: relative;
            z-index: 2;
        }

        /* новостная строка */
        .news-ticker {
            background: rgba(55, 25, 90, 0.8);
            backdrop-filter: blur(8px);
            border: 1px solid #c48aff;
            border-radius: 60px;
            padding: 0.7rem 2rem;
            margin-bottom: 2rem;
            display: flex;
            align-items: center;
            gap: 1rem;
            box-shadow: 0 0 25px #b56eff;
            overflow: hidden;
        }
        .ticker-label {
            background: #c48aff;
            color: #0c0a14;
            font-weight: 800;
            padding: 0.3rem 1.2rem;
            border-radius: 40px;
            font-size: 0.9rem;
            text-transform: uppercase;
        }
        .ticker-content {
            overflow: hidden;
            white-space: nowrap;
            flex: 1;
        }
        .ticker-scroll {
            display: inline-block;
            animation: tickerMove 30s linear infinite;
            font-weight: 500;
            color: #eeddff;
        }
        .ticker-scroll span {
            margin-right: 3rem;
        }
        .ticker-scroll i {
            color: #ffb2ff;
            margin: 0 0.5rem;
        }
        @keyframes tickerMove {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }

        /* логотип */
        .logo-hero {
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 1rem 0 2.5rem;
            filter: drop-shadow(0 0 30px #c27eff);
        }
        .logo-placeholder {
            max-width: 650px;
            width: 60%;
            aspect-ratio: 3/1;
            background: rgba(25, 10, 45, 0.6);
            backdrop-filter: blur(4px);
            border: 3px solid #c48aff;
            border-radius: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.2rem;
            font-weight: 800;
            letter-spacing: 6px;
            color: #f0e2ff;
            box-shadow: 0 0 70px #b05eff;
            background-size: contain;
            background-position: center;
            background-repeat: no-repeat;
            margin: 0 auto;
        }

        /* боковая навигация */
        .side-nav {
            position: fixed;
            right: 1.5rem;
            top: 50%;
            transform: translateY(-50%);
            background: rgba(45, 20, 70, 0.8);
            backdrop-filter: blur(15px);
            border: 1px solid #d7a5ff;
            border-radius: 60px;
            padding: 1.2rem 0.6rem;
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
            z-index: 999;
            box-shadow: 0 0 40px #b56eff;
        }
        .side-nav a {
            color: #dbbaff;
            font-size: 1.6rem;
            padding: 0.4rem 0.9rem;
            border-radius: 40px;
            transition: 0.2s;
            text-align: center;
            position: relative;
        }
        .side-nav a:hover, .side-nav a.active {
            color: #fff;
            background: #b05eff;
            box-shadow: 0 0 30px #e9adff;
            transform: scale(1.1);
        }
        .side-nav a .tooltip {
            position: absolute;
            right: 120%;
            top: 50%;
            transform: translateY(-50%);
            background: #3e2560;
            color: #f0e2ff;
            padding: 0.3rem 1rem;
            border-radius: 30px;
            font-size: 0.9rem;
            font-weight: 600;
            border: 1px solid #c48aff;
            opacity: 0;
            pointer-events: none;
            transition: 0.15s;
        }
        .side-nav a:hover .tooltip {
            opacity: 1;
            right: 140%;
        }

        /* мобильная навигация */
        .mobile-bottom-nav {
            display: none;
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            background: #2a1745cc;
            backdrop-filter: blur(20px);
            border-top: 2px solid #b87eff;
            justify-content: space-around;
            padding: 0.8rem 1rem;
            z-index: 1000;
        }
        .mobile-bottom-nav a {
            color: #dbb5ff;
            font-size: 2rem;
        }

        /* контейнер вкладок */
        .tab-container {
            background: rgba(22, 12, 38, 0.75);
            backdrop-filter: blur(20px);
            border: 2px solid #b77eff;
            border-radius: 60px;
            padding: 2rem 2.5rem;
            margin-bottom: 3rem;
            box-shadow: 0 20px 50px #1e0b38;
        }

        .tabs-header {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
            border-bottom: 2px solid #6a3f9e;
            padding-bottom: 1.5rem;
            margin-bottom: 2rem;
        }
        .tab-btn {
            background: transparent;
            border: none;
            color: #d1b0ff;
            font-size: 1.3rem;
            font-weight: 600;
            padding: 0.8rem 2rem;
            border-radius: 60px;
            cursor: pointer;
            transition: 0.2s;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .tab-btn i { color: #e2b5ff; }
        .tab-btn:hover {
            background: #4f3080;
            color: white;
        }
        .tab-btn.active {
            background: #b56eff;
            color: #100020;
            box-shadow: 0 0 30px #cf9fff;
        }

        .tab-pane { display: none; animation: fade 0.3s; }
        .tab-pane.active-pane { display: block; }
        @keyframes fade { from { opacity: 0.3; } to { opacity: 1; } }

        /* ===== ПЛЮШКИ ===== */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        .feature-card {
            background: linear-gradient(145deg, #251a3a, #1a0f2a);
            border: 2px solid #a56eff;
            border-radius: 40px;
            padding: 2rem 1.5rem;
            transition: 0.3s;
            box-shadow: 0 15px 30px #0f0520;
            position: relative;
            overflow: hidden;
        }
        .feature-card::before {
            content: '';
            position: absolute;
            top: -30%;
            left: -30%;
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, #c28eff40, transparent 70%);
            border-radius: 50%;
            z-index: 0;
        }
        .feature-card:hover {
            transform: translateY(-8px);
            border-color: #ddb5ff;
            box-shadow: 0 0 50px #b56eff;
        }
        .feature-icon {
            font-size: 3.2rem;
            color: #e5beff;
            margin-bottom: 1.5rem;
            position: relative;
            z-index: 2;
        }
        .feature-card h3 {
            font-size: 1.8rem;
            color: #f0d4ff;
            margin-bottom: 1rem;
            position: relative;
            z-index: 2;
        }
        .feature-card p {
            color: #ceb9f0;
            font-size: 1rem;
            line-height: 1.5;
            position: relative;
            z-index: 2;
        }

        /* ===== РАСЫ ===== */
        .race-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
            gap: 1.2rem;
            margin-top: 1.5rem;
        }
        .race-card {
            background: #1f123a;
            border: 2px solid #6f44b0;
            border-radius: 40px;
            padding: 1.3rem 1.5rem;
            transition: 0.2s;
            cursor: pointer;
            box-shadow: 0 10px 20px #11051f;
        }
        .race-card:hover {
            border-color: #d9a9ff;
            box-shadow: 0 0 35px #c08cff;
        }
        .race-card h4 {
            color: #f0d5ff;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .race-card h4 i { color: #cb9eff; }
        .race-expand {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            background: #2b1947;
            border-radius: 30px;
            margin-top: 0.8rem;
            padding: 0 1rem;
        }
        .race-expand-content {
            padding: 1.2rem 0.5rem;
            color: #e2d0ff;
            border-top: 1px dashed #a27bda;
        }
        .race-expand.show {
            max-height: 500px;
        }
        .race-badge {
            display: inline-block;
            background: #3f2770;
            color: #efdbff;
            padding: 0.2rem 1rem;
            border-radius: 30px;
            font-size: 0.8rem;
            margin-right: 0.5rem;
            margin-bottom: 0.4rem;
            border: 1px solid #ba85ff;
        }

        /* ===== ПРАВИЛА ===== */
        .rules-detailed {
            display: grid;
            grid-template-columns: repeat(2,1fr);
            gap: 1.5rem;
        }
        .rule-block {
            background: #21153b;
            border-left: 8px solid #b77eff;
            border-radius: 30px;
            padding: 1.5rem;
            box-shadow: 0 6px 18px #090012;
        }
        .rule-block h3 { color: #e2beff; margin-bottom: 1rem; font-size: 1.5rem; }
        .rule-list {
            list-style: none;
        }
        .rule-list li {
            margin-bottom: 0.7rem;
            padding-left: 1.8rem;
            position: relative;
        }
        .rule-list li::before {
            content: "⬩";
            color: #d79eff;
            font-weight: bold;
            font-size: 1.2rem;
            position: absolute;
            left: 0;
        }
        .punish {
            color: #ffa7a7;
            background: #4c1e3a;
            padding: 0.1rem 0.6rem;
            border-radius: 30px;
            font-size: 0.85rem;
            margin-left: 0.5rem;
        }

        /* галерея */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 1rem;
            margin: 1.5rem 0;
        }
        .gallery-item {
            aspect-ratio: 16/9;
            background: #2d194f;
            border-radius: 30px;
            border: 2px solid #a561ff;
            overflow: hidden;
            cursor: pointer;
            transition: 0.2s;
        }
        .gallery-item img {
            width: 100%; height: 100%; object-fit: cover; display: block;
        }
        .lightbox {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 10000;
            align-items: center;
            justify-content: center;
        }
        .lightbox.active {
            display: flex;
        }
        .lightbox img {
            max-width: 90vw;
            max-height: 85vh;
            border: 4px solid #c98eff;
            border-radius: 40px;
        }
        .close-lightbox {
            position: absolute;
            top: 30px; right: 50px;
            font-size: 3rem;
            color: white;
            cursor: pointer;
        }

        /* футер */
        .footer-purple {
            background: #1d0d32ee;
            backdrop-filter: blur(10px);
            border: 2px solid #b56eff;
            border-radius: 60px;
            padding: 2rem;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            margin-top: 3rem;
        }
        .footer-links a {
            color: #ebd2ff;
            font-size: 1.5rem;
            margin-right: 1.8rem;
        }
        .apply-footer {
            background: #d4a5ff;
            color: #180030;
            padding: 0.9rem 2.5rem;
            border-radius: 40px;
            font-weight: 700;
        }

        @media (max-width: 900px) {
            .side-nav { display: none; }
            .mobile-bottom-nav { display: flex; }
            .rules-detailed { grid-template-columns: 1fr; }
            .gallery-grid { grid-template-columns: repeat(2,1fr); }
            .wrapper { padding: 1rem 1rem 6rem; }
            .tab-container { padding: 1.5rem; }
        }
    </style>
</head>
<body>
    <!-- Весь твой код body остается БЕЗ ИЗМЕНЕНИЙ -->
    <!-- ... -->
</body>
</html>
