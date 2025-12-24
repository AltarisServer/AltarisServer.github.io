<html lang="ru">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>ALTARIS — Мир без вайпов</title>
  <link rel="icon" type="image/png" href="favicon.png">



<script src="https://cdn.tailwindcss.com"></script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">

<style>
:root{
  --page:#0B0426;
  --surface:#1A0933;
  --surface2:#291248;
  --brand:#C084FC;
  --accent:#F7C948;
  --text:#F8F7FB;
}
body{background:var(--page);color:var(--text);font-family:Inter,sans-serif}
.shadow-pop{box-shadow:4px 4px 0 0 rgba(0,0,0,1)}
.press:hover{transform:translate(2px,2px);box-shadow:none;transition:.08s}
</style>
</head>
<script>
  // Открытие lightbox при клике или Enter
  function openLightbox(src){
    const lb = document.getElementById('lightbox');
    const img = document.getElementById('lightbox-img');
    img.src = src;
    lb.classList.remove('hidden');
    lb.classList.add('flex');
    // для доступности — фокус на изображение
    setTimeout(()=> img.focus?.(), 50);
  }

  function closeLightbox(){
    const lb = document.getElementById('lightbox');
    if(!lb) return;
    lb.classList.add('hidden');
    lb.classList.remove('flex');
    const lbimg = document.getElementById('lightbox-img');
    if(lbimg) lbimg.src = "";
  }

  // Навешиваем обработчики на все картинки в галерее
  document.addEventListener('DOMContentLoaded', () => {
    document.querySelectorAll('#gallery img[data-src]').forEach(img => {
      img.addEventListener('click', (e) => openLightbox(e.currentTarget.dataset.src));
      img.addEventListener('keydown', (e) => {
        if(e.key === 'Enter' || e.key === ' ') { e.preventDefault(); openLightbox(e.currentTarget.dataset.src); }
      });
    });

    // Закрыть по Esc
    document.addEventListener('keydown', (e) => {
      if(e.key === 'Escape') closeLightbox();
    });
  });
</script>



<body>

<!-- HEADER -->
<header class="max-w-6xl mx-auto p-4 flex justify-between items-center border-b-4 border-black">
  <div class="flex items-center gap-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3">
    <div class="w-10 h-10 bg-[var(--brand)] border-2 border-black rounded-xl flex items-center justify-center text-black font-extrabold">A</div>
    <div>
      <div class="text-xl font-bold lowercase">altaris</div>
      <div class="text-sm opacity-80">мир без вайпов</div>
    </div>
  </div>
 <!-- ИКОНКИ САЙТА -->
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

  <link rel="manifest" href="/manifest.json">

  <meta name="msapplication-TileColor" content="#ffffff">
  <meta name="msapplication-TileImage" content="/ms-icon-144x144.png">
  <meta name="theme-color" content="#ffffff">
  <div class="flex gap-2">
    <a href="https://discord.gg/6WDeeJnT" target="_blank"
      class="bg-[var(--accent)] text-black font-bold px-4 py-2 rounded-full border-2 border-black shadow-pop press">
      Discord
    </a>
    <a href="https://t.me/altaris_whitellist" target="_blank"
      class="border-2 border-black rounded-full px-4 py-2 shadow-pop press">
      Заявка
    </a>
  </div>
</header>

<!-- HERO -->
<section class="max-w-6xl mx-auto p-6 mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
  <h1 class="text-4xl font-extrabold mb-3">ALTARIS</h1>
  <p class="text-lg max-w-3xl">
    Minecraft-сервер формата полуваниллы для тех, кто хочет играть в одном мире долго.
    Без вайпов. Без обнулений. Со своей историей.
  </p>
  <p class="mt-2 opacity-90 max-w-3xl">
    Каждый дом, дорога и город остаются частью мира навсегда.
  </p>

  <div class="mt-6 flex flex-wrap gap-3">
    <a href="https://discord.gg/6WDeeJnT" target="_blank"
      class="bg-[var(--accent)] text-black font-bold px-6 py-3 rounded-full border-2 border-black shadow-pop press">
      Зайти на сервер
    </a>
    <a href="https://t.me/altaris_server" target="_blank"
      class="border-2 border-black rounded-full px-6 py-3 shadow-pop press">
      Новости проекта
    </a>
  </div>
</section>

<!-- ABOUT -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">О сервере</h2>
  <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-5 space-y-3">
    <p>
      ALTARIS — это живой мир Minecraft, который развивается вместе с игроками.
      Здесь нет вайпов, поэтому всё, что вы строите, имеет смысл и остаётся частью истории.
    </p>
    <p>
      Сервер создан для спокойной, долгой игры: масштабные проекты, города, дороги,
      совместные инициативы и события.
    </p>
    <p>
      Мир не гонится за скоростью. Он растёт постепенно, аккуратно и естественно.
    </p>
  </div>
</section>

