<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>VitalFit</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: #0d1b2a;
      color: #e0e1dd;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(90deg, #1abc9c, #2c5364);
      padding: 2rem 2rem 3rem;
      text-align: center;
      color: white;
    }

    header h1 {
      font-size: 3rem;
      font-weight: 700;
      animation: glow 2s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 10px #1abc9c, 0 0 20px #1abc9c;
      }
      to {
        text-shadow: 0 0 20px #00c3ff, 0 0 30px #2c5364;
      }
    }

    .header-img {
      width: 100%;
      max-height: 400px;
      object-fit: cover;
      margin-top: 1rem;
      border-radius: 12px;
      box-shadow: 0 0 15px #1abc9c;
    }

    nav {
      margin-top: 2rem;
    }

    nav a {
      background: #1abc9c;
      color: #0d1b2a;
      padding: 0.7rem 1.2rem;
      margin: 0 0.5rem;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s ease, color 0.3s ease;
    }

    nav a:hover {
      background: #00c3ff;
      color: #0d1b2a
    }

    main {
      display: flex;
      max-width: 1200px;
      margin: 2rem auto;
      gap: 2rem;
      padding: 0 1rem;
      flex-wrap: wrap;
    }

    .posts {
      flex: 2;
      min-width: 0;
    }

    article {
      background: #2c2c2e;
      padding: 1.5rem;
      margin-bottom: 2rem;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(26, 188, 156,0.3);
    }

    article h2 {
      color: #1abc9c;
      margin-bottom: 0.5rem;
      font-size: 1.5rem;
    }

    article p {
      color: #e0e1dd;
      font-size: 1rem;
    }

    .athlete-card {
      background: #2d3e50;
      border-left: 5px solid #1abc9c;
      padding: 1rem;
      margin-bottom: 1.5rem;
      border-radius: 10px;
      display: flex;
      align-items: center;
      gap: 1rem;
      box-shadow: 0 0 10px #1abc9c55;
      flex-wrap: wrap;
    }

    .athlete-card img {
      width: 120px;
      height: auto;
      border-radius: 10px;
      flex-shrink: 0;
    }

    .athlete-card .info {
      flex: 1;
    }

    aside {
      flex: 1;
      background: #2b2b2d;
      padding: 1rem;
      border-radius: 10px;
      box-shadow: 0 0 10px #00f7ff66;
      min-width: 250px;
    }

    aside h3 {
      margin-bottom: 1rem;
      color: #00f7ff;
    }

    aside ul {
      list-style: none;
      padding-left: 0;
    }

    aside ul li {
      margin-bottom: 0.7rem;
    }

    aside ul li a {
      color: #f0f0f0;
      text-decoration: none;
      font-weight: bold;
    }

    aside ul li a:hover {
      color: #ff00d4;
    }

    footer {
      text-align: center;
      padding: 1rem;
      background: #1c1c1e;
      color: #999;
      margin-top: 3rem;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      main {
        flex-direction: column;
      }

      .athlete-card {
        flex-direction: column;
        text-align: center;
      }

      .athlete-card img {
        margin: 0 auto;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>VitalFit Blog</h1>
    <img src="https://i.pinimg.com/originals/62/54/5c/62545cb60d4d2e1e6e2789a3f09788e0.jpg" alt="Ilustración anime fitness" class="header-img" />
    <nav>
      <a href="#">Inicio</a>
      <a href="#">Sobre mí</a>
      <a href="#">Contacto</a>
    </nav>
  </header>

  <main>
    <section class="posts">
      <article>
        <h2>5 apps que debes conocer en 2025</h2>
        <p>Estas herramientas digitales están marcando tendencia en el entrenamiento físico digitalizado, generando impacto en rendimiento y consistencia diaria.</p>
      </article>

      <article>
        <h2>Salud mental y redes: conexión responsable</h2>
        <p>La gestión emocional en entornos digitales es clave. Aquí te explicamos cómo mejorar tu salud mental y mantener disciplina mientras consumes contenido fitness.</p>
      </article>

      <div class="athlete-card">
        <img src="https://images.unsplash.com/photo-1605296867304-46d5465a13f1?fit=crop&w=400&q=80" alt="Atleta Usain Bolt genérico" />
        <div class="info">
          <h3>Usain Bolt</h3>
          <p>Última presentación técnica: 9.81s en los 100m de Río 2016. Aceleración perfecta en los primeros 30m, excelente control biomecánico y fase final sin pérdida de potencia.</p>
        </div>
      </div>

      <div class="athlete-card">
        <img src="imagenes/Simone.jpg" alt="Simone Biles" />
        <div class="info">
          <h3>Simone Biles</h3>
          <p>Última actuación técnica: Mundial 2023. Ejecución impecable en doble mortal con giro, alto nivel de dificultad (G+), aterrizajes precisos y control mental sobresaliente.</p>
        </div>
      </div>

<div class="athlete-card">
        <img src="imagenes/Jarry.jpg" alt="Nicolas Jarry" />
        <div class="info">
          <h3>Nicolas Jarry</h3>
          <p>Nicolás Jarry sigue haciendo historia en Wimbledon 2025. En un emocionante partido de tercera ronda disputado el pasado viernes 4 de julio, el tenista chileno logró una trabajada y significativa victoria sobre el prometedor brasileño Joao Fonseca con parciales de 6-3, 6-4, 3-6 y 7-6.</p>
        </div>
      </div>

    </section>

    <aside>
      <h3>Redes Sociales</h3>
      <ul>
        <li><a href="#">Instagram</a></li>
        <li><a href="#">TikTok</a></li>
        <li><a href="#">YouTube</a></li>
      </ul>
    </aside>
  </main>

  <footer>
    &copy; 2025 VitalFit Blog | Inspiración y técnica para la nueva generación.
  </footer>

</body>
</html>
