<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="White Rose Beauty SPA — премиум салон красоты в Сыктывкаре. Массаж, косметология, маникюр, парикмахерские услуги и многое другое." />
  <meta name="keywords" content="СПА Сыктывкар, салон красоты, массаж, косметология, маникюр, педикюр, окрашивание волос, брови, ресницы, White Rose Beauty SPA" />
  <meta name="author" content="White Rose Beauty SPA" />
  <title>White Rose Beauty SPA — Салон красоты в Сыктывкаре</title>
  <link href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
  <style>
    /* Базовые стили */
    body {
      margin: 0;
      font-family: 'Open Sans', sans-serif;
      background: #fffafc;
      color: #333;
      line-height: 1.6;
    }
    
    /* Навигация */
    nav {
      background: linear-gradient(to right, #e23ca5, #5e2dc4);
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    
    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0 20px;
    }
    
    .logo {
      display: flex;
      align-items: center;
    }
    
    .logo img {
      height: 50px;
      border-radius: 50%;
      margin-right: 10px;
    }
    
    .logo span {
      color: white;
      font-weight: 600;
      font-size: 1.2rem;
    }
    
    .nav-links {
      display: flex;
      list-style: none;
      margin: 0;
      padding: 0;
    }
    
    .nav-links li {
      margin-left: 25px;
    }
    
    .nav-links a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      transition: all 0.3s ease;
      padding: 5px 10px;
      border-radius: 4px;
    }
    
    .nav-links a:hover {
      background: rgba(255,255,255,0.2);
    }
    
    /* Мобильное меню */
    .menu-toggle {
      display: none;
      flex-direction: column;
      justify-content: space-between;
      width: 30px;
      height: 21px;
      cursor: pointer;
    }
    
    .menu-toggle span {
      height: 3px;
      width: 100%;
      background: white;
      border-radius: 3px;
    }
    
    /* Главный экран */
    .hero {
      background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80') no-repeat center center/cover;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      padding: 0 20px;
    }
    
    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3.5rem;
      margin-bottom: 20px;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
    }
    
    .hero p {
      font-size: 1.5rem;
      max-width: 800px;
      margin-bottom: 30px;
    }
    
    .cta-button {
      display: inline-block;
      background: #e23ca5;
      color: white;
      padding: 15px 30px;
      text-decoration: none;
      border-radius: 30px;
      font-weight: 600;
      font-size: 1.1rem;
      transition: all 0.3s ease;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    
    .cta-button:hover {
      background: #5e2dc4;
      transform: translateY(-3px);
      box-shadow: 0 6px 12px rgba(0,0,0,0.3);
    }
    
    /* О нас */
    .about {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }
    
    .about h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 40px;
      color: #5e2dc4;
    }
    
    .about-content {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 40px;
    }
    
    .about-text {
      flex: 1;
      min-width: 300px;
    }
    
    .about-image {
      flex: 1;
      min-width: 300px;
      text-align: center;
    }
    
    .about-image img {
      max-width: 100%;
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    }
    
    /* Услуги */
    .services {
      background: #f9f9f9;
      padding: 80px 20px;
    }
    
    .services h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 40px;
      color: #5e2dc4;
    }
    
    .services-container {
      max-width: 1200px;
      margin: auto;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 30px;
    }
    
    .service-card {
      background: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
      transition: all 0.3s ease;
    }
    
    .service-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    }
    
    .service-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    
    .service-card-content {
      padding: 25px;
    }
    
    .service-card h3 {
      font-family: 'Playfair Display', serif;
      font-size: 1.5rem;
      margin-bottom: 15px;
      color: #e23ca5;
    }
    
    .service-card p {
      margin-bottom: 20px;
    }
    
    .service-card a {
      color: #5e2dc4;
      text-decoration: none;
      font-weight: 600;
      display: inline-flex;
      align-items: center;
    }
    
    .service-card a i {
      margin-left: 5px;
    }
    
    /* Акции */
    .promotions {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }
    
    .promotions h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 40px;
      color: #5e2dc4;
    }
    
    .promotion-card {
      background: linear-gradient(to right, #e23ca5, #5e2dc4);
      color: white;
      border-radius: 10px;
      padding: 30px;
      margin-bottom: 30px;
      display: flex;
      align-items: center;
      gap: 30px;
    }
    
    .promotion-card:last-child {
      margin-bottom: 0;
    }
    
    .promotion-text {
      flex: 2;
    }
    
    .promotion-text h3 {
      font-family: 'Playfair Display', serif;
      font-size: 1.8rem;
      margin-bottom: 15px;
    }
    
    .promotion-text p {
      margin-bottom: 20px;
    }
    
    .promotion-image {
      flex: 1;
      text-align: center;
    }
    
    .promotion-image img {
      max-width: 100%;
      border-radius: 10px;
    }
    
    .promotion-button {
      display: inline-block;
      background: white;
      color: #e23ca5;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 30px;
      font-weight: 600;
      transition: all 0.3s ease;
    }
    
    .promotion-button:hover {
      background: #f0f0f0;
    }
    
    /* Отзывы */
    .testimonials {
      background: #f9f9f9;
      padding: 80px 20px;
    }
    
    .testimonials h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 40px;
      color: #5e2dc4;
    }
    
    .testimonials-container {
      max-width: 1200px;
      margin: auto;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 30px;
    }
    
    .testimonial-card {
      background: white;
      border-radius: 10px;
      padding: 30px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
      position: relative;
    }
    
    .testimonial-card::before {
      content: """;
      font-size: 4rem;
      color: rgba(226, 60, 165, 0.2);
      position: absolute;
      top: 20px;
      left: 20px;
      font-family: 'Playfair Display', serif;
    }
    
    .testimonial-card p {
      margin-bottom: 20px;
      font-style: italic;
    }
    
    .testimonial-card .client {
      display: flex;
      align-items: center;
    }
    
    .client-avatar {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      margin-right: 15px;
      object-fit: cover;
    }
    
    .client-info h4 {
      margin: 0;
      color: #5e2dc4;
    }
    
    .client-info p {
      margin: 0;
      font-size: 0.9rem;
      color: #666;
    }
    
    /* Контакты */
    .contact {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }
    
    .contact h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 40px;
      color: #5e2dc4;
    }
    
    .contact-container {
      display: flex;
      flex-wrap: wrap;
      gap: 40px;
    }
    
    .contact-info {
      flex: 1;
      min-width: 300px;
    }
    
    .contact-info h3 {
      font-family: 'Playfair Display', serif;
      font-size: 1.8rem;
      margin-bottom: 20px;
      color: #e23ca5;
    }
    
    .contact-info p {
      margin-bottom: 15px;
      display: flex;
      align-items: center;
    }
    
    .contact-info i {
      margin-right: 10px;
      color: #5e2dc4;
      width: 20px;
      text-align: center;
    }
    
    .contact-form {
      flex: 1;
      min-width: 300px;
    }
    
    .contact-form h3 {
      font-family: 'Playfair Display', serif;
      font-size: 1.8rem;
      margin-bottom: 20px;
      color: #e23ca5;
    }
    
    .form-group {
      margin-bottom: 20px;
    }
    
    .form-group label {
      display: block;
      margin-bottom: 8px;
      font-weight: 600;
    }
    
    .form-group input,
    .form-group textarea {
      width: 100%;
      padding: 12px;
      border: 1px solid #ddd;
      border-radius: 5px;
      font-family: 'Open Sans', sans-serif;
      font-size: 1rem;
    }
    
    .form-group textarea {
      resize: vertical;
      min-height: 150px;
    }
    
    .submit-button {
      background: linear-gradient(to right, #e23ca5, #5e2dc4);
      color: white;
      border: none;
      padding: 15px 30px;
      border-radius: 30px;
      font-weight: 600;
      font-size: 1rem;
      cursor: pointer;
      transition: all 0.3s ease;
    }
    
    .submit-button:hover {
      transform: translateY(-3px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }
    
    /* Футер */
    footer {
      background: linear-gradient(to right, #e23ca5, #5e2dc4);
      color: white;
      padding: 60px 20px 30px;
    }
    
    .footer-content {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 40px;
    }
    
    .footer-section {
      flex: 1;
      min-width: 250px;
    }
    
    .footer-section h3 {
      font-family: 'Playfair Display', serif;
      font-size: 1.5rem;
      margin-bottom: 20px;
      position: relative;
      padding-bottom: 10px;
    }
    
    .footer-section h3::after {
      content: "";
      position: absolute;
      bottom: 0;
      left: 0;
      width: 50px;
      height: 3px;
      background: white;
      border-radius: 3px;
    }
    
    .footer-section p {
      margin-bottom: 15px;
    }
    
    .footer-section ul {
      list-style: none;
      padding: 0;
      margin: 0;
    }
    
    .footer-section ul li {
      margin-bottom: 10px;
    }
    
    .footer-section ul li a {
      color: white;
      text-decoration: none;
      transition: all 0.3s ease;
    }
    
    .footer-section ul li a:hover {
      text-decoration: underline;
    }
    
    .social-icons {
      display: flex;
      gap: 15px;
      margin-top: 20px;
    }
    
    .social-icons a {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 40px;
      height: 40px;
      background: rgba(255,255,255,0.2);
      border-radius: 50%;
      transition: all 0.3s ease;
    }
    
    .social-icons a:hover {
      background: white;
      color: #e23ca5;
    }
    
    .copyright {
      text-align: center;
      margin-top: 40px;
      padding-top: 20px;
      border-top: 1px solid rgba(255,255,255,0.2);
      font-size: 0.9rem;
    }
    
    /* Адаптивность */
    @media (max-width: 768px) {
      .nav-links {
        position: fixed;
        top: 70px;
        left: 0;
        width: 100%;
        background: linear-gradient(to right, #e23ca5, #5e2dc4);
        flex-direction: column;
        align-items: center;
        padding: 20px 0;
        transform: translateY(-150%);
        transition: transform 0.3s ease;
        z-index: 999;
      }
      
      .nav-links.active {
        transform: translateY(0);
      }
      
      .nav-links li {
        margin: 10px 0;
      }
      
      .menu-toggle {
        display: flex;
      }
      
      .hero h1 {
        font-size: 2.5rem;
      }
      
      .hero p {
        font-size: 1.2rem;
      }
      
      .about-content,
      .contact-container {
        flex-direction: column;
      }
      
      .promotion-card {
        flex-direction: column;
        text-align: center;
      }
      
      .promotion-text {
        order: 2;
      }
      
      .promotion-image {
        order: 1;
      }
    }
  </style>
</head>
<body>
  <!-- Навигация -->
  <nav>
    <div class="nav-container">
      <div class="logo">
        <img src="https://via.placeholder.com/50" alt="White Rose Beauty SPA">
        <span>White Rose Beauty SPA</span>
      </div>
      <ul class="nav-links">
        <li><a href="#home">Главная</a></li>
        <li><a href="#about">О нас</a></li>
        <li><a href="#services">Услуги</a></li>
        <li><a href="#promotions">Акции</a></li>
        <li><a href="#testimonials">Отзывы</a></li>
        <li><a href="#contact">Контакты</a></li>
      </ul>
      <div class="menu-toggle">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
  </nav>

  <!-- Главный экран -->
  <section class="hero" id="home">
    <h1 data-aos="fade-up">White Rose Beauty SPA</h1>
    <p data-aos="fade-up" data-aos-delay="100">Премиум салон красоты в Сыктывкаре</p>
    <a href="#services" class="cta-button" data-aos="fade-up" data-aos-delay="200">Наши услуги</a>
  </section>

  <!-- О нас -->
  <section class="about" id="about">
    <h2 data-aos="fade-up">О нас</h2>
    <div class="about-content">
      <div class="about-text" data-aos="fade-right">
        <p>White Rose Beauty SPA — это премиальный салон красоты в центре Сыктывкара, где каждый клиент может получить полный спектр услуг для поддержания красоты и здоровья.</p>
        <p>Наша команда профессионалов использует только проверенные косметические средства и современные методики, чтобы вы выглядели неотразимо.</p>
        <p>Мы создали уютную атмосферу, где вы можете расслабиться и получить удовольствие от процедур.</p>
      </div>
      <div class="about-image" data-aos="fade-left">
        <img src="https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80" alt="Салон красоты">
      </div>
    </div>
  </section>

  <!-- Услуги -->
  <section class="services" id="services">
    <h2 data-aos="fade-up">Наши услуги</h2>
    <div class="services-container">
      <div class="service-card" data-aos="fade-up" data-aos-delay="100">
        <img src="https://images.unsplash.com/photo-1596755094512-fb1a2afabf1c?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Массаж">
        <div class="service-card-content">
          <h3>Массаж и СПА</h3>
          <p>Расслабляющий массаж, обертывания, ароматерапия и другие СПА-процедуры для полного восстановления сил.</p>
          <a href="#contact">Записаться <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      <div class="service-card" data-aos="fade-up" data-aos-delay="200">
        <img src="https://images.unsplash.com/photo-1560066984-138dadb4c035?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Косметология">
        <div class="service-card-content">
          <h3>Косметология</h3>
          <p>Чистка лица, пилинги, уходовые процедуры, коррекция фигуры и многое другое.</p>
          <a href="#contact">Записаться <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      <div class="service-card" data-aos="fade-up" data-aos-delay="300">
        <img src="https://images.unsplash.com/photo-1516975080664-ed2fc6a32937?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Маникюр">
        <div class="service-card-content">
          <h3>Маникюр и педикюр</h3>
          <p>Классический и аппаратный маникюр, покрытие гель-лаком, дизайн ногтей, спа-педикюр.</p>
          <a href="#contact">Записаться <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      <div class="service-card" data-aos="fade-up" data-aos-delay="400">
        <img src="https://images.unsplash.com/photo-1521590832167-220acb8fc191?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Парикмахерские услуги">
        <div class="service-card-content">
          <h3>Парикмахерские услуги</h3>
          <p>Стрижки, окрашивание, укладки, кератиновое выпрямление и другие услуги для волос.</p>
          <a href="#contact">Записаться <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      <div class="service-card" data-aos="fade-up" data-aos-delay="500">
        <img src="https://images.unsplash.com/photo-1519494026892-80bbd2d6fd0d?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Брови и ресницы">
        <div class="service-card-content">
          <h3>Брови и ресницы</h3>
          <p>Коррекция и окрашивание бровей, ламинирование, наращивание ресниц.</p>
          <a href="#contact">Записаться <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      <div class="service-card" data-aos="fade-up" data-aos-delay="600">
        <img src="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Солярий">
        <div class="service-card-content">
          <h3>Солярий</h3>
          <p>Загар в современном солярии с использованием косметики для загара.</p>
          <a href="#contact">Записаться <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
    </div>
  </section>

  <!-- Акции -->
  <section class="promotions" id="promotions">
    <h2 data-aos="fade-up">Акции и скидки</h2>
    <div class="promotion-card" data-aos="fade-up" data-aos-delay="100">
      <div class="promotion-text">
        <h3>Скидка 20% на первый визит</h3>
        <p>Для новых клиентов мы предоставляем скидку 20% на любую услугу в нашем салоне.</p>
        <a href="#contact" class="promotion-button">Записаться</a>
      </div>
      <div class="promotion-image">
        <img src="https://images.unsplash.com/photo-1596755094512-fb1a2afabf1c?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Акция">
      </div>
    </div>
    <div class="promotion-card" data-aos="fade-up" data-aos-delay="200">
      <div class="promotion-text">
        <h3>Счастливые часы с 10:00 до 12:00</h3>
        <p>Запишитесь на процедуру в утренние часы и получите скидку 15% на все услуги.</p>
        <a href="#contact" class="promotion-button">Записаться</a>
      </div>
      <div class="promotion-image">
        <img src="https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80" alt="Акция">
      </div>
    </div>
  </section>

  <!-- Отзывы -->
  <section class="testimonials" id="testimonials">
    <h2 data-aos="fade-up">Отзывы клиентов</h2>
    <div class="testimonials-container">
      <div class="testimonial-card" data-aos="fade-up" data-aos-delay="100">
        <p>Отличный салон! Пользуюсь услугами уже полгода, всегда остаюсь довольна. Мастера профессионалы своего дела.</p>
        <div class="client">
          <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Клиент" class="client-avatar">
          <div class="client-info">
            <h4>Анна Петрова</h4>
            <p>Постоянный клиент</p>
          </div>
        </div>
      </div>
      <div class="testimonial-card" data-aos="fade-up" data-aos-delay="200">
        <p>Делала здесь свадебный макияж и укладку. Выглядела потрясающе! Мастер учла все мои пожелания.</p>
        <div class="client">
          <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Клиент" class="client-avatar">
          <div class="client-info">
            <h4>Елена Смирнова</h4>
            <p>Новичок</p>
          </div>
        </div>
      </div>
      <div class="testimonial-card" data-aos="fade-up" data-aos-delay="300">
        <p>Хожу только сюда на маникюр. Мастер Анна — волшебница! Всегда аккуратно и красиво.</p>
        <div class="client">
          <img src="https://randomuser.me/api/portraits/women/32.jpg" alt="Клиент" class="client-avatar">
          <div class="client-info">
            <h4>Мария Иванова</h4>
            <p>Постоянный клиент</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Контакты -->
  <section class="contact" id="contact">
    <h2 data-aos="fade-up">Контакты</h2>
    <div class="contact-container">
      <div class="contact-info" data-aos="fade-right">
        <h3>Свяжитесь с нами</h3>
        <p><i class="fas fa-map-marker-alt"></i> г. Сыктывкар, ул. Ленина, 42</p>
        <p><i class="fas fa-phone"></i> +7 (821) 123-45-67</p>
        <p><i class="fas fa-envelope"></i> info@whiterose.ru</p>
        <p><i class="fab fa-vk"></i> vk.com/club166483265</p>
        <p><i class="fab fa-instagram"></i> @whiterose_spa</p>
        <p><i class="fas fa-clock"></i> Пн-Пт: 10:00 - 20:00, Сб: 10:00 - 18:00, Вс: 11:00 - 17:00</p>
      </div>
      <div class="contact-form" data-aos="fade-left">
        <h3>Записаться на процедуру</h3>
        <form>
          <div class="form-group">
            <label for="name">Ваше имя</label>
            <input type="text" id="name" name="name" required>
          </div>
          <div class="form-group">
            <label for="phone">Телефон</label>
            <input type="tel" id="phone" name="phone" required>
          </div>
          <div class="form-group">
            <label for="service">Услуга</label>
            <input type="text" id="service" name="service" required>
          </div>
          <div class="form-group">
            <label for="message">Комментарий</label>
            <textarea id="message" name="message"></textarea>
          </div>
          <button type="submit" class="submit-button">Отправить заявку</button>
        </form>
      </div>
    </div>
  </section>

  <!-- Футер -->
  <footer>
    <div class="footer-content">
      <div class="footer-section">
        <h3>White Rose Beauty SPA</h3>
        <p>Премиум салон красоты в Сыктывкаре с полным спектром услуг для вашего отдыха и красоты.</p>
        <div class="social-icons">
          <a href="https://vk.com/club166483265" target="_blank"><i class="fab fa-vk"></i></a>
          <a href="#" target="_blank"><i class="fab fa-instagram"></i></a>
          <a href="#" target="_blank"><i class="fab fa-telegram"></i></a>
        </div>
      </div>
      <div class="footer-section">
        <h3>Услуги</h3>
        <ul>
          <li><a href="#services">Массаж и СПА</a></li>
          <li><a href="#services">Косметология</a></li>
          <li><a href="#services">Маникюр и педикюр</a></li>
          <li><a href="#services">Парикмахерские услуги</a></li>
          <li><a href="#services">Брови и ресницы</a></li>
          <li><a href="#services">Солярий</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>Информация</h3>
        <ul>
          <li><a href="#about">О нас</a></li>
          <li><a href="#promotions">Акции</a></li>
          <li><a href="#testimonials">Отзывы</a></li>
          <li><a href="#contact">Контакты</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>Контакты</h3>
        <p><i class="fas fa-map-marker-alt"></i> г. Сыктывкар, ул. Ленина, 42</p>
        <p><i class="fas fa-phone"></i> +7 (821) 123-45-67</p>
        <p><i class="fas fa-envelope"></i> info@whiterose.ru</p>
        <p><i class="fas fa-clock"></i> Пн-Пт: 10:00 - 20:00</p>
      </div>
    </div>
    <div class="copyright">
      &copy; 2023 White Rose Beauty SPA. Все права защищены.
    </div>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
  <script>
    // Инициализация AOS
    AOS.init({
      duration: 800,
      once: true
    });
    
    // Мобильное меню
    const menuToggle = document.querySelector('.menu-toggle');
    const navLinks = document.querySelector('.nav-links');
    
    menuToggle.addEventListener('click', () => {
      navLinks.classList.toggle('active');
    });
    
    // Закрытие меню при клике на ссылку
    document.querySelectorAll('.nav-links a').forEach(link => {
      link.addEventListener('click', () => {
        navLinks.classList.remove('active');
      });
    });
    
    // Плавная прокрутка к разделам
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          window.scrollTo({
            top: target.offsetTop - 70,
            behavior: 'smooth'
          });
        }
      });
    });
    
    // Обработка формы
    document.querySelector('form').addEventListener('submit', function(e) {
      e.preventDefault();
      
      // Здесь можно добавить код для отправки формы на сервер
      alert('Спасибо за заявку! Мы свяжемся с вами в ближайшее время.');
      this.reset();
    });
  </script>
</body>
</html>