<!-- FEATURES -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Плюшки сервера</h2>

  <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press">
      <h3 class="font-bold">Жители 2.0</h3>
      <p class="text-sm opacity-90">
        Улучшенная торговля, оптимизация и более прокаченные жители.
      </p>
    </div>

    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press">
      <h3 class="font-bold">Уникальный сид</h3>
      <p class="text-sm opacity-90">
        Горы с сакурой, реки, моря и просторные поля вокруг.
      </p>
    </div>

    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press">
      <h3 class="font-bold">1000 достижений</h3>
      <p class="text-sm opacity-90">
        Большой датапак с дополнительными целями и испытаниями.
      </p>
    </div>

    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press">
      <h3 class="font-bold">Уникальный лор</h3>
      <p class="text-sm opacity-90">
        История мира начнёт раскрываться в ближайшие дни.
      </p>
    </div>
  </div>
</section>

<!-- NEWS -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Лента новостей</h2>

  <div class="space-y-3">
    <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
      <div class="font-bold">15.12.2025 — Открытие сервера</div>
      <div class="text-sm opacity-90">
        ALTARIS успешно открылся. Онлайн на старте — 12 игроков.
      </div>
    </div>

    <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
      <div class="font-bold">20.12.2025 — Яйцо дракона</div>
      <div class="text-sm opacity-90">
        На открытии Энда яйцо дракона забрал игрок <b>kostyan4ik</b>.
      </div>
    </div>

    <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
      <div class="font-bold">Тайный Санта</div>
      <div class="text-sm opacity-90">
        Старт доброго и таинственного ивента. Каждый — чей-то волшебник в тени.
      </div>
    </div>
  </div>
</section>

<!-- GALLERY — ЗАМЕНИТЕ СТАРЫЙ БЛОК НА ЭТОТ -->
<section id="gallery" class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Скриншоты мира</h2>

  <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-4">
    <!-- 12 SCREENSHOTS: images/0.jpg .. images/11.jpg -->
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/0.jpg" alt="Скриншот 1" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/0.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/1.jpg" alt="Скриншот 2" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/1.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/2.jpg" alt="Скриншот 3" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/2.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/3.jpg" alt="Скриншот 4" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/3.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/4.jpg" alt="Скриншот 5" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/4.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/5.jpg" alt="Скриншот 6" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/5.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/6.jpg" alt="Скриншот 7" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/6.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/7.jpg" alt="Скриншот 8" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/7.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/8.jpg" alt="Скриншот 9" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/8.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/9.jpg" alt="Скриншот 10" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/9.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/10.jpg" alt="Скриншот 11" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/10.jpg">
    </div>

    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop overflow-hidden">
      <img src="images/12.jpg" alt="Скриншот 12" class="w-full h-full object-cover cursor-pointer" tabindex="0" data-src="images/11.jpg">
    </div>
  </div>

  <!-- Lightbox (один общий элемент) -->
  <div id="lightbox" class="fixed inset-0 hidden items-center justify-center z-50">
    <div class="absolute inset-0 bg-black/80" onclick="closeLightbox()"></div>
    <div class="relative max-w-5xl max-h-[90vh] p-4">
      <button onclick="closeLightbox()" class="absolute right-4 top-4 bg-[var(--surface)] border-2 border-black rounded-full p-2 shadow-pop">✕</button>
      <img id="lightbox-img" src="" alt="скриншот" class="max-h-[85vh] rounded-2xl border-2 border-black shadow-pop">
    </div>
  </div>
</section>


