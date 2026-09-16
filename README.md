# pagina-web
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grey's Anatomy - Sitio Oficial de Fans</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <!-- Encabezado y Navegación -->
    <header>
        <div class="logo">
            <h1>Grey's Anatomy</h1>
        </div>
        <nav>
            <ul>
                <!-- Home -->
                <li><a href="#home">Home</a></li>
                
                <!-- Link 1: Personajes -->
                <li><a href="#personajes">Personajes</a></li>
                
                <!-- Link 2: Temporadas con Menú Desplegable (Submenú) -->
                <li class="dropdown">
                    <a href="#temporadas">Temporadas ▾</a>
                    <ul class="submenu">
                        <li><a href="#temp-clasicas">Temporadas 1 - 5</a></li>
                        <li><a href="#temp-doradas">Temporadas 6 - 10</a></li>
                        <li><a href="#temp-recientes">Temporadas 11+</a></li>
                    </ul>
                </li>
                
                <!-- Link 3: Galería de Imágenes -->
                <li><a href="#galeria">Galería</a></li>
                
                <!-- Link 4: Contacto -->
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <!-- Banner Principal / Hero -->
    <section id="home" class="hero">
        <div class="hero-text">
            <h2>Bienvenido al Grey Sloan Memorial Hospital</h2>
            <p>Descubre la vida, la pasión y el drama de los cirujanos más icónicos de la televisión.</p>
        </div>
    </section>

    <!-- Sección 1: Personajes -->
    <section id="personajes" class="contenedor">
        <h2>Personajes Principales</h2>
        <div class="grid-personajes">
            <div class="card">
                <h3>Meredith Grey</h3>
                <p>Cirujana general y pilar fundamental del hospital. Hija de la renombrada Ellis Grey.</p>
            </div>
            <div class="card">
                <h3>Derek Shepherd</h3>
                <p>Reconocido neurocirujano apodado "McDreamy", clave en la historia del hospital.</p>
            </div>
            <div class="card">
                <h3>Cristina Yang</h3>
                <p>Cirujana cardiotorácica brillante, ambiciosa y la "persona" de Meredith.</p>
            </div>
            <div class="card">
                <h3>Miranda Bailey</h3>
                <p>La Jefa de Cirugía, mentora estricta y de gran corazón apodada "El Nazi" en sus inicios.</p>
            </div>
        </div>
    </section>

    <!-- Sección 2: Temporadas (Contenido para las subopciones) -->
    <section id="temporadas" class="contenedor bg-light">
        <h2>Secciones de Temporadas</h2>
        <div id="temp-clasicas" class="subseccion">
            <h3>Temporadas 1 - 5</h3>
            <p>Los inicios de los internos original (MAGIC: Meredith, Alex, George, Izzie, Cristina) bajo la tutoría de Bailey.</p>
        </div>
        <div id="temp-doradas" class="subseccion">
            <h3>Temporadas 6 - 10</h3>
            <p>La fusión con Mercy West, la consolidación como cirujanos plenos y eventos drásticos como el tiroteo y el accidente aéreo.</p>
        </div>
        <div id="temp-recientes" class="subseccion">
            <h3>Temporadas 11 en adelante</h3>
            <p>Nuevas generaciones de residentes, la evolución de la medicina moderna y el cambio de era en el Grey Sloan Memorial.</p>
        </div>
    </section>

    <!-- Sección 3: Galería de Imágenes -->
    <section id="galeria" class="contenedor">
        <h2>Galería de Imágenes</h2>
        <div class="galeria-grid">
            <div class="galeria-item">
                <img src="https://picsum.photos/400/300?random=1" alt="Grey Sloan Hospital">
                <p>Entrada Principal</p>
            </div>
            <div class="galeria-item">
                <img src="https://picsum.photos/400/300?random=2" alt="Quirófano">
                <p>Quirófano 1</p>
            </div>
            <div class="galeria-item">
                <img src="https://picsum.photos/400/300?random=3" alt="Equipo Médico">
                <p>Reunión de Residentes</p>
            </div>
            <div class="galeria-item">
                <img src="https://picsum.photos/400/300?random=4" alt="Trauma Room">
                <p>Sala de Emergencias</p>
            </div>
        </div>
    </section>

    <!-- Sección 4: Formulario de Contacto -->
    <section id="contacto" class="contenedor bg-light">
        <h2>Contacto para Fans</h2>
        <form class="formulario">
            <div class="campo">
                <label for="nombre">Nombre Completo:</label>
                <input type="text" id="nombre" name="nombre" placeholder="Ej. Meredith Grey" required>
            </div>
            <div class="campo">
                <label for="email">Correo Electrónico:</label>
                <input type="email" id="email" name="email" placeholder="tuemail@ejemplo.com" required>
            </div>
            <div class="campo">
                <label for="personaje-favorito">Personaje Favorito:</label>
                <select id="personaje-favorito" name="personaje-favorito">
                    <option value="meredith">Meredith Grey</option>
                    <option value="derek">Derek Shepherd</option>
                    <option value="cristina">Cristina Yang</option>
                    <option value="bailey">Miranda Bailey</option>
                    <option value="otro">Otro</option>
                </select>
            </div>
            <div class="campo">
                <label for="mensaje">Mensaje o Sugerencia:</label>
                <textarea id="mensaje" name="mensaje" rows="4" placeholder="Escribe tu mensaje aquí..." required></textarea>
            </div>
            <button type="submit" class="btn">Enviar Mensaje</button>
        </form>
    </section>

    <!-- Pie de página -->
    <footer>
        <p>&copy; 2026 Fan Page Grey's Anatomy. Todos los derechos reservados.</p>
    </footer>

