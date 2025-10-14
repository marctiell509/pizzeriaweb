<!DOCTYPE html>
<html lang="it">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>🍕 5IB Pizzeria 5IB - Menu Pizze</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet" />

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    font-family: 'Poppins', sans-serif;
    background: #E1F5FE;
    color: #01579B;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  header {
    background: #0288D1;
    color: white;
    padding: 1.5rem 2rem;
    text-align: center;
    box-shadow: 0 6px 20px rgba(2,136,209,0.4);
    user-select: none;
  }
  header h1 {
    font-weight: 600;
    font-size: 2.2rem;
    letter-spacing: 4px;
    text-shadow: 1px 1px 5px rgba(0,0,0,0.15);
    margin-bottom: 0.3rem;
  }
  header p {
    font-weight: 300;
    font-size: 1rem;
    letter-spacing: 1px;
    font-style: italic;
    text-shadow: 1px 1px 3px rgba(0,0,0,0.1);
  }
  main.menu {
    max-width: 1200px;
    margin: 3rem auto 5rem;
    padding: 0 1rem;
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
    gap: 2.5rem;
  }
  h2.section-title {
    grid-column: 1 / -1;
    color: #0288D1;
    font-weight: 600;
    font-size: 2rem;
    margin-bottom: 1.5rem;
    user-select: none;
  }
  .pizza-card {
    background: #FFFFFF;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(1,87,155,0.12);
    overflow: hidden;
    cursor: pointer;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
  }
  .pizza-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 50px rgba(1,87,155,0.18);
  }
  .pizza-img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    transition: filter 0.3s ease;
    filter: brightness(0.9);
  }
  .pizza-card:hover .pizza-img {
    filter: brightness(1);
  }
  .pizza-content {
    padding: 1.5rem 2rem 2rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .pizza-title {
    color: #0288D1;
    font-weight: 600;
    font-size: 1.5rem;
    margin-bottom: 0.6rem;
    user-select: none;
  }
  .pizza-desc {
    font-size: 1rem;
    color: #0277BD;
    margin-bottom: 1.2rem;
    line-height: 1.4;
    user-select: none;
  }
  .price {
    font-weight: 700;
    font-size: 1.3rem;
    color: #01579B;
    text-align: right;
    user-select: none;
  }
  footer {
    text-align: center;
    padding: 2rem 1rem;
    background: #01579B;
    color: white;
    font-weight: 500;
    font-size: 1rem;
    letter-spacing: 0.08em;
    user-select: none;
    margin-top: auto;
  }
  @media (max-width: 480px) {
    header h1 {
      font-size: 1.8rem;
      letter-spacing: 3px;
    }
    main.menu {
      grid-template-columns: 1fr;
      margin: 2rem auto 4rem;
      padding: 0 1rem;
    }
  }
</style>
</head>
<body>

<header>
  <h1>5IB - Pizzeria</h1>
  <p>Pizza artigianale, fatta con amore dal 1987</p>
</header>

<main class="menu">

  <h2 class="section-title">Pizze Normali</h2>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/margherita.png" alt="Margherita" />
    <div class="pizza-content">
      <h2 class="pizza-title">Margherita</h2>
      <p class="pizza-desc">Pomodoro San Marzano, mozzarella fior di latte, basilico</p>
      <p class="price">€6.50</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/diavola.png" alt="Diavola" />
    <div class="pizza-content">
      <h2 class="pizza-title">Diavola</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, salame piccante calabrese</p>
      <p class="price">€7.50</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/quattroformaggi.png" alt="Quattro Formaggi" />
    <div class="pizza-content">
      <h2 class="pizza-title">Quattro Formaggi</h2>
      <p class="pizza-desc">Mozzarella, gorgonzola, fontina, parmigiano</p>
      <p class="price">€8.00</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/capricciosa.png" alt="Capricciosa" />
    <div class="pizza-content">
      <h2 class="pizza-title">Capricciosa</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, funghi, carciofi, prosciutto cotto, olive</p>
      <p class="price">€8.50</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/vegetariana.png" alt="Vegetariana" />
    <div class="pizza-content">
      <h2 class="pizza-title">Vegetariana</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, zucchine, melanzane, peperoni</p>
      <p class="price">€7.50</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/bufalina.png" alt="Bufalina" />
    <div class="pizza-content">
      <h2 class="pizza-title">Bufalina</h2>
      <p class="pizza-desc">Pomodoro, mozzarella di bufala DOP, basilico fresco</p>
      <p class="price">€9.00</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/tonnocipolla.png" alt="Tonno e Cipolla" />
    <div class="pizza-content">
      <h2 class="pizza-title">Tonno e Cipolla</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, tonno, cipolla rossa</p>
      <p class="price">€7.80</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/prosciuttofunghi.png" alt="Prosciutto e Funghi" />
    <div class="pizza-content">
      <h2 class="pizza-title">Prosciutto e Funghi</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, prosciutto cotto, champignon</p>
      <p class="price">€8.20</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/napoli.png" alt="Napoli" />
    <div class="pizza-content">
      <h2 class="pizza-title">Napoli</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, acciughe, capperi, origano</p>
      <p class="price">€7.70</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/bianca.png" alt="Pizza Bianca" />
    <div class="pizza-content">
      <h2 class="pizza-title">Pizza Bianca</h2>
      <p class="pizza-desc">Mozzarella, patate al forno, rosmarino, olio EVO</p>
      <p class="price">€8.00</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/tartufata.png" alt="Pizza Tartufata" />
    <div class="pizza-content">
      <h2 class="pizza-title">Pizza Tartufata</h2>
      <p class="pizza-desc">Crema di tartufo, mozzarella, funghi porcini</p>
      <p class="price">€10.00</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/pugliese.png" alt="Pizza Pugliese" />
    <div class="pizza-content">
      <h2 class="pizza-title">Pizza Pugliese</h2>
      <p class="pizza-desc">Pomodoro, mozzarella, burrata, pomodorini, rucola</p>
      <p class="price">€9.50</p>
    </div>
  </div>

  <!-- Sezione Pizze Fritte (Ripiene) -->
  <h2 class="section-title">Pizze Fritte (Ripiene)</h2>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/ripienamargherita.png" alt="Fritta Margherita" />
    <div class="pizza-content">
      <h2 class="pizza-title">Fritta Margherita</h2>
      <p class="pizza-desc">Impasto fritto ripieno di mozzarella, pomodoro e basilico</p>
      <p class="price">€7.00</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/calzone.png" alt="Fritta Ripiena" />
    <div class="pizza-content">
      <h2 class="pizza-title">Fritta Ripiena</h2>
      <p class="pizza-desc">Impasto fritto con mozzarella, ricotta, salame e pepe nero</p>
      <p class="price">€8.50</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/ripienasalsiccia.png" alt="Fritta Salsiccia e Friarielli" />
    <div class="pizza-content">
      <h2 class="pizza-title">Fritta Salsiccia e Friarielli</h2>
      <p class="pizza-desc">Impasto fritto con salsiccia, friarielli e provola affumicata</p>
      <p class="price">€9.00</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/cuoppo.png" alt="Fritta Cuoppo" />
    <div class="pizza-content">
      <h2 class="pizza-title">Fritta Cuoppo</h2>
      <p class="pizza-desc">Impasto fritto con mozzarella, prosciutto cotto e ricotta</p>
      <p class="price">€8.80</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/pomobufala.png" alt="Fritta Pomodorini e Bufala" />
    <div class="pizza-content">
      <h2 class="pizza-title">Fritta Pomodorini e Bufala</h2>
      <p class="pizza-desc">Impasto fritto con pomodorini freschi e mozzarella di bufala</p>
      <p class="price">€9.20</p>
    </div>
  </div>

  <div class="pizza-card">
    <img class="pizza-img" src="immagini/spianci.png" alt="Fritta Spinaci e Ricotta" />
    <div class="pizza-content">
      <h2 class="pizza-title">Fritta Spinaci e Ricotta</h2>
      <p class="pizza-desc">Impasto fritto con spinaci freschi e ricotta cremosa</p>
      <p class="price">€8.70</p>
    </div>
  </div>

</main>

<footer>
  &copy; 2025 5IB - Pizzeria (Parisi, Illiano, Lorido, di Costanzo)
</footer>

</body>
</html>

