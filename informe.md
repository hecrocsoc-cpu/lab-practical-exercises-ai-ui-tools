´Prompt que utilicé:
Hazme una landing page con las siguientes caracteristicas: El objetivo o tema de la pagina es las prevención de ahogamientos, necesito que tenga un header con nav, hero, 3 cards y un footer. Formato de html y css
<details>
<summary>Ver HTML generado</summary>

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Prevención de Ahogamientos</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            line-height: 1.6;
        }

        /* HEADER */
        header {
            background: #0077b6;
            color: white;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav a {
            color: white;
            margin-left: 20px;
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            text-decoration: underline;
        }

        /* HERO */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
                        url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .hero button {
            padding: 12px 25px;
            border: none;
            background: #00b4d8;
            color: white;
            font-size: 1rem;
            cursor: pointer;
            border-radius: 5px;
        }

        .hero button:hover {
            background: #0096c7;
        }

        /* CARDS */
        .cards {
            display: flex;
            justify-content: center;
            gap: 20px;
            padding: 50px 20px;
            flex-wrap: wrap;
        }

        .card {
            background: #f4f4f4;
            padding: 20px;
            border-radius: 10px;
            width: 300px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .card h3 {
            margin-bottom: 15px;
            color: #0077b6;
        }

        .card p {
            font-size: 0.95rem;
        }

        /* FOOTER */
        footer {
            background: #023e8a;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
        }

        footer p {
            font-size: 0.9rem;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }

            nav {
                display: none;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <h2>Seguridad Acuática</h2>
        <nav>
            <a href="#">Inicio</a>
            <a href="#">Consejos</a>
            <a href="#">Prevención</a>
            <a href="#">Contacto</a>
        </nav>
    </header>

    <!-- HERO -->
    <section class="hero">
        <h1>Prevención de Ahogamientos</h1>
        <p>La seguridad en el agua salva vidas. Aprende cómo protegerte y proteger a otros.</p>
        <button>Aprender más</button>
    </section>

    <!-- CARDS -->
    <section class="cards">
        <div class="card">
            <h3>Supervisión constante</h3>
            <p>Nunca dejes a niños solos cerca del agua. La vigilancia activa es clave para evitar accidentes.</p>
        </div>

        <div class="card">
            <h3>Aprende a nadar</h3>
            <p>La educación acuática reduce significativamente el riesgo de ahogamiento en todas las edades.</p>
        </div>

        <div class="card">
            <h3>Uso de flotadores</h3>
            <p>Utiliza chalecos salvavidas certificados en playas, piscinas o actividades acuáticas.</p>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>© 2026 Prevención de Ahogamientos | Todos los derechos reservados</p>
    </footer>

</body>
</html>
```
</details>
Le añado manualmente 3 imagenes a las cards y ajusto con css.
Le añado id a los nav para que nos lleven a las cards y hero.
Pongo el header en fixed para continuidad en el scroll y añado función al botón inicio.
Intento hacer trolleo operando con claude haciendo preguntas de hacer funcion para paginas infinitas, no parece muy dispuesta.
Añade automaticamente funciones @media para pantallas.
Pido a claude que añada responsive para 3 tipos de pantalla y testeo
Revisando veo fallo en orden de aplicación del código según resoluciones
