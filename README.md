<html lang="ru">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>ALTARIS — Полуванильный мир без вайпов</title>

  <!-- Tailwind CDN -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Fonts -->
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
    html,body{ height:100%; }
    body{
      background:var(--page); color:var(--text);
      font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    /* Pop physics */
    .shadow-pop{ box-shadow:4px 4px 0 0 rgba(0,0,0,1); }
    .press:hover{ transform: translate(2px,2px); box-shadow:none; transition: .08s linear; }

    /* focus visible */
    :focus-visible { outline:4px solid black; outline-offset:2px; }

    /* accordion animation */
    .acc-content {
      max-height: 0;
      overflow: hidden;
      transition: max-height 240ms ease;
    }
    .acc-open .acc-content { max-height: 1200px; }

    /* gallery */
    .thumb { cursor: pointer; }
    .lightbox { background: rgba(0,0,0,0.8); }

    /* small helpers */
    .rounded-ctrl { border-radius: 1rem; } /* big rounding */
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

    <nav class="flex items-center gap-3">
      <a href="#features" class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Фишки</a>
      <a href="#news" class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Лента</a>
      <a href="#rules" class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Правила</a>
      <a href="#gallery" class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press">Скриншоты</a>
    </nav>
  </header>

  <!-- HERO -->
  <section class="max-w-6xl mx-auto p-6 mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
    <div class="md:flex md:justify-between md:items-center gap-6">
      <div class="max-w-2xl">
        <h1 class="text-4xl font-extrabold mb-3">ALTARIS</h1>
        <p class="text-lg mb-2">
          Полуванильный мир — без вайпов. Здесь каждая постройка имеет значение, а история — не стирается.
        </p>
        <p class="opacity-90 mb-4">
          «Максимум ванильного опыта — минимум вмешательства.»
        </p>

        <div class="flex gap-3 flex-wrap">
          <a href="https://discord.gg/6WDeeJnT" target="_blank" class="bg-[var(--accent)] text-black font-bold px-6 py-3 rounded-full border-2 border-black shadow-pop press">Discord (рекомендуем)</a>
          <a href="#news" class="bg-transparent text-[var(--text)] font-bold px-6 py-3 rounded-full border-2 border-black shadow-pop press">Лента новостей</a>
        </div>
      </div>

      <div class="mt-6 md:mt-0 w-full md:w-80">
        <div class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4">
          <div class="font-bold">Статус мира</div>
          <div class="mt-2 text-sm opacity-90">Мир: полуваниль · без вайпов</div>
          <div class="mt-2 text-sm opacity-90">События: новости сохраняются</div>
        </div>
      </div>
    </div>
  </section>

  <!-- FEATURES (отдельно) -->
  <section id="features" class="max-w-6xl mx-auto p-6 mt-6">
    <h2 class="text-2xl font-bold mb-4">Плюшки (геймплей)</h2>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
        <h3 class="font-bold mb-2">Жители 2.0</h3>
        <p class="text-sm opacity-90">Оптимизированные NPC, гибкие трейды, роли и задания.</p>
      </article>

      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
        <h3 class="font-bold mb-2">Комфортные твики</h3>
        <p class="text-sm opacity-90">QoL-улучшения без преимущества в балансе.</p>
      </article>

      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
        <h3 class="font-bold mb-2">Оптимизация</h3>
        <p class="text-sm opacity-90">Стабильная работа сервера и баланс ресурсов.</p>
      </article>

      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-5 press">
        <h3 class="font-bold mb-2">Честная экономика</h3>
        <p class="text-sm opacity-90">Ресурсы добываются в игре — без P2W.</p>
      </article>
    </div>

    <div class="mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-4">
      <h4 class="font-bold mb-2">Формат и философия</h4>
      <p class="text-sm opacity-90">
        Максимум ванильного опыта — минимум вмешательства. Для долгой игры, масштабных построек и историй, которые не стираются.
      </p>
    </div>
  </section>

  <!-- NEWS FEED -->
  <section id="news" class="max-w-6xl mx-auto p-6 mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
    <div class="flex items-center justify-between">
      <h2 class="text-2xl font-bold">Лента новостей</h2>
      <span class="text-sm opacity-90">Последние события мира</span>
    </div>

    <div class="mt-4 space-y-3">
      <!-- News item 1: egg stolen -->
      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press" role="article" aria-label="Новость: яйцо дракона украдено">
        <div class="flex items-start justify-between">
          <div>
            <div class="font-bold">⚠️ Яйцо дракона украдено</div>
            <div class="text-sm opacity-90">Сегодня — игроки нашли, что яйцо было вынесено из Храма. Расследование продолжается.</div>
            <div class="mt-2 text-xs opacity-80">Дата: <strong id="news-date-1"></strong></div>
          </div>
          <div class="text-sm">
            <button class="bg-[var(--accent)] border-2 border-black rounded-full px-3 py-1 shadow-pop press" onclick="alert('Подписка на обновления (демо)')">Следить</button>
          </div>
        </div>
      </article>

      <!-- News item 2 -->
      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press">
        <div class="font-bold">🔔 Анонс: новая охота</div>
        <div class="text-sm opacity-90">Через 3 дня стартует ивент — охота за древним артефактом. Победители получат уникальные таблички.</div>
        <div class="mt-2 text-xs opacity-80">Дата: <strong id="news-date-2"></strong></div>
      </article>

      <!-- News item 3 -->
      <article class="bg-[var(--surface2)] border-2 border-black rounded-2xl shadow-pop p-4 press">
        <div class="font-bold">📢 Рынок открыт</div>
        <div class="text-sm opacity-90">Новый торговый рынок на Порту: NPC-поставщики и место для обмена между игроками.</div>
        <div class="mt-2 text-xs opacity-80">Дата: <strong id="news-date-3"></strong></div>
      </article>
    </div>
  </section>

  <!-- RULES as Accordion -->
  <section id="rules" class="max-w-6xl mx-auto p-6 mt-6">
    <h2 class="text-2xl font-bold mb-4">Правила сервера</h2>

    <div class="space-y-3">
      <!-- 5. Buildings and Landscape -->
      <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3 acc" id="acc-build">
        <button class="w-full text-left flex items-center justify-between p-3 rounded-2xl acc-btn" aria-expanded="false">
          <div>
            <div class="font-bold">📝 5. ПОСТРОЙКИ И ЛАНДШАФТ</div>
            <div class="text-sm opacity-80">Уважайте общий вид мира. Оптимизируйте фермы. Не стройте близко к чужим базам (200 блоков).</div>
          </div>
          <div class="text-2xl">+</div>
        </button>

        <div class="acc-content mt-2 p-3 bg-[var(--surface2)] border-2 border-black rounded-2xl">
          <p><strong>Уважайте общий вид мира.</strong></p>
          <p class="mt-2">❌ Гигантские столбы из грязи, "летающие" деревья, открытая лава. ❌ Запрещены постройки с оскорблениями или непристойностями.</p>
          <p class="mt-2"><strong>Оптимизируйте</strong> фермы/базы, чтобы не создавать лагов.</p>
          <p class="mt-2"><strong>Не стройте близко</strong> к чужим базам без договорённости — рекомендуем минимум <strong>200 блоков</strong>.</p>
          <p class="mt-2"><strong>Нарушение:</strong> Предупреждение → бан 1 день. Повторное ×2.</p>
        </div>
      </div>

      <!-- 6. Administration -->
      <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3 acc" id="acc-admin">
        <button class="w-full text-left flex items-center justify-between p-3 rounded-2xl acc-btn" aria-expanded="false">
          <div>
            <div class="font-bold">👨‍💼 6. АДМИНИСТРАЦИЯ И МОДЕРАЦИЯ</div>
            <div class="text-sm opacity-80">Админы — помощники. Вопросы в тикеты, пожалуйста.</div>
          </div>
          <div class="text-2xl">+</div>
        </button>

        <div class="acc-content mt-2 p-3 bg-[var(--surface2)] border-2 border-black rounded-2xl">
          <p><strong>Администраторы и модераторы — помощники, а не слуги.</strong></p>
          <p class="mt-2">Не спорьте с решением модератора в публичном чате — решаем в тикетах или ЛС.</p>
          <p class="mt-2"><strong>Запрещено:</strong> просить у админов предметы/права/телепортацию; выдавать себя за админа.</p>
          <p class="mt-2"><strong>Нарушение:</strong> Мут/бан от 6 часов. Повторное ×2.</p>

          <div class="mt-3">
            <div class="font-bold">Актуальный список администрации:</div>
            <div class="text-sm mt-1">Тех. админ: &lt;@630073415180484629&gt;</div>
            <div class="text-sm">Администраторы: &lt;@630073415180484629&gt;, &lt;@974309446002040852&gt;, &lt;@822427874002337793&gt;, &lt;@803351990683697182&gt;</div>
          </div>
        </div>
      </div>

      <!-- 7. Safety and Age -->
      <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3 acc" id="acc-age">
        <button class="w-full text-left flex items-center justify-between p-3 rounded-2xl acc-btn" aria-expanded="false">
          <div>
            <div class="font-bold">🔞 7. БЕЗОПАСНОСТЬ И ВОЗРАСТ</div>
            <div class="text-sm opacity-80">Контент 18+ запрещён. Рекомендуемый возраст — 16+</div>
          </div>
          <div class="text-2xl">+</div>
        </button>

        <div class="acc-content mt-2 p-3 bg-[var(--surface2)] border-2 border-black rounded-2xl">
          <p>Контент 18+ (текст, постройки, названия) — запрещен. Рекомендуемый возраст игроков — 16+.</p>
          <p class="mt-2">Всё решает адекватность, а не цифра в паспорте.</p>
          <p class="mt-2"><strong>Нарушение:</strong> Бан от 7 дней. Повторное — вечный.</p>
        </div>
      </div>

      <!-- System of punishment -->
      <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3 acc" id="acc-punish">
        <button class="w-full text-left flex items-center justify-between p-3 rounded-2xl acc-btn" aria-expanded="false">
          <div>
            <div class="font-bold">⚖️ СИСТЕМА НАКАЗАНИЙ</div>
            <div class="text-sm opacity-80">Предупреждение → Мут → Бан → Вечный бан</div>
          </div>
          <div class="text-2xl">+</div>
        </button>

        <div class="acc-content mt-2 p-3 bg-[var(--surface2)] border-2 border-black rounded-2xl">
          <p>Нарушение правил влечёт последствия. За читы/дюпы/гриферство — вечный бан без предупреждения.</p>
          <p class="mt-2">История наказаний хранится; системные нарушения ведут к ужесточению санкций.</p>
        </div>
      </div>

      <!-- PRINCIPLE -->
      <div class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop p-3 acc" id="acc-principle">
        <button class="w-full text-left flex items-center justify-between p-3 rounded-2xl acc-btn" aria-expanded="false">
          <div>
            <div class="font-bold">💎 ГЛАВНЫЙ ПРИНЦИП</div>
            <div class="text-sm opacity-80">Относись к другим так, как хочешь, чтобы относились к тебе.</div>
          </div>
          <div class="text-2xl">+</div>
        </button>

        <div class="acc-content mt-2 p-3 bg-[var(--surface2)] border-2 border-black rounded-2xl">
          <p>Игрок, который знает правила и помогает их соблюдать — ценнейший игрок нашего сервера!</p>

          <div class="mt-3">
            <h4 class="font-bold">🏡 ТЕРРИТОРИИ</h4>
            <p class="text-sm opacity-90 mt-1">Занимайте свободную территорию, если не мешаете соседям. Границы — забор/таблички/координаты.</p>

            <h4 class="font-bold mt-3">📜 ПРАВИЛА ТЕРРИТОРИИ</h4>
            <p class="text-sm opacity-90 mt-1">Правила территории не должны противоречить основным правилам. Регистрация — не приват навсегда.</p>

            <h4 class="font-bold mt-3">🧱 ОГРАНИЧЕНИЯ</h4>
            <p class="text-sm opacity-90 mt-1">Запрещены постройки, мешающие навигации, порча ландшафта, фермы, создающие лаги.</p>

            <h4 class="font-bold mt-3">🚫 БЛЭКЛИСТ</h4>
            <p class="text-sm opacity-90 mt-1">Можно внести до 7 игроков. Администрация может отменить при злоупотреблениях.</p>

            <h4 class="font-bold mt-3">⏳ НЕАКТИВНОСТЬ</h4>
            <p class="text-sm opacity-90 mt-1">Территории в 1–2 км от спавна: при неактивности 60 дней статус может быть пересмотрен.</p>

            <h4 class="font-bold mt-3">📝 ЗАЧЕМ РЕГИСТРАЦИЯ?</h4>
            <p class="text-sm opacity-90 mt-1">Позволяет закрепить территорию, зафиксировать границы и правила, получить поддержку администрации.</p>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- CENTRAL SCREENSHOT PANEL -->
  <section id="gallery" class="max-w-6xl mx-auto p-6 mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
    <h2 class="text-2xl font-bold mb-4 text-center">Скриншоты мира</h2>

    <div class="grid grid-cols-2 sm:grid-cols-4 gap-3">
      <!-- thumbnails (Unsplash placeholders) -->
      <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?w=800&q=60" alt="скрин 1" class="thumb object-cover w-full h-40 rounded-2xl border-2 border-black shadow-pop" tabindex="0" onclick="openLightbox(this.src)" onkeypress="if(event.key==='Enter')openLightbox(this.src)">

      <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?w=800&q=60" alt="скрин 2" class="thumb object-cover w-full h-40 rounded-2xl border-2 border-black shadow-pop" tabindex="0" onclick="openLightbox(this.src)" onkeypress="if(event.key==='Enter')openLightbox(this.src)">

      <img src="https://images.unsplash.com/photo-1496307042754-b4aa456c4a2d?w=800&q=60" alt="скрин 3" class="thumb object-cover w-full h-40 rounded-2xl border-2 border-black shadow-pop" tabindex="0" onclick="openLightbox(this.src)" onkeypress="if(event.key==='Enter')openLightbox(this.src)">

      <img src="https://images.unsplash.com/photo-1470770903676-69b98201ea1c?w=800&q=60" alt="скрин 4" class="thumb object-cover w-full h-40 rounded-2xl border-2 border-black shadow-pop" tabindex="0" onclick="openLightbox(this.src)" onkeypress="if(event.key==='Enter')openLightbox(this.src)">
    </div>

    <!-- Lightbox -->
    <div id="lightbox" class="fixed inset-0 hidden items-center justify-center z-50">
      <div class="absolute inset-0 lightbox" onclick="closeLightbox()"></div>
      <div class="relative max-w-4xl max-h-[90vh] p-4">
        <button onclick="closeLightbox()" class="absolute right-4 top-4 bg-[var(--surface)] border-2 border-black rounded-full p-2 shadow-pop">✕</button>
        <img id="lightbox-img" src="" alt="скриншот" class="max-h-[85vh] rounded-2xl border-2 border-black shadow-pop">
      </div>
    </div>
  </section>

  <!-- LORE (обновлённый: яйцо украдено упомянуто в новостях) -->
  <section class="max-w-6xl mx-auto p-6 mt-6 bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop">
    <h2 class="text-2xl font-bold mb-3">О сервере</h2>

    <p class="opacity-90 mb-2">
      ALTARIS — полуванильный мир без вайпов. Здесь нет вайпов: каждая постройка, дорога и город остаются частью истории.
    </p>

    <p class="opacity-90 mb-2">
      Мир развивается естественно. Игроки формируют лор и события — и недавно одно из таких событий (яйцо дракона) стало предметом расследования.
    </p>

    <div class="mt-3 bg-[var(--surface2)] border-2 border-black rounded-2xl p-4 shadow-pop">
      <div class="font-bold">Контакты и сообщества</div>
      <ul class="mt-2 text-sm">
        <li>Discord (рекомендуем): <a class="underline" href="https://discord.gg/6WDeeJnT" target="_blank">https://discord.gg/6WDeeJnT</a></li>
        <li>TikTok: <a class="underline" href="https://tiktok.com/@altaris_server" target="_blank">tiktok.com/@altaris_server</a></li>
        <li>Telegram (важные новости): <a class="underline" href="https://t.me/altaris_server" target="_blank">https://t.me/altaris_server</a></li>
        <li>Telegram (заявки): <a class="underline" href="https://t.me/altaris_whitellist" target="_blank">https://t.me/altaris_whitellist</a></li>
      </ul>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="border-t-4 border-black mt-10 p-6">
    <div class="max-w-6xl mx-auto flex flex-col md:flex-row gap-4 justify-between">
      <div>
        <div class="font-bold text-lg">ALTARIS</div>
        <div class="text-sm opacity-90">Полуванильный мир без вайпов — история, которую пишут игроки.</div>
      </div>

      <div class="flex gap-3">
        <a class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press" href="https://discord.gg/6WDeeJnT" target="_blank">Discord</a>
        <a class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press" href="https://t.me/altaris_server" target="_blank">Telegram</a>
        <a class="bg-[var(--surface)] border-2 border-black rounded-2xl shadow-pop px-4 py-2 press" href="https://tiktok.com/@altaris_server" target="_blank">TikTok</a>
      </div>
    </div>
  </footer>

<script>
  // set current dates in news
  const now = new Date();
  function fmt(d){ return d.toLocaleString('ru-RU', { day: '2-digit', month: 'short', year: 'numeric' }); }
  document.getElementById('news-date-1').innerText = fmt(now);
  const tomorrow = new Date(now.getTime() + 24*3600*1000);
  document.getElementById('news-date-2').innerText = fmt(tomorrow);
  document.getElementById('news-date-3').innerText = fmt(new Date(now.getTime() - 2*24*3600*1000));

  // Accordion behavior (keyboard accessible)
  document.querySelectorAll('.acc').forEach(acc => {
    const btn = acc.querySelector('.acc-btn');
    const content = acc.querySelector('.acc-content');
    btn.addEventListener('click', () => {
      const open = btn.getAttribute('aria-expanded') === 'true';
      btn.setAttribute('aria-expanded', String(!open));
      acc.classList.toggle('acc-open', !open);
      btn.querySelector('div:last-child')?.classList.toggle('rot', !open);
      // update +/-
      btn.querySelector('.text-2xl').innerText = open ? '+' : '−';
    });
    btn.addEventListener('keydown', (e) => {
      if(e.key === 'Enter' || e.key === ' ') { e.preventDefault(); btn.click(); }
    });
  });

  // Lightbox
  function openLightbox(src){
    const lb = document.getElementById('lightbox');
    const img = document.getElementById('lightbox-img');
    img.src = src;
    lb.classList.remove('hidden');
    lb.classList.add('flex');
    img.focus();
  }
  function closeLightbox(){
    const lb = document.getElementById('lightbox');
    lb.classList.add('hidden');
    lb.classList.remove('flex');
    document.activeElement?.blur();
  }
  document.addEventListener('keydown', (e) => { if(e.key === 'Escape') closeLightbox(); });

  // small accessibility: make thumbnails keyboard-focusable
  document.querySelectorAll('.thumb').forEach(t => t.setAttribute('tabindex','0'));
</script>

</body>
</html>
