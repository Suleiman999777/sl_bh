# sl_bh 
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Сулейман Legend's — Империя Барвихи</title>
  <link href="https://fonts.googleapis.com/css2?family=Russo+One&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: 'Russo One', sans-serif;
      background: #0d0d0d;
      color: #fff;
      scroll-behavior: smooth;
    }
    header {
      background: linear-gradient(to right, #c49b2e, #8b6500);
      padding: 2rem 1rem 3rem 1rem;
      text-align: center;
      animation: fadeIn 2s ease-in-out;
    }
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: #111;
      z-index: 1000;
      display: flex;
      justify-content: center;
      padding: 0.5rem;
    }
    nav a {
      color: #ffa500;
      margin: 0 1rem;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #ffcc66;
    }
    section {
      padding: 1.5rem 1rem;
      animation: fadeInUp 1s ease-in-out;
    }
    .section-title {
      font-size: 1.5rem;
      margin-bottom: 1rem;
      color: #ffd700;
    }
    .card {
      background: #1a1a1a;
      padding: 1.2rem;
      border-radius: 10px;
      margin-bottom: 1.5rem;
      box-shadow: 0 0 10px rgba(255, 215, 0, 0.2);
    }
    .highlight {
      color: #ffa500;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 1rem;
    }
    .gallery img, .stats img {
      width: 100%;
      border-radius: 10px;
      border: 2px solid #333;
    }
    .youtube {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    .youtube iframe {
      width: 100%;
      height: 200px;
      border-radius: 10px;
    }
    .reviews {
      display: grid;
      gap: 1rem;
    }
    .review {
      background: #262626;
      border-left: 4px solid #ffa500;
      padding: 1rem;
      border-radius: 8px;
    }
    .btn {
      display: inline-block;
      background-color: #ffa500;
      color: #000;
      padding: 0.75rem 1.5rem;
      border-radius: 8px;
      font-weight: bold;
      text-align: center;
      margin-top: 1rem;
      text-decoration: none;
      transition: all 0.3s ease;
    }
    .btn:hover {
      background-color: #ffcc66;
      transform: scale(1.05);
      box-shadow: 0 0 10px #ffa500;
    }
    .poll {
      background: #1a1a1a;
      padding: 1rem;
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
    }
    .poll label {
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .fixed-play {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #ffcc00;
      color: #000;
      padding: 0.8rem 1.4rem;
      font-size: 1rem;
      font-weight: bold;
      border-radius: 12px;
      text-decoration: none;
      box-shadow: 0 0 10px rgba(255,204,0,0.7);
      z-index: 999;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .fixed-play:hover {
      transform: scale(1.1);
      box-shadow: 0 0 15px rgba(255,204,0,1);
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #111;
      font-size: 0.9rem;
      color: #777;
    }
    a {
      color: #ffa500;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#">Главная</a>
    <a href="#Отзывы">Отзывы</a>
    <a href="#Галерея">Галерея</a>
    <a href="#Контакты">Контакты</a>
  </nav>

  <header>
    <h1>Сулейман Legend's</h1>
    <p>Официальный сайт Империи Барвихи</p>
  </header>

  <!-- контент разделов, тот же, без изменений -->

  <a href="https://t.me/sl_bhrp" target="_blank" class="fixed-play" onclick="playClick();">Играть сейчас</a>
  <audio id="click-sound" src="https://cdn.pixabay.com/audio/2022/03/15/audio_643fa5f60c.mp3"></audio>

  <footer>
    © 2025 Сулейман Legend's | Все права защищены
  </footer>

  <script>
    function playClick() {
      const snd = document.getElementById("click-sound");
      snd.volume = 0.4;
      snd.play();
      if (navigator.vibrate) navigator.vibrate(100);
    }
  </script>
</body>
</html>
