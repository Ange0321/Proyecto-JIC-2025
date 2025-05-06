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
/* styles.css */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  color: #333;
}

header {
  background-color: #007BFF;
  padding: 20px;
  color: white;
  text-align: center;
}

nav ul {
  list-style: none;
}

nav ul li {
  display: inline;
  margin-right: 20px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

main {
  padding: 20px;
}

section {
  margin-bottom: 40px;
}

section#home h1 {
  color: #007BFF;
}

form label {
  display: block;
  margin: 10px 0 5px;
}

form input, form textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

form button {
  background-color: #007BFF;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
}

footer {
  text-align: center;
  background-color: #333;
  color: white;
  padding: 10px;
}
// script.js
document.querySelector('form').addEventListener('submit', function (e) {
  e.preventDefault();

  let name = document.getElementById('name').value;
  let email = document.getElementById('email').value;
  let message = document.getElementById('message').value;

  if (name && email && message) {
    alert('Formulario enviado con éxito');
  } else {
    alert('Por favor, complete todos los campos.');
  }
});
