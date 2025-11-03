<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device‑width, initial‑scale=1.0">
  <title>Vitvisor – Formación Tecnológica</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* estilos básicos integrados para facilidad */
    body { margin:0; font‑family: Arial, sans‑serif; line‑height:1.6; color:#333; }
    header { background:#0a3d62; color:#fff; padding:20px 0; }
    header .container { display:flex; align‑items:center; justify‑space-between; max‑width:1200px; margin:0 auto; padding:0 20px; }
    header .logo { font‑size:1.8em; font‑weight:bold; }
    nav ul { list‑style:none; margin:0; padding:0; display:flex; }
    nav ul li { margin‑left:20px; }
    nav ul li a { color:#fff; text‑decoration:none; }
    .hero { background:#f4f6f8; padding:100px 20px; text‑align:center; }
    .hero h1 { font‑size:2.8em; margin-bottom:20px; color:#0a3d62; }
    .hero p { font-size:1.2em; max‑width:700px; margin:0 auto 30px auto; }
    .btn { display:inline-block; padding:12px 30px; background:#0a3d62; color:#fff; text‑decoration:none; border‑radius:4px; }
    .container { max‑width:1200px; margin:0 auto; padding:0 20px; }
    section { padding:60px 0; }
    .services { display:flex; flex‑wrap:wrap; gap:30px; justify‑space‑between; }
    .service { flex:1 1 calc(33% ‑ 40px); background:#fff; border:1px solid #e1e1e1; border‑radius:8px; padding:30px; text‑align:center; }
    .service h3 { margin‑20px 0 10px; color:#0a3d62; }
    .team { display:flex; flex‑wrap:wrap; gap:30px; justify‑space‑between; }
    .member { flex:1 1 calc(50% ‑ 40px); text‑align:center; }
    .member img { width:150px; height:150px; border‑radius:50%; }
    footer { background:#333; color:#ccc; padding:40px 0; text-align:center; }
    footer a { color:#ccc; text‑decoration:none; }
    @media (max‑768px) {
      .services, .team { flex‑direction:column; }
      .service, .member { flex:1 1 100%; }
    }
  </style>
</head>
<body>

<header>
  <div class="container">
    <div class="logo">Vitvisor</div>
    <nav>
      <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#servicios">Servicios</a></li>
        <li><a href="#equipo">Equipo</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </div>
</header>

<section class="hero" id="inicio">
  <h1>Formación Tecnológica de Vanguardia</h1>
  <p>En Vitvisor combinamos experiencia, innovación y pasión para formar especialistas en sistemas microinformáticos, redes y nuevas tecnologías. Únete a nuestra comunidad y da el salto al siguiente nivel.</p>
  <a class="btn" href="#servicios">Nuestros Servicios</a>
</section>

<section id="servicios">
  <div class="container">
    <h2>Qué ofrecemos</h2>
    <div class="services">
      <div class="service">
        <h3>Formación en Redes y Sistemas</h3>
        <p>Profundizamos en sistemas microinformáticos, redes, mantenimiento, virtualización y más con un enfoque práctico.</p>
      </div>
      <div class="service">
        <h3>Desarrollo Web y Programación</h3>
        <p>Desde HTML/CSS hasta frameworks modernos. Aprenderás a crear sitios, apps y servicios reales.</p>
      </div>
      <div class="service">
        <h3>Consultoría y Soporte Técnologico</h3>
        <p>Servicios de asesoría tecnológica, auditoría de sistemas y soporte para empresas que quieren digitalizarse.</p>
      </div>
    </div>
  </div>
</section>

<section id="equipo">
  <div class="container">
    <h2>Nuestro Equipo</h2>
    <div class="team">
      <div class="member">
        <img src="https://via.placeholder.com/150" alt="Sergio de Paz">
        <h4>Sergio de Paz</h4>
        <p>Fundador y Formador Principal</p>
      </div>
      <div class="member">
        <img src="https://via.placeholder.com/150" alt="SysBoos">
        <h4>SysBoos</h4>
        <p>Inteligencia de Apoyo y Desarrollo</p>
      </div>
    </div>
  </div>
</section>

<section id="contacto">
  <div class="container">
    <h2>Contacto</h2>
    <p>¿Tienes preguntas o quieres colaborar con nosotros? Escríbenos y estaremos encantados de responderte.</p>
    <p><strong>Email:</strong> contacto@vitvisor.com</p>
    <p><strong>Teléfono:</strong> +34 600 000 000</p>
    <a class="btn" href="mailto:contacto@vitvisor.com">Envíanos un email</a>
  </div>
</section>

<footer>
  <div class="container">
    <p>© 2025 Vitvisor. Todos los derechos reservados.</p>
    <p><a href="#">Política de Privacidad</a> | <a href="#">Términos de Uso</a></p>
  </div>
</footer>

</body>
</html>
