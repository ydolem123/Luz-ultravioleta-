# Luz-ultravioleta-
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Explorando la Luz Ultravioleta</title>
    <link rel="stylesheet" href="style.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <h1>Explorando la Luz Ultravioleta</h1>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#que-es">¿Qué es?</a></li>
                <li><a href="#aplicaciones">Aplicaciones</a></li>
                <li><a href="#beneficios">Beneficios y Riesgos</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <section id="inicio" class="section">
        <h2>Bienvenido</h2>
        <p>Descubre el poder invisible de la luz ultravioleta y su impacto en la ciencia, la tecnología y la vida cotidiana.</p>
        <button id="btn-info">Ver un Dato Curioso</button>
        <p id="dato-curioso"></p>
    </section>

    <section id="que-es" class="section">
        <h2>¿Qué es la Luz Ultravioleta?</h2>
        <p>La luz ultravioleta (UV) es un tipo de radiación electromagnética que no es visible para el ojo humano...</p>
    </section>

    <section id="aplicaciones" class="section">
        <h2>Aplicaciones</h2>
        <ul>
            <li>Desinfección y esterilización</li>
            <li>Detección de fraudes con luz negra</li>
            <li>Fotografía y astronomía</li>
        </ul>
    </section>

    <section id="beneficios" class="section">
        <h2>Beneficios y Riesgos</h2>
        <p>La luz UV tiene beneficios como la producción de vitamina D, pero también puede causar daños en la piel y los ojos.</p>
    </section>

    <section id="contacto" class="section">
        <h2>Contacto</h2>
        <p>¿Tienes preguntas? Contáctanos llenando el siguiente formulario:</p>
        <form>
            <input type="text" placeholder="Tu nombre" required>
            <input type="email" placeholder="Tu correo" required>
            <textarea placeholder="Tu mensaje" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Explorando la Luz Ultravioleta</p>
    </footer>
</body>
</html>body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #111;
    color: #fff;
}

header {
    background-color: #5500aa;
    padding: 20px;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

.section {
    padding: 50px;
    text-align: center;
}

button {
    background-color: #6600ff;
    color: white;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #8800ff;
}

form input, form textarea {
    width: 80%;
    padding: 10px;
    margin: 10px 0;
}

footer {
    background-color: #5500aa;
    text-align: center;
    padding: 10px;
    position: relative;
    bottom: 0;
    width: 100%;
}document.getElementById("btn-info").addEventListener("click", function() {
    const datos = [
        "La luz UV puede matar bacterias y virus en pocos segundos.",
        "Las abejas pueden ver la luz ultravioleta, lo que les ayuda a encontrar flores.",
        "Las lámparas UV se usan para esterilizar agua en zonas sin acceso a agua potable."
    ];
    let datoAleatorio = datos[Math.floor(Math.random() * datos.length)];
    document.getElementById("dato-curioso").innerText = datoAleatorio;
});
