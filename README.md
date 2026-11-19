# PULIDOS-MARTINEZ
Especialistas en trabajos en mármol, cantera, granito, terrazo, madera y lavado profundo de cerámicas. Devolvemos la elegancia y el acabado espejo a tus espacios residenciales y comerciales.
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pulidos Martínez | Pulido de Pisos y Superficies</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>
        /* Variables de color basadas en las imágenes */
        :root {
            --azul-marino: #122B49;
            --azul-claro: #1D4575;
            --amarillo-acento: #F5A623;
            --gris-fondo: #F4F6F9;
            --texto-oscuro: #222222;
            --blanco: #FFFFFF;
            --verde-whatsapp: #25D366;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--gris-fondo);
            color: var(--texto-oscuro);
            line-height: 1.6;
        }

        /* Encabezado / Navegación */
        header {
            background-color: var(--azul-marino);
            color: var(--blanco);
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
            border-bottom: 4px solid var(--amarillo-acento);
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            letter-spacing: 1px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo span {
            color: var(--amarillo-acento);
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        nav a {
            color: var(--blanco);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--amarillo-acento);
        }

        /* Sección Principal (Hero) */
        .hero {
            background: linear-gradient(rgba(18, 43, 73, 0.8), rgba(18, 43, 73, 0.85)), 
                        url('https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat;
            color: var(--blanco);
            text-align: center;
            padding: 100px 20px;
            position: relative;
        }

        .hero h1 {
            font-size: 3rem;
            font-weight: 800;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .hero p.eslogan {
            font-size: 1.4rem;
            color: var(--amarillo-acento);
            font-weight: 700;
            margin-bottom: 20px;
        }

        .hero p.descripcion {
            max-width: 700px;
            margin: 0 auto 35px auto;
            font-size: 1.1rem;
            color: #E0E6ED;
        }

        .btn-grupo {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 15px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1rem;
            transition: transform 0.2s, background-color 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }

        .btn:hover {
            transform: translateY(-3px);
        }

        .btn-whatsapp {
            background-color: var(--verde-whatsapp);
            color: var(--blanco);
        }

        .btn-llamar {
            background-color: var(--amarillo-acento);
            color: var(--azul-marino);
        }

        /* Sección de Servicios */
        .servicios {
            padding: 80px 5%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .titulo-seccion {
            text-align: center;
            margin-bottom: 50px;
        }

        .titulo-seccion h2 {
            font-size: 2.2rem;
            color: var(--azul-marino);
            text-transform: uppercase;
            font-weight: 800;
        }

        .linea-decorativa {
            width: 80px;
            height: 4px;
            background-color: var(--amarillo-acento);
            margin: 10px auto 0 auto;
        }

        .grid-servicios {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .tarjeta-servicio {
            background-color: var(--blanco);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.06);
            border-top: 5px solid var(--azul-marino);
            transition: transform 0.3s, border-color 0.3s;
        }

        .tarjeta-servicio:hover {
            transform: translateY(-5px);
            border-top-color: var(--amarillo-acento);
        }

        .tarjeta-servicio h3 {
            color: var(--azul-marino);
            font-size: 1.3rem;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .tarjeta-servicio p {
            color: #555555;
            font-size: 0.95rem;
        }

        /* Sección Por qué elegirnos / Calidad */
        .destacado {
            background-color: var(--azul-claro);
            color: var(--blanco);
            padding: 60px 5%;
            text-align: center;
        }

        .destacado h2 {
            font-size: 2rem;
            margin-bottom: 15px;
        }

        .destacado p {
            max-width: 750px;
            margin: 0 auto;
            font-size: 1.1rem;
        }

        /* Sección de Contacto */
        .contacto {
            padding: 80px 5%;
            max-width: 1000px;
            margin: 0 auto;
        }

        .contenedor-contacto {
            background-color: var(--blanco);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            display: grid;
            grid-template-columns: 1fr 1fr;
        }

        .info-contacto {
            background-color: var(--azul-marino);
            color: var(--blanco);
            padding: 40px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .info-contacto h3 {
            font-size: 1.8rem;
            color: var(--amarillo-acento);
            margin-bottom: 5px;
        }

        .info-contacto .subtitulo {
            font-size: 1rem;
            margin-bottom: 30px;
            color: #CBD5E1;
        }

        .dato-item {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }

        .dato-item strong {
            display: block;
            color: var(--amarillo-acento);
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .dato-item a {
            color: var(--blanco);
            text-decoration: none;
            font-weight: 600;
        }

        .dato-item a:hover {
            text-decoration: underline;
        }

        .formulario-contacto {
            padding: 40px;
        }

        .formulario-contacto h4 {
            color: var(--azul-marino);
            font-size: 1.4rem;
            margin-bottom: 20px;
        }

        .grupo-input {
            margin-bottom: 15px;
        }

        .grupo-input label {
            display: block;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 5px;
            color: var(--azul-marino);
        }

        .grupo-input input, 
        .grupo-input select, 
        .grupo-input textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #CCC;
            border-radius: 5px;
            font-size: 0.95rem;
        }

        .btn-enviar {
            width: 100%;
            background-color: var(--azul-marino);
            color: var(--blanco);
            border: none;
            padding: 14px;
            font-size: 1rem;
            font-weight: 700;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .btn-enviar:hover {
            background-color: var(--azul-claro);
        }

        /* Pie de página */
        footer {
            background-color: #0B1B2E;
            color: #A0AEC0;
            text-align: center;
            padding: 25px 20px;
            font-size: 0.9rem;
            border-top: 4px solid var(--amarillo-acento);
        }

        /* Botón Flotante de WhatsApp */
        .whatsapp-float {
            position: fixed;
            bottom: 25px;
            right: 25px;
            background-color: var(--verde-whatsapp);
            color: var(--blanco);
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.3);
            text-decoration: none;
            z-index: 1000;
            transition: transform 0.3s;
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
        }

        /* Responsivo para celulares */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.2rem; }
            .contenedor-contacto { grid-template-columns: 1fr; }
            nav ul { display: none; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">
            PULIDOS <span>MARTÍNEZ
        </div>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <section id="inicio" class="hero">
        <h1>Pulidos Martìnez </h1>
        <p class="eslogan">Tu mejor opción en restauración y brillo de pisos</p>
        <p class="descripcion">
            Especialistas en trabajos en mármol, cantera, granito, terrazo, madera y lavado profundo de cerámicas.Devolvemos la elegancia y el acabado espejo a tus espacios residenciales y comerciales.
        </p>
        <div class="btn-grupo">
            <a href="https://wa.me/525611736651?text=Hola%20Christian,%20me%20interesa%20cotizar%20un%20trabajo%20de%20pulido." target="_blank" class="btn btn-whatsapp">
                Cotizar por WhatsApp
            </a>
            <a href="tel:5645576656" class="btn btn-llamar">
                Llamar: 56 4557 6656
            </a>
        </div>
    </section>

    <section id="servicios" class="servicios">
        <div class="titulo-seccion">
            <h2>Nuestros Servicios</h2>
            <div class="linea-decorativa"></div>
        </div>

        <div class="grid-servicios">
            <div class="tarjeta-servicio">
                <h3>✨ Mármol</h3>
                <p>Desbastado, pulido y abrillantado profesional para eliminar rayones, manchas y opacidad, logrando un reflejo tipo espejo.</p>
            </div>

            <div class="tarjeta-servicio">
                <h3>🏛️ Cantera</h3>
                <p>Limpieza profunda, restauración y sellado protector para conservar la textura natural y evitar la absorción de humedad.</p>
            </div>

            <div class="tarjeta-servicio">
                <h3>💎 Granito</h3>
                <p>Pulido de alta resistencia con maquinaria especializada para resaltar la veta natural y durabilidad de tus superficies.</p>
            </div>

            <div class="tarjeta-servicio">
                <h3>🏢 Terrazo</h3>
                <p>Renovación completa para pisos de alto tránsito, nivelando juntas y devolviendo el brillo original a áreas comerciales o del hogar.</p>
            </div>

            <div class="tarjeta-servicio">
                <h3>🪵 Madera</h3>
                <p>Pulido fino y barnizado para duelas y pisos de madera, eliminando el desgaste diario y protegiendo la superficie.</p>
            </div>

            <div class="tarjeta-servicio">
                <h3>🧼 Lavado de Cerámica</h3>
                <p>Limpieza mecánica profunda de losetas y boquillas para remover suciedad incrustada y devolver su aspecto limpio.</p>
            </div>
        </div>
    </section>

    <section class="destacado">
        <h2>Resultados Garantizados en Cada Proyecto</h2>
        <p>
            Atención personalizada directamente por <strong>Christian Martínez</strong> Utilizamos equipo profesional y productos de primera calidad para cuidar tu patrimonio.
        </p>
    </section>

    <section id="contacto" class="contacto">
        <div class="titulo-seccion">
            <h2>Contáctanos</h2>
            <div class="linea-decorativa"></div>
        </div>

        <div class="contenedor-contacto">
            <div class="info-contacto">
                <h3>Christian Martínez</h3>
                <p class="subtitulo">Presupuestos sin compromiso</p>

                <div class="dato-item">
                    <strong>Teléfono Directo</strong>
                    <a href="tel:5645576656">56 4557 6656</a>)
                </div>

                <div class="dato-item">
                    <strong>WhatsApp</strong>
                    <a href="https://wa.me/525611736651" target="_blank">56 1173 6651</a>

                <div class="dato-item">
                    <strong>Especialidades</strong>
                    <span>Mármol • Cantera • Granito • Terrazo • Madera • Cerámica</span>
                </div>
            </div>

            <div class="formulario-contacto">
                <h4>Solicita una cotización</h4>
                <form action="#" method="POST">
                    <div class="grupo-input">
                        <label for="nombre">Tu Nombre</label>
                        <input type="text" id="nombre" name="nombre" placeholder="Ej. Juan Pérez" required>
                    </div>

                    <div class="grupo-input">
                        <label for="telefono">Teléfono / WhatsApp</label>
                        <input type="tel" id="telefono" name="telefono" placeholder="Ej. 55 1234 5678" required>
                    </div>

                    <div class="grupo-input">
                        <label for="servicio">Tipo de Superficie</label>
                        <select id="servicio" name="servicio">
                            <option value="marmol">Mármol</option>
                            <option value="cantera">Cantera</option>
                            <option value="granito">Granito</option>
                            <option value="terrazo"></option>
                            <option value="madera">Madera</option>
                            <option value="ceramica">Lavado de Cerámica</option>
                        </select>
                    </div>

                    <div class="grupo-input">
                        <label for="mensaje">Detalles (metros aproximados o ubicación)</label>
                        <textarea id="mensaje" name="mensaje" rows="3" placeholder="Cuéntanos qué necesitas..."></textarea>
                    </div>

                    <button type="submit" class="btn-enviar">Enviar Solicitud</button>
                </form>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Pulidos Martínez - Christian Martínez. Todos los derechos reservados.</p>
    </footer>

    <a href="https://wa.me/525611736651?text=Hola%20Christian,%20quisiera%20pedir%20informes%20sobre%20pulido%20de%20pisos." class="whatsapp-float" target="_blank" title="Enviar WhatsApp">
        💬
    </a>

</body>
</html>
