<html lang="ru">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1"/>
<title>ALTARIS — Мир без вайпов</title>

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

<!-- GALLERY -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Скриншоты мира</h2>

  <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-4">
    <!-- 12 SCREENSHOTS -->
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
    <div class="aspect-video bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop"></div>
  </div>
</section>

<!-- RULES (ACCORDION) -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Правила сервера</h2>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">Взаимоуважение</summary>
    <p class="mt-2 text-sm opacity-90">
      Будьте вежливы, избегайте токсичности, конфликтов и провокаций.
    </p>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">Честная игра</summary>
    <p class="mt-2 text-sm opacity-90">
      Запрещены читы, дюпы, лаг-машины и любые способы нечестной игры.
    </p>
  </details>

  <details class="mb-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">Гриф и кражи</summary>
    <p class="mt-2 text-sm opacity-90">
      Чужие постройки и ресурсы неприкосновенны без разрешения владельца.
    </p>
  </details>

  <details class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
    <summary class="font-bold cursor-pointer">Территории</summary>
    <p class="mt-2 text-sm opacity-90">
      Свободные земли можно занимать. Регистрация помогает защитить проект и границы.
    </p>
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
