<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi Web UX/UI</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Encabezado -->
  <header>
    <nav>
      <ul>
        <li><a href="#home">Inicio</a></li>
        <li><a href="#about">Acerca de</a></li>
        <li><a href="#services">Servicios</a></li>
        <li><a href="#contact">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <!-- Contenido Principal -->
  <main>
    <section id="home">
      <h1>Bienvenidos a mi sitio web</h1>
      <p>Este sitio está diseñado para ofrecer una experiencia de usuario intuitiva.</p>
    </section>

    <section id="about">
      <h2>Acerca de Nosotros</h2>
      <p>Somos una empresa dedicada a crear soluciones digitales centradas en el usuario.</p>
    </section>

    <section id="services">
      <h2>Servicios</h2>
      <ul>
        <li>Diseño de Interfaces</li>
        <li>Desarrollo Web</li>
        <li>Consultoría UX/UI</li>
      </ul>
    </section>

    <section id="contact">
      <h2>Contacto</h2>
      <form>
        <label for="name">Nombre:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Correo electrónico:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">Mensaje:</label>
        <textarea id="message" name="message" required></textarea>

        <button type="submit">Enviar</button>
      </form>
    </section>
  </main>

  <!-- Pie de página -->
  <footer>
    <p>&copy; 2025 Mi Empresa. Todos los derechos reservados.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
