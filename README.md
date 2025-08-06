<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="White Rose Beauty SPA — премиум салон красоты в Сыктывкаре. Массаж, косметология, маникюр, парикмахерские услуги и многое другое." />
  <meta name="keywords" content="СПА Сыктывкар, салон красоты, массаж, косметология, маникюр, педикюр, окрашивание волос, брови, ресницы, White Rose Beauty SPA" />
  <meta name="author" content="White Rose Beauty SPA" />
  <title>Массаж и СПА — White Rose Beauty SPA</title>
  <link href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Open+Sans&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Open Sans', sans-serif;
      background: #fffafc;
      color: #333;
    }
    header {
      background: linear-gradient(to right, #e23ca5, #5e2dc4);
      color: white;
      padding: 30px;
      text-align: center;
    }
    header img {
      width: 100px;
    }
    .back-btn {
      display: inline-block;
      margin-top: 20px;
      background: #e23ca5;
      color: white;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 5px;
    }
    section {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
    }
    h1, h2 {
      font-family: 'Playfair Display', serif;
      text-align: center;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 15px;
      margin: 30px 0;
    }
    .gallery img {
      width: 100%;
      border-radius: 10px;
    }
    .reviews blockquote {
      background: #fff0f5;
      padding: 20px;
      margin: 20px 0;
      border-left: 4px solid #e23ca5;
      border-radius: 5px;
      font-style: italic;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
    }
    table, th, td {
      border: 1px solid #ccc;
    }
    th, td {
      padding: 12px;
      text-align: left;
    }
    th {
      background-color: #f8d6e4;
    }
  </style>
</head>
<body>
  <header>
    <a href="index.html"><img src="logo.jpg" alt="White Rose Beauty SPA"></a>
    <h1>Массаж и СПА</h1>
    <p>Погрузитесь в мир полного расслабления</p>
  </header>

  <section>
    <h2>Описание процедур</h2>
    <p>Мы предлагаем широкий спектр СПА-процедур: тайский, классический, лимфодренажный массаж, расслабляющие обертывания, ароматерапия, релакс-фитобочка и многое другое. Все процедуры проводятся в уютной атмосфере с использованием профессиональной косметики.</p>

    <h2>Прайс</h2>
    <table>
      <tr><th>Услуга</th><th>Продолжительность</th><th>Цена</th></tr>
      <tr><td>Тайский массаж</td><td>60 мин</td><td>2200 ₽</td></tr>
      <tr><td>Фитобочка с массажем</td><td>45 мин</td><td>1800 ₽</td></tr>
      <tr><td>Обертывание + массаж</td><td>90 мин</td><td>3200 ₽</td></tr>
    </table>

    <h2>Отзывы</h2>
    <div class="reviews">
      <blockquote>«После массажа почувствовала лёгкость во всём теле. Уютно и профессионально!» — Мария</blockquote>
      <blockquote>«Очень понравилась обстановка и мастер. Рекомендую всем, кто хочет перезагрузиться!» — Екатерина</blockquote>
    </div>

    <h2>Фотогалерея</h2>
    <div class="gallery">
      <img src="gallery/spa1.jpg" alt="СПА 1">
      <img src="gallery/spa2.jpg" alt="СПА 2">
      <img src="gallery/spa3.jpg" alt="СПА 3">
    </div>

    <div style="text-align:center">
      <a class="back-btn" href="index.html">← Назад на главную</a>
    </div>
  </section>

  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
  <script>
    AOS.init();
  </script>
</body>
</html>

