<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>ALTARIS — Полуванильный мир без вайпов</title>

  <!-- Tailwind CDN -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Fonts -->
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
    body{ background:var(--page); color:var(--text); font-family:Inter,system-ui,sans-serif; }

    /* HARD POP PHYSICS */
    .shadow-pop{ box-shadow:4px 4px 0 0 rgba(0,0,0,1); }
    .press:hover{ transform:translate(2px,2px); box-shadow:none; transition:.08s linear; }

    /* focus */
    :focus-visible{ outline:4px solid black; outline-offset:2px; }
  </style>
</head>

<body class="min-h-screen">

<!-- HEADER -->
<header class="max-w-6xl mx-auto p-4 flex items-center justify-between border-b-4 border-black">
  <div class="flex items-center gap-3 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3">
    <div class="w-10 h-10 rounded-xl bg-[var(--brand)] border-2 border-black flex items-center justify-center text-black font-extrabold">
      A
    </div>
    <div>
      <div class="text-xl font-bold lowercase">altaris</div>
      <div class="text-sm opacity-90">полуванильный мир</div>
    </div>
  </div>

  <div class="flex items-center gap-3">
    <div class="hidden sm:block bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop px-4 py-2">
      <div class="text-xs">account</div>
      <div class="font-bold">player_017</div>
    </div>

    <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 flex items-center gap-3">
      <span class="font-bold" id="balance">120 ⍟</span>
      <button onclick="topup()" class="bg-[var(--accent)] text-black font-bold px-3 py-1 rounded-full border-2 border-black shadow-pop press text-sm">
        + topup
      </button>
    </div>
  </div>
</header>

<!-- HERO -->
<section class="max-w-6xl mx-auto p-6 mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
  <h1 class="text-4xl font-extrabold mb-3">ALTARIS</h1>
  <p class="text-lg max-w-2xl">
    Полуванильный мир без вайпов. Здесь история не обнуляется, а игроки действительно оставляют след.
  </p>
  <p class="mt-2 opacity-90 max-w-2xl">
    Долговечность, честная экономика и события, которые имеют последствия.
  </p>

  <div class="mt-6 flex flex-wrap gap-3">
    <button class="bg-[var(--accent)] text-black font-bold px-6 py-3 rounded-full border-2 border-black shadow-pop press">
      Присоединиться
    </button>
    <button class="bg-transparent text-[var(--text)] font-bold px-6 py-3 rounded-full border-2 border-black shadow-pop press">
      Читать лор
    </button>
  </div>
</section>

<!-- FEATURES -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Почему ALTARIS</h2>

  <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
      <h3 class="font-bold mb-2">Жители 2.0</h3>
      <ul class="text-sm opacity-90">
        <li>• живые NPC</li>
        <li>• торговля и роли</li>
      </ul>
    </div>

    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
      <h3 class="font-bold mb-2">Комфортные твики</h3>
      <ul class="text-sm opacity-90">
        <li>• QoL без казуала</li>
        <li>• честный баланс</li>
      </ul>
    </div>

    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
      <h3 class="font-bold mb-2">Оптимизация</h3>
      <ul class="text-sm opacity-90">
        <li>• стабильный TPS</li>
        <li>• быстрые зоны</li>
      </ul>
    </div>

    <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
      <h3 class="font-bold mb-2">Честная экономика</h3>
      <ul class="text-sm opacity-90">
        <li>• без Pay-to-Win</li>
        <li>• всё через игру</li>
      </ul>
    </div>
  </div>
</section>

<!-- TERRITORIES -->
<section class="max-w-6xl mx-auto p-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
  <div class="flex flex-col md:flex-row md:items-center md:justify-between gap-4">
    <div>
      <h2 class="text-2xl font-bold">Территории</h2>
      <p class="opacity-90 max-w-xl">
        Регистрируй земли, влияй на мир и участвуй в событиях, которые меняют карту.
      </p>
    </div>

    <button onclick="openModal()" class="bg-[var(--accent)] text-black font-bold px-5 py-3 rounded-full border-2 border-black shadow-pop press">
      Зарегистрировать территорию
    </button>
  </div>
</section>

<!-- LORE -->
<section class="max-w-6xl mx-auto p-6">
  <h2 class="text-2xl font-bold mb-4">Лор и события</h2>

  <div class="space-y-3">
    <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
      <div class="font-bold">Основание Алтариса</div>
      <div class="text-sm opacity-90">
        Мир был создан как убежище от бесконечных вайпов.
      </div>
    </div>

    <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
      <div class="font-bold">Охота за яйцом Эндер-дракона</div>
      <div class="text-sm opacity-90">
        Игроки поборются за уникальный артефакт.
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer class="border-t-4 border-black mt-10 p-6">
  <div class="max-w-6xl mx-auto flex flex-col md:flex-row gap-4 justify-between">
    <div>
      <div class="font-bold text-lg">ALTARIS</div>
      <div class="text-sm opacity-90">
        Полуванильный мир без вайпов. История, которую пишут игроки.
      </div>
    </div>

    <div class="flex gap-3">
      <a class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Discord</a>
      <a class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Wiki</a>
      <a class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Rules</a>
    </div>
  </div>
</footer>

<!-- MODAL -->
<div id="modal" class="fixed inset-0 hidden items-center justify-center z-50">
  <div class="absolute inset-0 bg-black/60" onclick="closeModal()"></div>

  <div class="relative bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-6 w-full max-w-md">
    <h3 class="text-xl font-bold mb-3">Регистрация территории</h3>
    <input id="territory" placeholder="Название территории"
      class="w-full bg-white text-black border-4 border-black rounded-xl px-4 py-2 mb-3 focus:outline-none">

    <div class="flex justify-end gap-3">
      <button onclick="closeModal()" class="border-2 border-black rounded-full px-4 py-2 shadow-pop press">
        Отмена
      </button>
      <button onclick="registerTerritory()" class="bg-[var(--accent)] text-black font-bold px-4 py-2 rounded-full border-2 border-black shadow-pop press">
        Зарегистрировать
      </button>
    </div>
  </div>
</div>

<script>
  let balance = 120;

  function topup(){
    balance += 50;
    document.getElementById("balance").innerText = balance + " ⍟";
    alert("Баланс пополнен (демо)");
  }

  function openModal(){
    document.getElementById("modal").classList.remove("hidden");
    document.getElementById("modal").classList.add("flex");
  }

  function closeModal(){
    document.getElementById("modal").classList.add("hidden");
    document.getElementById("modal").classList.remove("flex");
  }

  function registerTerritory(){
    const name = document.getElementById("territory").value.trim();
    if(name.length < 3){
      alert("Название слишком короткое");
      return;
    }
    alert("Территория «" + name + "» зарегистрирована (демо)");
    closeModal();
  }
</script>

</body>
</html>
