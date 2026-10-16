
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GoalFlash | Futbol olami</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #080d0a;
      color: white;
    }
    header {
      background: #101a13;
      padding: 20px 16px;
      border-bottom: 2px solid #27e66b;
    }
    .logo { font-size: 27px; font-weight: 900; }
    .logo span { color: #27e66b; }
    header p { color: #a9b8ad; margin-bottom: 0; }
    nav {
      display: flex;
      gap: 20px;
      padding: 14px 16px;
      overflow-x: auto;
      background: #0c120e;
    }
    nav a { color: white; text-decoration: none; white-space: nowrap; }
    nav a:first-child { color: #27e66b; }
    main { padding: 16px; max-width: 850px; margin: auto; }
    .hero {
      background: linear-gradient(135deg, #163c24, #101713);
      border: 1px solid #276b3e;
      padding: 24px 18px;
      border-radius: 16px;
      margin-bottom: 25px;
    }
    .hero h1 { font-size: 30px; margin: 8px 0; }
    .green { color: #27e66b; }
    .tag {
      color: #27e66b;
      font-size: 12px;
      font-weight: bold;
      letter-spacing: 2px;
    }
    h2 { font-size: 21px; }
    .match, .news {
      background: #111914;
      border: 1px solid #25352a;
      border-radius: 12px;
      padding: 16px;
      margin: 12px 0;
    }
    .match { display: flex; justify-content: space-between; align-items: center; gap: 8px; }
    .teams { font-weight: bold; line-height: 1.8; }
    .score { font-size: 23px; font-weight: bold; color: #27e66b; }
    .status { color: #a8b6ac; font-size: 12px; text-align: right; }
    .news h3 { margin: 8px 0; }
    .news p { color: #a9b8ad; line-height: 1.5; }
    .label { color: #27e66b; font-size: 12px; }
    footer {
      text-align: center;
      padding: 25px;
      color: #829187;
      border-top: 1px solid #25352a;
      margin-top: 30px;
    }
    button {
      background: #27e66b; color: #061009;
      border: 0; border-radius: 8px;
      padding: 12px 16px; font-weight: bold;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">GOAL<span>FLASH</span> ⚽</div>
    <p>Futbol olamidagi barcha yangiliklar bir joyda</p>
  </header>

  <nav>
    <a href="#live">Jonli hisoblar</a>
    <a href="#matches">O‘yinlar</a>
    <a href="#news">Yangiliklar</a>
  </nav>

  <main>
    <section class="hero">
      <div class="tag">FUTBOL • TEZKOR • ISHONCHLI</div>
      <h1>Futbol dunyosi <span class="green">shu yerda!</span></h1>
      <p>Sevimli jamoang natijalari va futbol yangiliklarini kuzat.</p>
      <button onclick="document.querySelector('#matches').scrollIntoView({behavior:'smooth'})">
        O‘yinlarni ko‘r ↓
      </button>
    </section>

    <section id="live">
      <h2>🟢 Jonli hisoblar</h2>
      <p id="notice" style="color:#a9b8ad;font-size:13px">
        Hozircha namuna hisoblar. Haqiqiy natijalar uchun API ulash kerak.
      </p>
      <div id="scores">
        <div class="match">
          <div class="teams">Real Madrid<br>Barcelona</div>
          <div class="score">VS</div>
          <div class="status">El Clásico<br>Namuna</div>
        </div>
        <div class="match">
          <div class="teams">Manchester City<br>Liverpool</div>
          <div class="score">VS</div>
          <div class="status">Premier League<br>Namuna</div>
        </div>
      </div>
    </section>

    <section id="matches">
      <h2>📅 Bugungi o‘yinlar</h2>
      <div class="match">
        <div class="teams">⚽ Jamoalar ro‘yxati</div>
        <div class="status">Jadval API ulangandan keyin yangilanadi</div>
      </div>
    </section>

    <section id="news">
      <h2>📰 Futbol yangiliklari</h2>
      <article class="news">
        <div class="label">YANGILIKLAR</div>
        <h3>Futbol olamidagi eng so‘nggi xabarlar</h3>
        <p>Bu bo‘limga haqiqiy yangiliklarni chiqarish uchun ishonchli yangiliklar manbasi yoki API ulaymiz.</p>
      </article>
    </section>
  </main>

  <footer>
    © 2026 GoalFlash — Futbol muxlislari uchun 💚
  </footer>
</body>
</html>
