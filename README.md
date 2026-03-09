<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BANDERILLAS BLUE - Banderillas Coreanas Auténticas</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;900&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            overflow-x: hidden;
        }

        /* Header */
        header {
            background: rgba(0,0,0,0.3);
            backdrop-filter: blur(10px);
            padding: 1rem;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 3px solid #FFD700;
        }

        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 900;
            color: #FFD700;
            text-shadow: 3px 3px 0px #ff006e;
            letter-spacing: 2px;
        }

        .logo span {
            color: #00d9ff;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin-left: 2rem;
            font-weight: 600;
            transition: all 0.3s;
            position: relative;
        }

        nav a:hover {
            color: #FFD700;
            transform: translateY(-2px);
        }

        nav a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 3px;
            background: #FFD700;
            transition: width 0.3s;
        }

        nav a:hover::after {
            width: 100%;
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            padding: 4rem 1rem;
            text-align: center;
            background: radial-gradient(circle at center, rgba(255,255,255,0.1) 0%, transparent 70%);
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 900;
            margin-bottom: 1rem;
            text-shadow: 4px 4px 0px #ff006e, 8px 8px 0px rgba(0,0,0,0.3);
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .hero-badge {
            display: inline-block;
            background: #ff006e;
            color: #fff;
            padding: 0.5rem 1.5rem;
            border-radius: 50px;
            font-weight: 700;
            margin-bottom: 2rem;
            box-shadow: 0 4px 15px rgba(255,0,110,0.4);
        }

        /* Menu Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            position: relative;
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
        }

        .section-title::after {
            content: '🍢';
            position: absolute;
            right: -50px;
            top: 0;
            animation: bounce 1s infinite;
        }

        .section-title::before {
            content: '🍢';
            position: absolute;
            left: -50px;
            top: 0;
            animation: bounce 1s infinite 0.5s;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        /* Menu Grid */
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .menu-card {
            background: rgba(255,255,255,0.95);
            border-radius: 20px;
            padding: 2rem;
            color: #333;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
            border: 4px solid transparent;
        }

        .menu-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.3), transparent);
            transform: rotate(45deg);
            transition: all 0.5s;
            opacity: 0;
        }

        .menu-card:hover::before {
            animation: shine 0.5s ease-in-out;
        }

        @keyframes shine {
            0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); opacity: 0; }
            50% { opacity: 1; }
            100% { transform: translateX(100%) translateY(100%) rotate(45deg); opacity: 0; }
        }

        .menu-card:hover {
            transform: translateY(-10px) scale(1.02);
            border-color: #FFD700;
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }

        .card-header {
            display: flex;
            align-items: center;
            margin-bottom: 1.5rem;
            border-bottom: 3px solid #667eea;
            padding-bottom: 1rem;
        }

        .card-icon {
            font-size: 3rem;
            margin-right: 1rem;
            filter: drop-shadow(2px 2px 0px rgba(0,0,0,0.2));
        }

        .card-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: #667eea;
            line-height: 1.2;
        }

        .card-subtitle {
            font-size: 0.9rem;
            color: #666;
            font-weight: 600;
        }

        .menu-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.8rem 0;
            border-bottom: 1px dashed #ddd;
            transition: all 0.2s;
        }

        .menu-item:hover {
            background: rgba(102, 126, 234, 0.1);
            margin: 0 -1rem;
            padding-left: 1rem;
            padding-right: 1rem;
            border-radius: 10px;
        }

        .menu-item:last-child {
            border-bottom: none;
        }

        .item-name {
            font-weight: 600;
            display: flex;
            align-items: center;
        }

        .item-name::before {
            content: '▸';
            color: #ff006e;
            margin-right: 0.5rem;
            font-weight: 900;
        }

        .item-price {
            font-weight: 700;
            color: #ff006e;
            font-size: 1.1rem;
        }

        /* Special Cards */
        .special-card {
            background: linear-gradient(135deg, #ff006e 0%, #ff4d00 100%);
            color: #fff;
            border: 4px solid #FFD700;
        }

        .special-card .card-title,
        .special-card .item-price {
            color: #fff;
        }

        .special-card .card-subtitle {
            color: rgba(255,255,255,0.9);
        }

        .special-badge {
            position: absolute;
            top: 10px;
            right: -30px;
            background: #FFD700;
            color: #333;
            padding: 0.3rem 2rem;
            transform: rotate(45deg);
            font-size: 0.8rem;
            font-weight: 900;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }

        /* Package Cards */
        .package-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .package-card {
            background: linear-gradient(135deg, #00d9ff 0%, #00a8ff 100%);
            border-radius: 20px;
            padding: 2rem;
            color: #fff;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            position: relative;
            overflow: hidden;
            border: 4px solid #fff;
        }

        .package-card::after {
            content: '🎁';
            position: absolute;
            bottom: -20px;
            right: -20px;
            font-size: 8rem;
            opacity: 0.2;
        }

        .package-title {
            font-size: 1.8rem;
            font-weight: 900;
            margin-bottom: 0.5rem;
            text-shadow: 2px 2px 0px rgba(0,0,0,0.2);
        }

        .package-subtitle {
            font-size: 1rem;
            opacity: 0.9;
            margin-bottom: 1.5rem;
            font-weight: 600;
        }

        .package-item {
            background: rgba(255,255,255,0.2);
            padding: 1rem;
            margin-bottom: 0.8rem;
            border-radius: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            backdrop-filter: blur(5px);
            border: 2px solid rgba(255,255,255,0.3);
            transition: all 0.3s;
        }

        .package-item:hover {
            background: rgba(255,255,255,0.3);
            transform: translateX(10px);
        }

        /* Location Section */
        .location-section {
            background: rgba(0,0,0,0.2);
            border-radius: 30px;
            padding: 3rem;
            margin: 4rem 0;
            text-align: center;
            border: 3px solid #FFD700;
            position: relative;
        }

        .location-icon {
            font-size: 4rem;
            margin-bottom: 1rem;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }

        .location-text {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            font-weight: 600;
        }

        .delivery-badge {
            display: inline-block;
            background: #00d9ff;
            color: #fff;
            padding: 0.8rem 2rem;
            border-radius: 50px;
            font-weight: 700;
            margin-top: 1rem;
            box-shadow: 0 4px 15px rgba(0,217,255,0.4);
            animation: glow 2s infinite;
        }

        @keyframes glow {
            0%, 100% { box-shadow: 0 4px 15px rgba(0,217,255,0.4); }
            50% { box-shadow: 0 4px 30px rgba(0,217,255,0.8); }
        }

        /* WhatsApp Button */
        .whatsapp-container {
            position: fixed;
            bottom: 30px;
            right: 30px;
            z-index: 9999;
        }

        .whatsapp-btn {
            background: #25D366;
            color: #fff;
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.5);
            transition: all 0.3s;
            text-decoration: none;
            position: relative;
            animation: pulse-whatsapp 2s infinite;
        }

        @keyframes pulse-whatsapp {
            0%, 100% { transform: scale(1); box-shadow: 0 5px 20px rgba(37, 211, 102, 0.5); }
            50% { transform: scale(1.1); box-shadow: 0 10px 30px rgba(37, 211, 102, 0.8); }
        }

        .whatsapp-btn:hover {
            transform: scale(1.2) rotate(10deg);
            box-shadow: 0 10px 40px rgba(37, 211, 102, 0.8);
        }

        .whatsapp-tooltip {
            position: absolute;
            right: 80px;
            top: 50%;
            transform: translateY(-50%);
            background: #fff;
            color: #333;
            padding: 0.8rem 1.2rem;
            border-radius: 10px;
            font-weight: 700;
            font-size: 0.9rem;
            white-space: nowrap;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .whatsapp-tooltip::after {
            content: '';
            position: absolute;
            right: -10px;
            top: 50%;
            transform: translateY(-50%);
            border: 5px solid transparent;
            border-left-color: #fff;
        }

        .whatsapp-container:hover .whatsapp-tooltip {
            opacity: 1;
            visibility: visible;
            right: 90px;
        }

        .whatsapp-banner {
            background: #25D366;
            color: #fff;
            text-align: center;
            padding: 1rem;
            font-weight: 700;
            font-size: 1.1rem;
            margin: 2rem 0;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.3);
        }

        /* Footer */
        footer {
            background: rgba(0,0,0,0.4);
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
            border-top: 3px solid #FFD700;
        }

        .footer-text {
            font-size: 1.2rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .footer-sub {
            opacity: 0.8;
            font-size: 0.9rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .menu-grid {
                grid-template-columns: 1fr;
            }
            
            .package-grid {
                grid-template-columns: 1fr;
            }
            
            nav a {
                margin-left: 1rem;
                font-size: 0.9rem;
            }
            
            .whatsapp-container {
                bottom: 20px;
                right: 20px;
            }
            
            .whatsapp-btn {
                width: 60px;
                height: 60px;
                font-size: 2rem;
            }
            
            .location-section {
                padding: 2rem 1rem;
            }
        }

        /* Loading Animation */
        .loader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            transition: opacity 0.5s;
        }

        .loader.hidden {
            opacity: 0;
            pointer-events: none;
        }

        .loader-content {
            text-align: center;
        }

        .loader-logo {
            font-size: 4rem;
            font-weight: 900;
            color: #FFD700;
            text-shadow: 3px 3px 0px #ff006e;
            animation: loader-bounce 1s infinite;
        }

        @keyframes loader-bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        /* Scroll animations */
        .scroll-reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s;
        }

        .scroll-reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Loader -->
    <div class="loader" id="loader">
        <div class="loader-content">
            <div class="loader-logo">BLUE 🔵</div>
            <p style="margin-top: 1rem; font-weight: 600;">Cargando sabor...</p>
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="header-content">
            <div class="logo">BANDERILLAS <span>BLUE</span></div>
            <nav>
                <a href="#menu">Menú</a>
                <a href="#paquetes">Paquetes</a>
                <a href="#ubicacion">Ubicación</a>
                <a href="#contacto">Contacto</a>
            </nav>
        </div>
    </header>

    <!-- Hero -->
    <section class="hero">
        <div class="hero-badge">🔥 AUTÉNTICO SABOR COREANO 🔥</div>
        <h1>BANDERILLAS BLUE</h1>
        <p>El verdadero sabor de Corea en cada mordida. Crujientes, sabrosas y 100% irresistibles.</p>
        <div style="font-size: 3rem; margin-top: 1rem;">🌭🧀🍫</div>
    </section>

    <!-- WhatsApp Banner -->
    <div class="container">
        <div class="whatsapp-banner">
            📱 ¡Haz tu pedido ahora! Click en el botón verde de WhatsApp →
        </div>
    </div>

    <!-- Menu Section -->
    <section id="menu" class="container">
        <h2 class="section-title">Nuestro Menú</h2>
        
        <div class="menu-grid">
            <!-- Empanizado Normal -->
            <div class="menu-card scroll-reveal">
                <div class="card-header">
                    <div class="card-icon">🟡</div>
                    <div>
                        <div class="card-title">EMPANIZADO NORMAL</div>
                        <div class="card-subtitle">Pan Molido Tradicional</div>
                    </div>
                </div>
                <div class="menu-item">
                    <span class="item-name">Salchicha</span>
                    <span class="item-price">$35</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">Salchicha + Queso</span>
                    <span class="item-price">$40</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">Únicamente Queso</span>
                    <span class="item-price">$50</span>
                </div>
            </div>

            <!-- Flaming Hot -->
            <div class="menu-card special-card scroll-reveal">
                <div class="special-badge">PICOSITO</div>
                <div class="card-header">
                    <div class="card-icon">🔥</div>
                    <div>
                        <div class="card-title">FLAMING HOT</div>
                        <div class="card-subtitle">Con chile piquín</div>
                    </div>
                </div>
                <div class="menu-item">
                    <span class="item-name">Salchicha</span>
                    <span class="item-price">$40</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">Salchicha + Queso</span>
                    <span class="item-price">$45</span>
                </div>
                <div class="menu-item">
                    <span class="item-name">Únicamente Queso</span>
                    <span class="item-price">$55</span>
                </div>
            </div>

            <!-- Corazón de Chocolate -->
            <div class="menu-card scroll-reveal" style="background: linear-gradient(135deg, #5D4037 0%, #8D6E63 100%); color: #fff; border-color: #FFD700;">
                <div class="card-header">
                    <div class="card-icon">🍫</div>
                    <div>
                        <div class="card-title" style="color: #FFD700;">CORAZÓN DE CHOCOLATE</div>
                        <div class="card-subtitle" style="color: #fff;">Dulce tentación</div>
                    </div>
                </div>
                <div class="menu-item" style="border-color: rgba(255,255,255,0.3);">
                    <span class="item-name" style="color: #fff;">Kinder Delice</span>
                    <span class="item-price" style="color: #FFD700;">$45</span>
                </div>
                <div class="menu-item" style="border-color: rgba(255,255,255,0.3);">
                    <span class="item-name" style="color: #fff;">Gansito</span>
                    <span class="item-price" style="color: #FFD700;">$50</span>
                </div>
                <div class="menu-item" style="border-color: rgba(255,255,255,0.3);">
                    <span class="item-name" style="color: #fff;">ROCKO</span>
                    <span class="item-price" style="color: #FFD700;">$40</span>
                </div>
                <div class="menu-item" style="border-color: rgba(255,255,255,0.3);">
                    <span class="item-name" style="color: #fff;">Chocorrol</span>
                    <span class="item-price" style="color: #FFD700;">$50</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Paquetes Section -->
    <section id="paquetes" class="container">
        <h2 class="section-title" style="margin-top: 4rem;">Paquetes Especiales</h2>
        <p style="text-align: center; margin-bottom: 2rem; font-size: 1.1rem; opacity: 0.9;">¡La mejor combinación al mejor precio!</p>
        
        <div class="package-grid">
            <!-- Paquetes Salados -->
            <div class="package-card scroll-reveal">
                <div class="package-title">🌭 PAQUETES SALADOS</div>
                <div class="package-subtitle">Cualquier banderilla + Salchipulpos</div>
                
                <div style="margin-top: 1.5rem; font-weight: 700; font-size: 1.2rem; margin-bottom: 1rem;">Empanizado Normal:</div>
                <div class="package-item">
                    <span>Salchicha</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$55</span>
                </div>
                <div class="package-item">
                    <span>Salchicha + Queso</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$65</span>
                </div>
                <div class="package-item">
                    <span>Únicamente Queso</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$75</span>
                </div>
                
                <div style="margin-top: 1.5rem; font-weight: 700; font-size: 1.2rem; margin-bottom: 1rem; color: #ff006e;">Flaming Hot:</div>
                <div class="package-item" style="background: rgba(255,0,110,0.2); border-color: rgba(255,0,110,0.4);">
                    <span>Salchicha</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$60</span>
                </div>
                <div class="package-item" style="background: rgba(255,0,110,0.2); border-color: rgba(255,0,110,0.4);">
                    <span>Salchicha + Queso</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$70</span>
                </div>
                <div class="package-item" style="background: rgba(255,0,110,0.2); border-color: rgba(255,0,110,0.4);">
                    <span>Únicamente Queso</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$80</span>
                </div>
            </div>

            <!-- Paquetes Dulces -->
            <div class="package-card scroll-reveal" style="background: linear-gradient(135deg, #9C27B0 0%, #E91E63 100%);">
                <div class="package-title">🍫🥤 PAQUETES DULCES</div>
                <div class="package-subtitle">Cualquier banderilla dulce + Licuado</div>
                
                <div class="package-item">
                    <span>Kinder Delice</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$60</span>
                </div>
                <div class="package-item">
                    <span>Gansito</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$70</span>
                </div>
                <div class="package-item">
                    <span>ROCKO</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$60</span>
                </div>
                <div class="package-item">
                    <span>Chocorrol</span>
                    <span style="font-weight: 900; font-size: 1.2rem;">$65</span>
                </div>
                
                <div style="margin-top: 1.5rem; padding: 1rem; background: rgba(255,255,255,0.2); border-radius: 10px; text-align: center; font-weight: 700;">
                    🥤 ¡Incluye licuado de sabor a elegir!
                </div>
            </div>
        </div>
    </section>

    <!-- Ubicación -->
    <section id="ubicacion" class="container">
        <div class="location-section scroll-reveal">
            <div class="location-icon">📍</div>
            <h2 style="font-size: 2rem; margin-bottom: 1rem;">¿Dónde Estamos?</h2>
            <p class="location-text">
                Av. Morelos, Centro, No. 209<br>
                3ra Sección<br>
                <span style="color: #FFD700; font-size: 1.1rem;">(A un costado de la Mueblería Casa Santo Tomás)</span>
            </p>
            <div class="delivery-badge">
                🛵 ¡ENTREGA A DOMICILIO DISPONIBLE!
            </div>
        </div>
    </section>

    <!-- Contacto -->
    <section id="contacto" class="container" style="text-align: center; margin-bottom: 4rem;">
        <h2 class="section-title">¡Haz Tu Pedido!</h2>
        <p style="font-size: 1.2rem; margin-bottom: 2rem;">Click en el botón verde de WhatsApp o escríbenos directo:</p>
        <a href="https://wa.me/525651234036?text=¡Hola!%20Vengo%20de%20la%20página%20web%20y%20quiero%20hacer%20un%20pedido%20🌭" 
           style="display: inline-block; background: #25D366; color: #fff; padding: 1.2rem 3rem; border-radius: 50px; text-decoration: none; font-weight: 700; font-size: 1.2rem; box-shadow: 0 5px 20px rgba(37,211,102,0.4); transition: all 0.3s; margin-bottom: 1rem;">
            📱 WhatsApp: 56 5123 4036
        </a>
        <p style="opacity: 0.8; margin-top: 1rem;">Horario: Todos los días | Pedidos con anticipación</p>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-text">BANDERILLAS BLUE 🔵</div>
        <div class="footer-sub">Auténtico sabor coreano en tu ciudad</div>
        <div style="margin-top: 1rem; font-size: 2rem;">🍢🧀🌭🍫</div>
    </footer>

    <!-- WhatsApp Floating Button -->
    <div class="whatsapp-container">
        <a href="https://wa.me/525651234036?text=¡Hola!%20Vengo%20de%20la%20página%20web%20y%20quiero%20hacer%20un%20pedido%20🌭" class="whatsapp-btn" target="_blank">
            💬
        </a>
        <div class="whatsapp-tooltip">¡Haz tu pedido aquí!</div>
    </div>

    <script>
        // Hide loader after page loads
        window.addEventListener('load', () => {
            setTimeout(() => {
                document.getElementById('loader').classList.add('hidden');
            }, 1500);
        });

        // Scroll reveal animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: "0px 0px -50px 0px"
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.scroll-reveal').forEach(el => {
            observer.observe(el);
        });

        // Smooth scroll for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add parallax effect to hero
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('.hero');
            if (hero) {
                hero.style.transform = `translateY(${scrolled * 0.5}px)`;
            }
        });
    </script>
</body>
</html>
