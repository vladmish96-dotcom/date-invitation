<!doctype html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <meta name="theme-color" content="#f8eee8">
  <meta name="description" content="Маленькое приглашение на большое свидание">
  <title>Приглашение для тебя 💌</title>
  <link rel="preload" href="assets/bear.png" as="image">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="ambient" aria-hidden="true">
    <span class="blob blob-one"></span><span class="blob blob-two"></span>
    <div id="petals"></div>
  </div>

  <main class="app-shell">
    <header class="topbar">
      <span class="brand"><span class="brand-heart">♥</span> только для тебя</span>
      <button class="sound-toggle" id="soundToggle" type="button" aria-label="Включить звуки" title="Звуки">
        <span aria-hidden="true">♫</span>
      </button>
    </header>

    <section class="story-card" id="storyCard" aria-live="polite">
      <div class="progress-wrap" id="progressWrap" hidden>
        <div class="progress-label"><span>Наш маленький план</span><span id="progressText">1 из 2</span></div>
        <div class="progress-track"><span id="progressBar"></span></div>
      </div>

      <div class="bear-stage" id="bearStage">
        <div class="bouquet" id="bouquet" aria-hidden="true">
          <span>🌷</span><span>🌸</span><span>🌼</span>
          <i></i>
        </div>
        <div class="bear-wrap">
          <img class="bear" src="assets/bear.png" alt="Добрый белый медвежонок">
          <span class="blink blink-left"></span>
          <span class="blink blink-right"></span>
        </div>
        <div class="mood-sparkles" aria-hidden="true"><i>✦</i><i>♥</i><i>✦</i></div>
      </div>

      <div class="content" id="content"></div>
    </section>

    <p class="tiny-note">сделано с теплом и лёгким волнением</p>
  </main>

  <div class="modal" id="inviteModal" aria-hidden="true">
    <button class="modal-close" id="modalClose" type="button" aria-label="Закрыть">×</button>
    <div class="envelope-scene">
      <div class="envelope" id="envelope">
        <div class="envelope-back"></div>
        <div class="letter">
          <p class="letter-kicker">наше свидание</p>
          <h2>Приглашение</h2>
          <div class="letter-details">
            <div><span>Когда</span><strong data-setting="date">Выбери дату</strong></div>
            <div><span>Во сколько</span><strong data-setting="time">19:00</strong></div>
            <div><span>Где встретимся</span><strong data-setting="place">Скажу чуть позже ✨</strong></div>
          </div>
          <p class="letter-choice" id="letterChoice"></p>
          <p class="letter-footer">Я очень жду нашей встречи <b>♥</b></p>
        </div>
        <div class="envelope-front"></div>
        <div class="envelope-flap"></div>
        <div class="seal">♥</div>
      </div>
      <p class="open-hint" id="openHint">нажми на конверт</p>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
