<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>White Rose Beauty SPA</title>
  <link href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #fffafc;
      color: #333;
    }
    header {
      background: #f8e6ed;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2em;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      padding: 10px;
      background: #fff0f5;
    }
    nav a {
      text-decoration: none;
      color: #333;
    }
    section {
      padding: 40px 20px;
      max-width: 960px;
      margin: auto;
    }
    h2 {
      text-align: center;
    }
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .service-card {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    }
    .modal {
      display: none;
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0,0,0,0.5);
      justify-content: center;
      align-items: center;
    }
    .modal-content {
      background: white;
      padding: 30px;
      border-radius: 10px;
      width: 90%;
      max-width: 400px;
    }
    .modal-content input,
    .modal-content textarea {
      width: 100%;
      margin-bottom: 15px;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .map {
      height: 300px;
      margin-top: 20px;
    }
    .btn {
      display: inline-block;
      background: #e88fad;
      color: white;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <header>
    <h1>White Rose Beauty SPA</h1>
    <p>SPA-салон в Сыктывкаре</p>
  </header>

  <nav>
    <a href="#services">Услуги</a>
    <a href="#actions">Акции</a>
    <a href="#contacts">Контакты</a>
    <a href="#" onclick="openModal()">Записаться</a>
  </nav>

  <section id="services" data-aos="fade-up">
    <h2>Наши услуги</h2>
    <div class="services-grid">
      <div class="service-card">
        <h3>Массаж и СПА</h3>
        <p>Классический, антистресс, тайский массаж. СПА-программы и фитобочка.</p>
      </div>
      <div class="service-card">
        <h3>Косметология</h3>
        <p>Чистки, пилинги, биоревитализация, RF‑лифтинг, ботокс.</p>
      </div>
      <div class="service-card">
        <h3>Маникюр и педикюр</h3>
        <p>Классический и аппаратный маникюр, педикюр, дизайн ногтей.</p>
      </div>
      <div class="service-card">
        <h3>Парикмахерские услуги</h3>
        <p>Стрижки, окрашивание, укладки, ботокс и уход за волосами.</p>
      </div>
      <div class="service-card">
        <h3>Брови и макияж</h3>
        <p>Перманентный макияж, окрашивание и ламинирование бровей.</p>
      </div>
    </div>
  </section>

  <section id="actions" data-aos="fade-up">
    <h2>Акции</h2>
    <ul>
      <li><strong>Сентябрьская акция:</strong> -15% на СПА-программы!</li>
      <li><strong>Новым клиентам:</strong> скидка 10% на первую услугу</li>
      <li><strong>С днём рождения:</strong> подарок от салона</li>
    </ul>
  </section>

  <section id="contacts" data-aos="fade-up">
    <h2>Контакты</h2>
    <p><strong>Адрес:</strong> Сыктывкар, Интернациональная, 32</p>
    <p><strong>Тел.:</strong> +7 (8212) 446‑199, +7 (904) 101‑18‑88</p>
    <p><strong>ВКонтакте:</strong> <a href="https://vk.com/club166483265" target="_blank">vk.com/club166483265</a></p>
    <div class="map">
      <iframe src="https://yandex.ru/map-widget/v1/?um=constructor%3Ae4b90f80ecf2a418a78972d8a85fc529b85bb0ee0e0d542f8c8f580e870f1f1e&amp;source=constructor" width="100%" height="300" frameborder="0"></iframe>
    </div>
  </section>

  <div class="modal" id="bookingModal">
    <div class="modal-content">
      <h3>Запись на приём</h3>
      <input type="text" placeholder="Ваше имя">
      <input type="tel" placeholder="Телефон">
      <textarea rows="3" placeholder="Комментарий"></textarea>
      <button class="btn" onclick="closeModal()">Отправить</button>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
  <script>
    AOS.init();

    function openModal() {
      document.getElementById('bookingModal').style.display = 'flex';
    }
    function closeModal() {
      document.getElementById('bookingModal').style.display = 'none';
    }
  </script>
</body>
</html>