</body>
</html>
/* Estilos Generales */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    color: #333;
    line-height: 1.6;
    background-color: #f4f7f6;
}

.contenedor {
    padding: 60px 20px;
    max-width: 1100px;
    margin: auto;
}

.bg-light {
    background-color: #ffffff;
    border-radius: 8px;
}

/* Encabezado y Menú */
header {
    background-color: #0b2545;
    color: #fff;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 50px;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo h1 {
    font-size: 1.5rem;
    letter-spacing: 1px;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    position: relative;
}

nav ul li a {
    color: white;
    text-decoration: none;
    padding: 15px 20px;
    display: block;
    transition: background 0.3s;
}

nav ul li a:hover {
    background-color: #134074;
}

/* Submenú Desplegable (Desplegable de 2do nivel) */
.dropdown .submenu {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    background-color: #134074;
    min-width: 180px;
    box-shadow: 0px 8px 16px rgba(0,0,0,0.2);
    border-radius: 0 0 5px 5px;
}

.dropdown .submenu li a {
    padding: 12px 16px;
}

.dropdown:hover .submenu {
    display: block;
}

/* Hero Section (Home) */
.hero {
    background: linear-gradient(rgba(11, 37, 69, 0.7), rgba(11, 37, 69, 0.7)), 
                url('https://picsum.photos/1200/500?random=10') center/cover no-repeat;
    height: 60vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
}

.hero-text h2 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

/* Secciones de Contenido */
h2 {
    text-align: center;
    margin-bottom: 30px;
    color: #0b2545;
}

.grid-personajes {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
}

.card {
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    border-top: 4px solid #134074;
}

.subseccion {
    margin-bottom: 25px;
    padding: 15px;
    border-left: 4px solid #8da9c4;
    background-color: #f9fbfd;
}

/* Galería de Imágenes */
.galeria-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 20px;
}

.galeria-item {
    background: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    text-align: center;
    transition: transform 0.3s ease;
}

.galeria-item:hover {
    transform: translateY(-5px);
}

.galeria-item img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.galeria-item p {
    padding: 10px;
    font-weight: bold;
}

/* Formulario */
.formulario {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.campo {
    display: flex;
    flex-direction: column;
}

.campo label {
    margin-bottom: 5px;
    font-weight: bold;
}

.campo input, .campo select, .campo textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 1rem;
}

.btn {
    background-color: #0b2545;
    color: white;
    padding: 12px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    transition: background 0.3s;
}

.btn:hover {
    background-color: #134074;
}

/* Footer */
footer {
    background-color: #0b2545;
    color: white;
    text-align: center;
    padding: 20px;
    margin-top: 40px;
}
