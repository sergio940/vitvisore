<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vitvisor – Retro-Gamer Arcade</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

body {
  margin: 0;
  font-family: 'Press Start 2P', cursive;
  background: #0b0c10;
  color: #c5c6c7;
  position: relative;
  overflow-x: hidden;
}

/* Scanlines CRT */
body::before {
  content: '';
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: repeating-linear-gradient(
    rgba(0,0,0,0.05) 0px,
    rgba(0,0,0,0.05) 1px,
    transparent 1px,
    transparent 2px
  );
  pointer-events: none;
  z-index: 9999;
}

/* Parpadeo de texto */
@keyframes blink {
  0%, 50%, 100% { opacity: 1; }
  25%, 75% { opacity: 0; }
}

header {
  background: #1f2833;
  padding: 20px 0;
  border-bottom: 4px solid #66fcf1;
}

header .container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
}

header .logo {
  font-size: 1.5em;
  color: #66fcf1;
  text-shadow: 2px 2px #0b0c10;
}

nav ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

nav ul li { margin-left: 20px; }

nav ul li a {
  color: #66fcf1;
  text-decoration: none;
  transition: 0.3s;
}

nav ul li a:hover { color: #45a29e; text-shadow: 0 0 5px #45a29e; }

.hero {
  background: url('https://i.imgur.com/kd3X2vU.png') center/cover no-repeat;
  padding: 120px 20px;
  text-align: center;
  color: #45a29e;
  text-shadow: 2px 2px #0b0c10;
}

.hero h1 {
  font-size: 2em;
  margin-bottom: 20px;
  animation: blink 1s infinite;
}

.hero p { max-width: 700px; margin: 0 auto 30px; }

.btn {
  display: inline-block;
  padding: 12px 25px;
  background: #45a29e;
  color: #0b0c10;
  text-decoration: none;
  border-radius: 4px;
  font-weight: bold;
  transition: 0.3s;
  box-shadow: 0 0 10px #45a29e, 0 0 20px #66fcf1;
}

.btn:hover { box-shadow: 0 0 20px #45a29e, 0 0 30px #66fcf1; }

section { padding: 60px 20px; }

h2 {
  text-align: center;
  color: #66fcf1;
  margin-bottom: 40px;
  animation: blink 2s infinite;
}

.services, .team, .noticias-list {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: center;
}

.service, .member, .noticia {
  flex: 1 1 300px;
  background: #1f2833;
  border: 3px solid #45a29e;
  border-radius: 8px;
  padding: 30px;
  text-align: center;
  transition: 0.3s;
}

.service:hover, .member:hover, .noticia:hover {
  background: #0b0c10;
  border-color: #66fcf1;
  box-shadow: 0 0 15px #66fcf1;
}

.service h3, .member h4, .noticia h3 {
  margin: 20px 0 10px;
  color: #66fcf1;
  text-shadow: 1px 1px #0b0c10;
}

.member img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 2px solid #45a29e;
}

footer {
  background: #1f2833;
  color: #c5c6c7;
  padding: 40px 20px;
  text-align: center;
  border-top: 4px solid #66fcf1;
}

footer a { color: #45a29e; text-decoration: none; }
footer a:hover { color: #66fcf1; }

/* Noticias animadas */
.noticias-scroll {
  display: flex;
  overflow: hidden;
  width: 100%;
  margin: 0 auto;
}

.noticias-inner {
  display: flex;
  animation: scrollLeft 15s linear infinite;
  gap: 20px;
}

@keyframes scrollLeft {
  0% { transform: translateX(0); }
  100% { transform: translateX(-100%); }
}

@media (max-width: 768px) {
  .services, .team, .noticias-inner { flex-direction: column; align-items: center; }
  .noticias-inner { animation: none; }
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
        <li><a href="#noticias">Noticias</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </div>
</header>

<section class="hero" id="inicio">
  <h1>Vitvisor Retro-Gamer</h1>
  <p>Aprende tecnología con estilo pixel. Sumérgete en redes, programación y soporte con la vibra de los videojuegos clásicos.</p>
  <a class="btn" href="#servicios">Nuestros Servicios</a>
</section>

<section id="servicios">
  <h2>Servicios Retro</h2>
  <div class="services">
    <div class="service">
      <h3>Redes & Sistemas</h3>
      <p>Configura routers, switches y redes virtuales con nuestro módulo retro. ¡Nivel Boss desbloqueado!</p>
    </div>
    <div class="service">
      <h3>Desarrollo Web</h3>
      <p>Diseña páginas y apps con estética pixel-art, aprendiendo HTML, CSS y JS de manera práctica y divertida.</p>
    </div>
    <div class="service">
      <h3>Consultoría Tech</h3>
      <p>Asesora empresas y optimiza sistemas con estrategia, ¡como un verdadero jefe final de IT!</p>
    </div>
  </div>
</section>

<section id="equipo">
  <h2>Equipo Pixel</h2>
  <div class="team">
    <div class="member">
      <img src="https://via.placeholder.com/150" alt="Sergio de Paz">
      <h4>Sergio de Paz</h4>
      <p>Fundador y Formador Principal</p>
    </div>
    <div class="member">
      <img src="https://via.placeholder.com/150" alt="SysBoos">
      <h4>SysBoos</h4>
      <p>IA de Apoyo y Desarrollo</p>
    </div>
  </div>
</section>

<section id="noticias">
  <h2>Últimas Entradas</h2>
  <div class="noticias-scroll">
    <div class="noticias-inner">
      <div class="noticia">
        <h3>Nuevo Curso de Redes Pixeladas</h3>
        <p>Aprende a configurar routers y redes virtuales con nuestro módulo retro. ¡Nivel Boss desbloqueado!</p>
      </div>
      <div class="noticia">
        <h3>Tips de Programación Retro</h3>
        <p>Trucos y hacks para dominar HTML, CSS y JS con un estilo pixel-art que recuerda los 80s.</p>
      </div>
      <div class="noticia">
        <h3>Soporte Tech Arcade</h3>
        <p>Atención a problemas de sistemas con estrategias tipo juego: cada fallo es un mini-jefe a superar.</p>
      </div>
      <div class="noticia">
        <h3>Nuevas Misiones Tech</h3>
        <p>Actualizaciones y retos semanales para mejorar tus habilidades de IT con estilo retro.</p>
      </div>
    </div>
  </div>
</section>

<section id="contacto">
  <h2>Contacto Retro</h2>
  <p>¿Tienes dudas o quieres unirte a la aventura? Escríbenos y responderemos con velocidad pixel.</p>
  <p><strong>Email:</strong> contacto@vitvisor.com</p>
  <p><strong>Teléfono:</strong> +34 600 000 000</p>
  <a class="btn" href="mailto:contacto@vitvisor.com">Enviar Email</a>
</section>

<footer>
  <p>© 2025 Vitvisor – Todos los derechos reservados.</p>
  <p><a href="#">Política de Privacidad</a> | <a href="#">Términos de Uso</a></p>
</footer>

</body>
</html>