<!-- RULES (ACCORDION) — ЗАМЕНИТЕ СТАРЫЙ БЛОК НА ЭТОТ -->
<section id="rules" class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Правила сервера</h2>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">1. ОСНОВЫ ВЗАИМОУВАЖЕНИЯ</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Наш сервер — это комфортное пространство для всех игроков.</p>
      <p><strong>Обязанности каждого:</strong></p>
      <ul class="list-disc ml-5 mt-2">
        <li>Быть вежливым и доброжелательным.</li>
        <li>Уважать других игроков, их мнение, стиль игры и личные границы.</li>
        <li>Помнить, что за каждым ником — живой человек.</li>
      </ul>

      <p class="mt-3"><strong>Строго запрещено:</strong></p>
      <ul class="list-disc ml-5 mt-2">
        <li>Оскорбления, унижения, травля (буллинг).</li>
        <li>Расизм, сексизм и любая дискриминация.</li>
        <li>Провокации конфликтов и намеренное разжигание ссор.</li>
      </ul>

      <p class="mt-3"><strong>Также запрещено:</strong> реклама других серверов и проектов без разрешения; PvP без явного и обоюдного согласия.</p>

      <p class="mt-3"><strong>Наказание (PvP без согласия):</strong> первое — бан 1 день; повторное — срок увеличивается ×2.</p>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">2. ЧЕСТНАЯ ИГРА (АНТИЧИТ)</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Сервер придерживается принципа честной игры. Любые читерские преимущества разрушают экономику и атмосферу.</p>

      <p class="mt-2"><strong>Разрешено:</strong> OptiFine, Sodium, Lithium, мини-карта (без X-Ray), Replay Mod, настройки яркости.</p>

      <p class="mt-2"><strong>Запрещено:</strong> Wurst, Aristois, Baritone, X-Ray (моды и текстуры), авто-кликеры и макросы для PvP, создание лаг-машин и дюп-ферм, DDoS/умышленный вред сервера.</p>

      <p class="mt-3"><strong>Наказание:</strong> за читы и дюпы — бан на 1 месяц без предупреждений; за лаг-машины/вред серверу — первое нарушение 7 дней, повторное или умышленное вредительство — перманентный бан.</p>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">3. ГРИФЕРСТВО И ВОРОВСТВО</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Сервер построен на доверии, но злоупотребления не допускаются.</p>

      <p class="mt-2"><strong>Запрещено:</strong> ломать, портить или изменять чужие постройки без разрешения владельца; воровать из сундуков, печей и хранилищ; использовать чужие фермы без согласия.</p>

      <p class="mt-3"><strong>Наказание:</strong> первое нарушение — бан 3 дня; повторное — 7 дней; систематическое — по решению администрации.</p>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">4. ОБЩЕНИЕ В ЧАТЕ</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Чат — для общения, а не хаоса.</p>

      <p class="mt-2"><strong>Запрещено:</strong> спам, флуд, бессмысленные сообщения, постоянный CAPS LOCK, политические и религиозные холивары.</p>

      <p class="mt-3"><strong>Наказание:</strong> мут от 1 часа; повторное нарушение — мут ×2.</p>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">5. ПОСТРОЙКИ И ЛАНДШАФТ</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Мир сервера — общий. Уважайте внешний вид ландшафта и соседей.</p>

      <p class="mt-2"><strong>Запрещено:</strong> гигантские столбы из грязи, «летающие» деревья, открытая лава, постройки с оскорбительным или непристойным содержимым.</p>

      <p class="mt-2">Оптимизируйте фермы и механизмы, чтобы не создавать лагов. Не стройте ближе <strong>200 блоков</strong> к чужим базам без договорённости.</p>

      <p class="mt-3"><strong>Наказание:</strong> предупреждение → бан от 1 дня; повторное — ×2.</p>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">6. АДМИНИСТРАЦИЯ И МОДЕРАЦИЯ</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Администрация и модерация — для помощи и порядка.</p>

      <p class="mt-2">Не спорьте с модераторами в публичном чате, все жалобы и вопросы оформляйте в тикетах или в личных сообщениях.</p>

      <p class="mt-2"><strong>Запрещено:</strong> выдавать себя за администрацию; требовать предметы, права или телепортацию у модеров.</p>

      <p class="mt-3"><strong>Наказание:</strong> мут или бан от 6 часов; повторное нарушение — ×2.</p>

      <p class="mt-2"><strong>Актуальная администрация:</strong></p>
      <ul class="list-disc ml-5 mt-1 text-sm">
        <li>Тех. админ: Тёма Тема</li>
        <li>Администраторы: Тёма Тема, gyrt46, Василёк, имп хй</li>
      </ul>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">7. БЕЗОПАСНОСТЬ И ВОЗРАСТ</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Контент 18+ (постройки, текст, названия) — запрещён. Рекомендуемый возраст игроков — 16+.</p>
      <p>Решает адекватность, а не лишь цифра в паспорте.</p>
      <p class="mt-3"><strong>Наказание:</strong> бан от 7 дней; повторное — перманентный бан.</p>
    </div>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">8. СИСТЕМА НАКАЗАНИЙ</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Общая схема: <strong>Предупреждение → Мут → Временный бан → Вечный бан</strong>. История наказаний хранится и учитывается при решениях.</p>
      <p class="mt-2">За читы, дюпы и откровенное гриферство — вечный бан без предупреждения.</p>
    </div>
  </details>

  <details class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4 mt-3">
    <summary class="font-bold cursor-pointer">9. ГЛАВНЫЙ ПРИНЦИП</summary>
    <div class="mt-2 text-sm opacity-90">
      <p>Относитесь к другим так, как хотите, чтобы относились к вам.</p>
      <p>Игрок, который знает правила и помогает их соблюдать — ценнейший участник сообщества.</p>
    </div>
  </details>
</section>

<!-- FOOTER -->
<footer class="border-t-4 border-black mt-10 p-6">
  <div class="max-w-6xl mx-auto flex flex-wrap gap-3 justify-center">
    <a href="https://discord.gg/6WDeeJnT" target="_blank"
      class="bg-[var(--accent)] text-black font-bold px-6 py-3 rounded-full border-2 border-black shadow-pop press">
      Discord
    </a>
    <a href="https://tiktok.com/@altaris_server" target="_blank"
      class="border-2 border-black rounded-full px-6 py-3 shadow-pop press">
      TikTok
    </a>
    <a href="https://t.me/altaris_server" target="_blank"
      class="border-2 border-black rounded-full px-6 py-3 shadow-pop press">
      Telegram
    </a>
    <a href="https://t.me/altaris_whitellist" target="_blank"
      class="border-2 border-black rounded-full px-6 py-3 shadow-pop press">
      Заявка
    </a>
  </div>
</footer>

</body>
</html>
