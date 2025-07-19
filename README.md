<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Club Schiavone</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Orbitron:wght@500&display=swap" rel="stylesheet">
  <style>
    :root {
      --neon-pink: #ff00c8;
      --neon-blue: #00eaff;
      --neon-purple: #9d00ff;
      --bg-black: #0a0a0a;
      --text-white: #ffffff;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background-color: var(--bg-black);
      font-family: 'Montserrat', sans-serif;
      color: var(--text-white);
      overflow-x: hidden;
    }

    header {
      height: 100vh;
      background: linear-gradient(180deg, rgba(10,10,10,0.9), rgba(10,10,10,0.6)), url('https://images.unsplash.com/photo-1587385789090-3725ef8cdb38') center/cover;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
    }

    header h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 3rem;
      color: var(--neon-pink);
      text-shadow: 0 0 10px var(--neon-pink);
    }

    header p {
      font-size: 1.5rem;
      color: var(--neon-blue);
      margin: 1rem 0;
      text-shadow: 0 0 8px var(--neon-blue);
    }

    .cta-button {
      background: var(--neon-purple);
      padding: 1rem 2rem;
      border: none;
      border-radius: 5px;
      font-size: 1rem;
      color: #fff;
      text-shadow: 0 0 5px white;
      cursor: pointer;
      transition: 0.3s;
      box-shadow: 0 0 10px var(--neon-purple), 0 0 20px var(--neon-purple);
    }

    .cta-button:hover {
      box-shadow: 0 0 20px var(--neon-pink), 0 0 30px var(--neon-blue);
    }

    section {
      padding: 4rem 2rem;
      text-align: center;
    }

    .info-section, .pricing-section, .gallery-section {
      background-color: #111;
      margin-bottom: 2rem;
      border-top: 2px solid var(--neon-purple);
    }

    .info-section h2, .pricing-section h2, .gallery-section h2 {
      color: var(--neon-blue);
      font-family: 'Orbitron', sans-serif;
      margin-bottom: 1rem;
      text-shadow: 0 0 8px var(--neon-blue);
    }

    .info-section p {
      font-size: 1.1rem;
      margin: 0.5rem 0;
    }

    .map {
      margin-top: 1rem;
    }

    .pricing-cards {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 2rem;
    }

    .price-box {
      background: #1a1a1a;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 0 10px var(--neon-pink);
      min-width: 200px;
    }

    .price-box h3 {
      color: var(--neon-pink);
      font-size: 1.5rem;
      margin-bottom: 0.5rem;
    }

    .price-box p {
      font-size: 1.2rem;
    }

    .gallery {
      display: flex;
      overflow-x: scroll;
      gap: 1rem;
    }

    .gallery img {
      max-height: 300px;
      border-radius: 10px;
      flex-shrink: 0;
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 2rem;
      text-align: center;
    }

    footer a {
      color: var(--neon-purple);
      margin: 0 0.5rem;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>Vivi la notte vivi il Club</h1>
    <p>Club Schiavone - la notte prende vita</p>
    <button class="cta-button">Prenota il tuo ingresso</button>
  </header>

  <section class="info-section">
    <h2>Info Club</h2>
    <p><strong>Indirizzo:</strong> Via V. Pietro Micca 25, Cisterna di Latina</p>
    <p><strong>Telefono:</strong> 3703343708</p>
    <div class="map">
      <iframe src="https://www.google.com/maps?q=Via+V.+Pietro+Micca+25,+Cisterna+di+Latina&output=embed" width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    </div>
  </section>

  <section class="pricing-section">
    <h2>Prezzi</h2>
    <div class="pricing-cards">
      <div class="price-box">
        <h3>Under 20</h3>
        <p>15€</p>
      </div>
      <div class="price-box">
        <h3>Over 20</h3>
        <p>20€</p>
      </div>
    </div>
  </section>

  <section class="gallery-section">
    <h2>Gallery</h2>
    <div class="gallery">
      <img src="https://images.unsplash.com/photo-1606857521015-7f84f8d0b9a6" alt="DJ set" />
      <img src="https://images.unsplash.com/photo-1509228627159-6452ac295c31" alt="Luci da club" />
      <img src="https://images.unsplash.com/photo-1508672019048-805c876b67e2" alt="Pubblico in festa" />
    </div>
  </section>

  <footer>
    <p>Club Schiavone - Via V. Pietro Micca 25, Cisterna di Latina - Tel: 3703343708</p>
    <p>
      Seguici su:
      <a href="#">Instagram</a>
      <a href="#">Facebook</a>
      <a href="#">TikTok</a>
    </p>
  </footer>
</body>
</html>
