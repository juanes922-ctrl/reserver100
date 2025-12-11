<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Añadir meta tags para accesibilidad -->
    <meta name="description" content="Londono's Immigration Advisors - Expertos en soluciones migratorias para reunir familias y construir futuros en nuevos países.">
    <meta name="keywords" content="inmigración, visas, residencia, asesoría migratoria, reunificación familiar">
    <meta name="author" content="Londono's Immigration Advisors">
    <title>Londono's Immigration Advisors | Asesoría Migratoria Profesional</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Variables de color - Escala de grises ejecutiva */
        :root {
            --primary-dark: #222222; /* Gris muy oscuro */
            --primary: #333333; /* Gris oscuro */
            --primary-light: #444444; /* Gris medio oscuro */
            --secondary: #555555; /* Gris medio */
            --accent: #777777; /* Gris acento */
            --light: #F5F5F5; /* Fondo claro */
            --dark: #111111; /* Texto muy oscuro */
            --gray: #666666; /* Texto gris */
            --light-gray: #EEEEEE; /* Gris claro */
            --white: #FFFFFF;
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s ease;
        }
        
        /* Estilos generales */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            color: var(--dark);
            line-height: 1.6;
            background-color: var(--light);
        }
        
        a {
            text-decoration: none;
            color: inherit;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            color: var(--primary-dark);
            font-size: 2.5rem;
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 70px;
            height: 3px;
            background-color: var(--accent);
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .section-title p {
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto;
            font-size: 1.1rem;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: var(--primary);
            color: var(--white);
            border: none;
            border-radius: 4px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            font-size: 1rem;
        }
        
        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: var(--shadow);
        }
        
        .btn-accent {
            background-color: var(--accent);
            color: var(--white);
        }
        
        .btn-accent:hover {
            background-color: #666666;
        }
        
        .btn-consultation {
            background-color: var(--primary-dark);
            color: var(--white);
            border: 2px solid var(--accent);
        }
        
        .btn-consultation:hover {
            background-color: var(--accent);
            color: var(--primary-dark);
        }
        
        /* Botón de WhatsApp flotante */
        .whatsapp-float {
            position: fixed;
            bottom: 25px;
            right: 25px;
            width: 60px;
            height: 60px;
            background-color: #25D366;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
            z-index: 1000;
            transition: var(--transition);
            animation: pulse-whatsapp 2s infinite;
        }
        
        @keyframes pulse-whatsapp {
            0% {
                box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
            }
            70% {
                box-shadow: 0 4px 20px rgba(37, 211, 102, 0.7);
            }
            100% {
                box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
            }
        }
        
        .whatsapp-float:hover {
            background-color: #128C7E;
            transform: scale(1.1);
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.6);
        }
        
        .whatsapp-tooltip {
            position: absolute;
            right: 70px;
            top: 50%;
            transform: translateY(-50%);
            background-color: var(--primary-dark);
            color: white;
            padding: 8px 15px;
            border-radius: 4px;
            font-size: 0.85rem;
            white-space: nowrap;
            opacity: 0;
            visibility: hidden;
            transition: var(--transition);
            box-shadow: var(--shadow);
            pointer-events: none;
        }
        
        .whatsapp-tooltip::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 100%;
            transform: translateY(-50%);
            border-width: 6px;
            border-style: solid;
            border-color: transparent transparent transparent var(--primary-dark);
        }
        
        .whatsapp-float:hover .whatsapp-tooltip {
            opacity: 1;
            visibility: visible;
            right: 75px;
        }
        
        /* Mejorar el header sticky para móviles */
        header {
            background-color: var(--white);
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 1000;
            transition: var(--transition);
        }

        /* Efecto de scroll en header */
        .header-scrolled {
            padding: 10px 0;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .header-scrolled .header-container {
            padding: 5px 0;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            transition: var(--transition);
        }
        
        .logo-container {
            display: flex;
            align-items: center;
            gap: 15px;
            transition: var(--transition);
        }
        
        .logo-img {
            height: 60px;
            width: auto;
            transition: var(--transition);
        }
        
        .header-scrolled .logo-img {
            height: 50px;
        }
        
        .logo-text {
            display: flex;
            flex-direction: column;
            transition: var(--transition);
        }
        
        .logo-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-dark);
            line-height: 1.2;
            transition: var(--transition);
        }
        
        .header-scrolled .logo-title {
            font-size: 1.3rem;
        }
        
        .logo-subtitle {
            font-size: 0.9rem;
            color: var(--secondary);
            font-weight: 500;
            letter-spacing: 0.5px;
            transition: var(--transition);
        }
        
        .header-scrolled .logo-subtitle {
            font-size: 0.8rem;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
            align-items: center;
        }
        
        nav ul li a {
            font-weight: 600;
            color: var(--primary);
            transition: var(--transition);
            position: relative;
        }
        
        nav ul li a:hover {
            color: var(--accent);
        }
        
        nav ul li a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            background-color: var(--accent);
            left: 0;
            bottom: -5px;
            transition: var(--transition);
        }
        
        nav ul li a:hover::after {
            width: 100%;
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--primary);
            cursor: pointer;
            transition: var(--transition);
        }
        
        .header-scrolled .mobile-menu-btn {
            font-size: 1.3rem;
        }
        
        /* Hero section */
        .hero {
            background: linear-gradient(rgba(34, 34, 34, 0.85), rgba(34, 34, 34, 0.9)), url('https://images.unsplash.com/photo-1551524165-6b6e5a6166f3?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            color: var(--white);
            padding: 120px 0;
            text-align: center;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 3.2rem;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .hero-btns {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        /* Sección de familias felices - flotante central */
        .happy-families {
            background-color: var(--white);
            position: relative;
            overflow: hidden;
        }
        
        .families-container {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 30px;
            flex-wrap: wrap;
            position: relative;
        }
        
        .family-card {
            width: 280px;
            height: 280px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            position: relative;
            transition: var(--transition);
            animation: float 6s ease-in-out infinite;
        }
        
        .family-card:nth-child(1) {
            animation-delay: 0s;
            transform: translateY(0px);
        }
        
        .family-card:nth-child(2) {
            animation-delay: 2s;
            transform: translateY(0px);
        }
        
        .family-card:nth-child(3) {
            animation-delay: 4s;
            transform: translateY(0px);
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
        
        .family-card:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .family-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }
        
        .family-card:hover img {
            transform: scale(1.1);
        }
        
        .family-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
            color: white;
            padding: 20px;
            transform: translateY(100%);
            transition: var(--transition);
        }
        
        .family-card:hover .family-overlay {
            transform: translateY(0);
        }
        
        /* Sección Quiénes Somos con imagen */
        .quienes-somos {
            background-color: var(--light-gray);
            position: relative;
        }
        
        .quienes-content {
            display: flex;
            align-items: center;
            gap: 60px;
            max-width: 1100px;
            margin: 0 auto;
        }
        
        .quienes-text {
            flex: 1;
        }
        
        .quienes-text h2 {
            color: var(--primary-dark);
            font-size: 2.2rem;
            margin-bottom: 25px;
            position: relative;
            display: inline-block;
        }
        
        .quienes-text h2::after {
            content: '';
            position: absolute;
            width: 60px;
            height: 3px;
            background-color: var(--accent);
            bottom: -10px;
            left: 0;
        }
        
        .quienes-text p {
            color: var(--gray);
            font-size: 1.1rem;
            line-height: 1.8;
            margin-bottom: 20px;
        }
        
        .quienes-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }
        
        .quienes-image:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .quienes-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: var(--transition);
        }
        
        .quienes-image:hover img {
            transform: scale(1.03);
        }
        
        /* Sección unificada de testimonios con movimiento */
        .testimonios-unificados {
            background-color: var(--white);
            position: relative;
            overflow: hidden;
            padding: 100px 0;
        }
        
        .testimonios-container {
            position: relative;
            max-width: 1300px;
            margin: 0 auto;
            padding: 0 60px;
        }
        
        .testimonios-track {
            display: flex;
            transition: transform 0.5s ease;
            gap: 30px;
            padding: 20px 0;
        }
        
        .testimonio-card {
            min-width: calc(33.333% - 20px);
            background-color: var(--light-gray);
            border-radius: 10px;
            padding: 40px 35px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
            border-left: 5px solid var(--accent);
            animation: card-float 4s ease-in-out infinite;
        }
        
        .testimonio-card:nth-child(odd) {
            animation-delay: 0s;
        }
        
        .testimonio-card:nth-child(even) {
            animation-delay: 2s;
        }
        
        @keyframes card-float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        
        .testimonio-card:hover {
            transform: translateY(-15px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
            z-index: 2;
        }
        
        .testimonio-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--accent), var(--primary));
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.5s ease;
        }
        
        .testimonio-card:hover::before {
            transform: scaleX(1);
        }
        
        .testimonio-icon {
            color: var(--accent);
            font-size: 2rem;
            margin-bottom: 20px;
            opacity: 0.8;
        }
        
        .testimonio-text {
            font-style: italic;
            color: var(--gray);
            margin-bottom: 25px;
            font-size: 1.15rem;
            line-height: 1.7;
        }
        
        .testimonio-author {
            color: var(--primary-dark);
            font-weight: 600;
            font-size: 1.2rem;
            margin-bottom: 5px;
        }
        
        .testimonio-details {
            color: var(--secondary);
            font-size: 0.95rem;
        }
        
        .testimonio-badge {
            position: absolute;
            top: 20px;
            right: 20px;
            background-color: var(--primary);
            color: var(--white);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
        }
        
        .testimonios-btn {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: var(--primary-dark);
            color: var(--white);
            border: none;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            font-size: 1.8rem;
            cursor: pointer;
            z-index: 10;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
            box-shadow: var(--shadow);
        }
        
        .testimonios-btn:hover {
            background-color: var(--accent);
            transform: translateY(-50%) scale(1.1);
        }
        
        .testimonios-btn.prev {
            left: 0;
        }
        
        .testimonios-btn.next {
            right: 0;
        }
        
        .testimonios-dots {
            display: flex;
            justify-content: center;
            margin-top: 40px;
            gap: 10px;
        }
        
        .testimonios-dot {
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background-color: var(--light-gray);
            border: 2px solid var(--accent);
            cursor: pointer;
            transition: var(--transition);
        }
        
        .testimonios-dot.active {
            background-color: var(--accent);
            transform: scale(1.2);
        }
        
        /* Efectos de partículas flotantes para testimonios */
        .floating-particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
            overflow: hidden;
        }
        
        .particle {
            position: absolute;
            background-color: var(--light-gray);
            border-radius: 50%;
            opacity: 0.1;
        }
        
        .particle:nth-child(1) {
            width: 20px;
            height: 20px;
            top: 10%;
            left: 5%;
            animation: particle-float-1 20s infinite linear;
        }
        
        .particle:nth-child(2) {
            width: 15px;
            height: 15px;
            top: 30%;
            right: 10%;
            animation: particle-float-2 25s infinite linear;
        }
        
        .particle:nth-child(3) {
            width: 25px;
            height: 25px;
            bottom: 20%;
            left: 15%;
            animation: particle-float-3 30s infinite linear;
        }
        
        .particle:nth-child(4) {
            width: 10px;
            height: 10px;
            bottom: 40%;
            right: 20%;
            animation: particle-float-4 15s infinite linear;
        }
        
        @keyframes particle-float-1 {
            0% { transform: translate(0, 0) rotate(0deg); }
            100% { transform: translate(100px, 100px) rotate(360deg); }
        }
        
        @keyframes particle-float-2 {
            0% { transform: translate(0, 0) rotate(0deg); }
            100% { transform: translate(-150px, 50px) rotate(-360deg); }
        }
        
        @keyframes particle-float-3 {
            0% { transform: translate(0, 0) rotate(0deg); }
            100% { transform: translate(80px, -80px) rotate(180deg); }
        }
        
        @keyframes particle-float-4 {
            0% { transform: translate(0, 0) rotate(0deg); }
            100% { transform: translate(-100px, -50px) rotate(-180deg); }
        }
        
        /* Servicios */
        .services {
            background-color: var(--white);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: var(--white);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            padding: 30px;
            text-align: center;
            border-top: 4px solid var(--primary);
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 20px;
        }
        
        .service-card h3 {
            color: var(--primary-dark);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .service-card p {
            color: var(--gray);
            margin-bottom: 20px;
        }
        
        /* Sobre nosotros */
        .about {
            background-color: var(--light-gray);
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-img {
            flex: 1;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }
        
        .about-img img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            color: var(--primary-dark);
            font-size: 1.8rem;
            margin-bottom: 20px;
        }
        
        .about-text p {
            margin-bottom: 20px;
            color: var(--gray);
        }
        
        .about-features {
            margin-top: 30px;
        }
        
        .feature {
            display: flex;
            align-items: flex-start;
            margin-bottom: 20px;
        }
        
        .feature-icon {
            color: var(--accent);
            font-size: 1.2rem;
            margin-right: 15px;
            margin-top: 5px;
        }
        
        /* Contacto */
        .contact {
            background-color: var(--primary-dark);
            color: var(--white);
        }
        
        .contact .section-title h2 {
            color: var(--white);
        }
        
        .contact .section-title p {
            color: rgba(255, 255, 255, 0.8);
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 50px;
        }
        
        .contact-info h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: var(--light-gray);
        }
        
        .contact-info p {
            margin-bottom: 15px;
            opacity: 0.9;
        }
        
        .contact-info i {
            color: var(--light-gray);
            margin-right: 10px;
            width: 20px;
        }
        
        .contact-form input,
        .contact-form textarea,
        .contact-form select {
            width: 100%;
            padding: 12px 15px;
            margin-bottom: 20px;
            border: none;
            border-radius: 4px;
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--white);
            font-size: 1rem;
        }
        
        .contact-form input::placeholder,
        .contact-form textarea::placeholder,
        .contact-form select {
            color: rgba(255, 255, 255, 0.7);
        }
        
        .contact-form textarea {
            height: 150px;
            resize: vertical;
        }
        
        /* Mapa de Google Maps */
        .map-container {
            margin-top: 60px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            position: relative;
        }
        
        .map-title {
            text-align: center;
            margin-bottom: 20px;
            color: var(--light-gray);
            font-size: 1.5rem;
        }
        
        .map-frame {
            width: 100%;
            height: 400px;
            border: none;
            filter: grayscale(20%) contrast(90%);
            transition: var(--transition);
        }
        
        .map-frame:hover {
            filter: grayscale(0%) contrast(100%);
        }
        
        .map-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(34, 34, 34, 0.8), transparent);
            color: white;
            padding: 20px;
            text-align: center;
        }
        
        .map-overlay h4 {
            margin-bottom: 5px;
            font-size: 1.2rem;
        }
        
        .map-overlay p {
            opacity: 0.9;
            font-size: 0.95rem;
        }
        
        /* Sección CTA antes del footer */
        .cta-section {
            background: linear-gradient(rgba(34, 34, 34, 0.85), rgba(34, 34, 34, 0.9)), url('https://images.unsplash.com/photo-1497366754035-f200968a6e72?ixlib=rb-4.0.3&auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: var(--white);
            padding: 100px 0;
            text-align: center;
            position: relative;
        }
        
        .cta-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }
        
        .cta-content h2 {
            font-size: 2.8rem;
            margin-bottom: 25px;
            line-height: 1.2;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
        }
        
        .cta-content p {
            font-size: 1.3rem;
            margin-bottom: 40px;
            opacity: 0.95;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
        }
        
        .btn-cta {
            display: inline-block;
            padding: 18px 45px;
            background-color: #25D366; /* Color WhatsApp */
            color: var(--white);
            border: none;
            border-radius: 8px;
            font-weight: 700;
            cursor: pointer;
            transition: var(--transition);
            font-size: 1.3rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            animation: pulse-cta 2s infinite;
        }
        
        @keyframes pulse-cta {
            0% {
                transform: scale(1);
                box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            }
            50% {
                transform: scale(1.05);
                box-shadow: 0 12px 30px rgba(37, 211, 102, 0.4);
            }
            100% {
                transform: scale(1);
                box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            }
        }
        
        .btn-cta:hover {
            background-color: #128C7E;
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 35px rgba(37, 211, 102, 0.5);
        }
        
        /* Enlaces de dirección con Google Maps */
        .address-link {
            color: var(--light-gray);
            transition: var(--transition);
            text-decoration: none;
            display: inline-block;
            position: relative;
        }
        
        .address-link:hover {
            color: var(--white);
            transform: translateY(-2px);
        }
        
        .address-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 1px;
            background-color: var(--white);
            left: 0;
            bottom: -2px;
            transition: var(--transition);
        }
        
        .address-link:hover::after {
            width: 100%;
        }
        
        .map-icon {
            color: var(--light-gray);
            margin-right: 8px;
            transition: var(--transition);
        }
        
        .address-link:hover .map-icon {
            color: var(--white);
        }
        
        /* Footer */
        footer {
            background-color: var(--primary);
            color: var(--white);
            padding: 60px 0 30px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-col h4 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: var(--light-gray);
        }
        
        .footer-col p {
            opacity: 0.9;
            margin-bottom: 15px;
        }
        
        .footer-links li {
            list-style: none;
            margin-bottom: 10px;
        }
        
        .footer-links a {
            opacity: 0.9;
            transition: var(--transition);
        }
        
        .footer-links a:hover {
            opacity: 1;
            color: var(--light-gray);
            padding-left: 5px;
        }
        
        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-icons a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: var(--transition);
        }
        
        .social-icons a:hover {
            background-color: var(--light-gray);
            color: var(--primary-dark);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }
        
        /* Responsive */
        @media (max-width: 992px) {
            .about-content {
                flex-direction: column;
            }
            
            .about-img, .about-text {
                width: 100%;
            }
            
            .families-container {
                gap: 20px;
            }
            
            .family-card {
                width: 250px;
                height: 250px;
            }
            
            .quienes-content {
                flex-direction: column;
                gap: 40px;
            }
            
            .quienes-text h2::after {
                left: 50%;
                transform: translateX(-50%);
            }
            
            .testimonio-card {
                min-width: calc(50% - 15px);
            }
            
            .cta-content h2 {
                font-size: 2.4rem;
            }
            
            .cta-content p {
                font-size: 1.2rem;
            }
        }
        
        @media (max-width: 768px) {
            .header-container {
                padding: 15px 0;
            }
            
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: var(--white);
                flex-direction: column;
                padding: 20px;
                box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
                text-align: center;
                gap: 20px;
            }
            
            .header-scrolled nav ul {
                top: 80px;
            }
            
            nav ul.show {
                display: flex;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
            
            .hero-btns {
                flex-direction: column;
                align-items: center;
            }
            
            .btn {
                width: 100%;
                max-width: 300px;
            }
            
            .logo-img {
                height: 50px;
            }
            
            .header-scrolled .logo-img {
                height: 40px;
            }
            
            .logo-title {
                font-size: 1.3rem;
            }
            
            .header-scrolled .logo-title {
                font-size: 1.1rem;
            }
            
            .logo-subtitle {
                font-size: 0.8rem;
            }
            
            .header-scrolled .logo-subtitle {
                font-size: 0.7rem;
            }
            
            .quienes-text h2 {
                font-size: 1.9rem;
            }
            
            .testimonios-container {
                padding: 0 50px;
            }
            
            .testimonio-card {
                min-width: calc(100% - 0px);
            }
            
            .testimonios-btn {
                width: 50px;
                height: 50px;
                font-size: 1.5rem;
            }
            
            .header-scrolled .header-container {
                padding: 8px 0;
            }
            
            .map-frame {
                height: 300px;
            }
            
            .cta-section {
                padding: 80px 0;
                background-attachment: scroll;
            }
            
            .cta-content h2 {
                font-size: 2rem;
            }
            
            .cta-content p {
                font-size: 1.1rem;
            }
            
            .btn-cta {
                padding: 15px 35px;
                font-size: 1.1rem;
            }
            
            .whatsapp-float {
                width: 55px;
                height: 55px;
                font-size: 24px;
                bottom: 20px;
                right: 20px;
            }
        }
        
        @media (max-width: 576px) {
            section {
                padding: 60px 0;
            }
            
            .hero {
                padding: 80px 0;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .families-container {
                flex-direction: column;
            }
            
            .family-card {
                width: 280px;
                height: 280px;
            }
            
            .logo-container {
                gap: 10px;
            }
            
            .logo-img {
                height: 45px;
            }
            
            .header-scrolled .logo-img {
                height: 35px;
            }
            
            .logo-title {
                font-size: 1.1rem;
            }
            
            .header-scrolled .logo-title {
                font-size: 1rem;
            }
            
            .logo-subtitle {
                font-size: 0.75rem;
            }
            
            .header-scrolled .logo-subtitle {
                font-size: 0.65rem;
            }
            
            .quienes-text h2 {
                font-size: 1.7rem;
                text-align: center;
            }
            
            .quienes-text p {
                font-size: 1rem;
                text-align: center;
            }
            
            .testimonios-container {
                padding: 0 40px;
            }
            
            .testimonio-card {
                padding: 30px 25px;
            }
            
            .testimonio-text {
                font-size: 1.1rem;
            }
            
            .testimonios-btn {
                width: 45px;
                height: 45px;
                font-size: 1.3rem;
            }
            
            .header-scrolled .header-container {
                padding: 5px 0;
            }
            
            .map-frame {
                height: 250px;
            }
            
            .map-title {
                font-size: 1.3rem;
            }
            
            .cta-section {
                padding: 70px 0;
            }
            
            .cta-content h2 {
                font-size: 1.8rem;
            }
            
            .cta-content p {
                font-size: 1rem;
            }
            
            .btn-cta {
                padding: 14px 30px;
                font-size: 1rem;
            }
            
            .whatsapp-float {
                width: 50px;
                height: 50px;
                font-size: 22px;
                bottom: 15px;
                right: 15px;
            }
            
            .whatsapp-tooltip {
                display: none; /* Ocultar tooltip en móviles */
            }
        }
    </style>
</head>
<body>
    <!-- Botón de WhatsApp flotante -->
    <a href="https://wa.me/15551234567?text=Hola,%20me%20interesa%20saber%20más%20sobre%20sus%20servicios%20de%20inmigración" 
       target="_blank" 
       rel="noopener noreferrer" 
       class="whatsapp-float">
        <i class="fab fa-whatsapp"></i>
        <div class="whatsapp-tooltip">¡Chatea con nosotros!</div>
    </a>
    
    <!-- Header y Navegación -->
    <header>
        <div class="container header-container">
            <div class="logo-container">
                <img src="https://thumbs.dreamstime.com/z/dise%C3%B1o-del-logotipo-de-la-letra-lia-en-fondo-blanco-concepto-logo-carta-inicio-creativo-designlia-letras-246951203.jpg?ct=jpeg" alt="Logo LIA - Londono's Immigration Advisors" class="logo-img">
                <div class="logo-text">
                    <div class="logo-title">Londono's</div>
                    <div class="logo-subtitle">Immigration Advisors</div>
                </div>
            </div>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav>
                <ul id="navMenu">
                    <li><a href="#home">Inicio</a></li>
                    <li><a href="#families">Familias Felices</a></li>
                    <li><a href="#services">Servicios</a></li>
                    <li><a href="#quienes-somos">Quiénes Somos</a></li>
                    <li><a href="#testimonios">Testimonios</a></li>
                    <li><a href="#about">Nosotros</a></li>
                    <li><a href="#contact">Contacto</a></li>
                    <li><a href="#contact" class="btn btn-consultation">Agenda tu consulta gratuita</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Sección Hero -->
    <section class="hero" id="home">
        <div class="container hero-content">
            <h1>Londono's Immigration Advisors</h1>
            <p>Expertos en soluciones migratorias que unen familias y construyen futuros. Más de 15 años ayudando a personas a alcanzar sus sueños en nuevos países.</p>
            <div class="hero-btns">
                <a href="#contact" class="btn">Solicitar Consulta</a>
                <a href="#families" class="btn btn-accent">Ver Historias de Éxito</a>
            </div>
        </div>
    </section>

    <!-- Sección de Familias Felices -->
    <section class="happy-families" id="families">
        <div class="container">
            <div class="section-title">
                <h2>Familias Felices Reunidas</h2>
                <p>Hemos ayudado a cientos de familias a reunirse y comenzar nuevas vidas en diferentes países alrededor del mundo.</p>
            </div>
            
            <div class="families-container">
                <div class="family-card">
                    <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Familia reunida celebrando">
                    <div class="family-overlay">
                        <h4>Familia Rodríguez</h4>
                        <p>Reunidos en Canadá después de 2 años</p>
                    </div>
                </div>
                
                <div class="family-card">
                    <img src="https://images.unsplash.com/photo-1511988617509-a57c8a288659?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Familia sonriendo juntos">
                    <div class="family-overlay">
                        <h4>Familia García</h4>
                        <p>Nueva vida en Australia desde 2021</p>
                    </div>
                </div>
                
                <div class="family-card">
                    <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Padres e hijos felices">
                    <div class="family-overlay">
                        <h4>Familia Martínez</h4>
                        <p>Residencia permanente en EE.UU. obtenida</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Servicios -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Nuestros Servicios</h2>
                <p>Ofrecemos asesoría especializada en todos los aspectos del proceso migratorio, con un enfoque personalizado y estratégico.</p>
            </div>
            
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-briefcase"></i>
                    </div>
                    <h3>Visas de Trabajo</h3>
                    <p>Asesoramiento completo para la obtención de visas laborales en diferentes países, adaptándonos a las necesidades específicas de profesionales y empresas.</p>
                    <a href="#" class="btn">Más información</a>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-graduation-cap"></i>
                    </div>
                    <h3>Visas de Estudio</h3>
                    <p>Guiamos a estudiantes en el proceso de obtención de visas para programas académicos en el extranjero, asegurando el cumplimiento de todos los requisitos.</p>
                    <a href="#" class="btn">Más información</a>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-home"></i>
                    </div>
                    <h3>Residencia Permanente</h3>
                    <p>Asesoría especializada en procesos de residencia permanente, incluyendo evaluación de elegibilidad y preparación de documentación.</p>
                    <a href="#" class="btn">Más información</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Quiénes Somos con Imagen -->
    <section class="quienes-somos" id="quienes-somos">
        <div class="container">
            <div class="quienes-content">
                <div class="quienes-text">
                    <h2>Quiénes Somos</h2>
                    <p>Somos una compañía dedicada a brindar servicios y trámites de inmigración, comprometidos en ayudarte a lograr tu sueño de vivir y trabajar en los Estados Unidos. Nuestro equipo está compuesto por personal calificado y certificado que te acompañará en cada paso del proceso.</p>
                </div>
                <div class="quienes-image">
                    <img src="https://images.unsplash.com/photo-1573164713988-8665fc963095?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Equipo de trabajo de Londono's Immigration Advisors">
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Unificada de Testimonios con Movimiento -->
    <section class="testimonios-unificados" id="testimonios">
        <div class="floating-particles">
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
        </div>
        
        <div class="container">
            <div class="section-title">
                <h2>Testimonios de Nuestros Clientes</h2>
                <p>Historias reales de personas que han logrado sus sueños migratorios con nuestra ayuda profesional.</p>
            </div>
            
            <!-- Añadir roles ARIA al carrusel -->
            <div class="testimonios-container" role="region" aria-label="Testimonios de clientes">
                <button class="testimonios-btn prev" aria-label="Testimonio anterior">
                    <i class="fas fa-chevron-left" aria-hidden="true"></i>
                </button>
                
                <div class="testimonios-track" role="list">
                    <!-- Cada testimonio debe tener role="listitem" -->
                    <!-- Testimonio 1 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Éxito</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Gracias a Londono's Immigration Advisors, mi familia y yo pudimos reunirnos en Canadá después de años de separación. Su profesionalismo y apoyo emocional fueron invaluables en cada etapa del proceso."</p>
                        <div class="testimonio-author">Carlos Mendoza</div>
                        <div class="testimonio-details">Reunificación familiar en Canadá - 2022</div>
                    </div>
                    
                    <!-- Testimonio 2 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Rápido</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Obtuve mi visa de trabajo para Australia en tiempo récord. El equipo de Londono's fue extremadamente detallista y me guió en cada paso del proceso, incluso con situaciones complicadas."</p>
                        <div class="testimonio-author">Ana Lucía Fernández</div>
                        <div class="testimonio-details">Visa de trabajo en Australia - 2021</div>
                    </div>
                    
                    <!-- Testimonio 3 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Experto</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Después de varios intentos fallidos con otras agencias, Londono's logró conseguirme la residencia permanente en Estados Unidos. ¡Son verdaderos expertos! Su conocimiento marcó la diferencia."</p>
                        <div class="testimonio-author">Roberto Jiménez</div>
                        <div class="testimonio-details">Residencia permanente en EE.UU. - 2023</div>
                    </div>
                    
                    <!-- Testimonio 4 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Inversión</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Como inversionista, necesitaba orientación experta para el proceso de visa EB-5. Londono's no solo me guió perfectamente, sino que también me conectó con recursos clave."</p>
                        <div class="testimonio-author">María González</div>
                        <div class="testimonio-details">Visa de inversionista EB-5 - 2022</div>
                    </div>
                    
                    <!-- Testimonio 5 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Nueva Zelanda</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Mi esposo y yo logramos la visa de trabajo para Nueva Zelanda en solo 4 meses gracias a Londono's. Su asesoría detallada y su conocimiento de los requisitos específicos hicieron toda la diferencia."</p>
                        <div class="testimonio-author">Patricia Sánchez</div>
                        <div class="testimonio-details">Visa de trabajo en Nueva Zelanda - 2023</div>
                    </div>
                    
                    <!-- Testimonio 6 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Estudiante</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Después de 3 años de intentos fallidos, Londono's Immigration Advisors logró que aprobaran mi visa de estudiante para el Reino Unido. Su paciencia y conocimiento fueron fundamentales."</p>
                        <div class="testimonio-author">Diego Ramírez</div>
                        <div class="testimonio-details">Visa de estudiante en Reino Unido - 2022</div>
                    </div>
                    
                    <!-- Testimonio 7 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Canadá</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Mi proceso de residencia permanente en Canadá fue complejo debido a mi profesión. Londono's manejó cada detalle con precisión y logramos la aprobación en tiempo récord. ¡Excelente servicio!"</p>
                        <div class="testimonio-author">Dr. Fernando López</div>
                        <div class="testimonio-details">Residencia permanente en Canadá - 2023</div>
                    </div>
                    
                    <!-- Testimonio 8 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Alemania</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Como ingeniero, necesitaba una visa de trabajo para Alemania. Londono's no solo me ayudó con el proceso, sino que también me orientó sobre los requisitos específicos para mi profesión. ¡Altamente recomendados!"</p>
                        <div class="testimonio-author">Andrés Martínez</div>
                        <div class="testimonio-details">Visa de trabajo en Alemania - 2022</div>
                    </div>
                    
                    <!-- Testimonio 9 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">España</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Logramos la reunificación familiar en España gracias al apoyo de Londono's. Su equipo fue paciente y comprensivo durante todo el proceso, especialmente con los trámites burocráticos complejos."</p>
                        <div class="testimonio-author">Familia Herrera</div>
                        <div class="testimonio-details">Reunificación familiar en España - 2023</div>
                    </div>
                    
                    <!-- Testimonio 10 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Portugal</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Mi visa de inversionista para Portugal fue aprobada gracias a la asesoría experta de Londono's. Su conocimiento del sistema portugués y su atención al detalle fueron impresionantes."</p>
                        <div class="testimonio-author">Ricardo Gómez</div>
                        <div class="testimonio-details">Visa de inversionista en Portugal - 2022</div>
                    </div>
                    
                    <!-- Testimonio 11 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Francia</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"Después de un rechazo inicial, Londono's ayudó a mi hija a obtener su visa de estudio para Francia. Su estrategia de apelación fue brillante y logramos la aprobación en la segunda oportunidad."</p>
                        <div class="testimonio-author">Sofía Castillo</div>
                        <div class="testimonio-details">Visa de estudio en Francia - 2023</div>
                    </div>
                    
                    <!-- Testimonio 12 -->
                    <div class="testimonio-card" role="listitem">
                        <div class="testimonio-badge">Japón</div>
                        <div class="testimonio-icon">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <p class="testimonio-text">"La visa de trabajo para Japón que obtuve con Londono's superó todas mis expectativas. Su equipo multilingüe y su conocimiento de la cultura japonesa hicieron la diferencia en mi aplicación."</p>
                        <div class="testimonio-author">Camila Rodríguez</div>
                        <div class="testimonio-details">Visa de trabajo en Japón - 2022</div>
                    </div>
                </div>
                
                <button class="testimonios-btn next" aria-label="Siguiente testimonio">
                    <i class="fas fa-chevron-right" aria-hidden="true"></i>
                </button>
                
                <div class="testimonios-dots">
                    <div class="testimonios-dot active" data-slide="0"></div>
                    <div class="testimonios-dot" data-slide="1"></div>
                    <div class="testimonios-dot" data-slide="2"></div>
                    <div class="testimonios-dot" data-slide="3"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Sobre Nosotros -->
    <section class="about" id="about">
        <div class="container">
            <div class="section-title">
                <h2>Nuestro Equipo</h2>
                <p>Conoce al equipo de expertos que hace posible cada historia de éxito migratorio.</p>
            </div>
            
            <div class="about-content">
                <div class="about-img">
                    <img src="https://images.unsplash.com/photo-1551836026-d5c2c5af78e4?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Equipo de Londono's Immigration Advisors">
                </div>
                
                <div class="about-text">
                    <h3>Expertos en Soluciones Migratorias</h3>
                    <p>En Londono's Immigration Advisors entendemos que los procesos migratorios no son solo trámites legales, sino sueños y esperanzas de personas y familias. Nuestro equipo combina conocimiento legal profundo con sensibilidad humana.</p>
                    <p>Nos especializamos en casos complejos y ofrecemos acompañamiento personalizado desde el inicio hasta la conclusión exitosa de cada proceso.</p>
                    
                    <div class="about-features">
                        <div class="feature">
                            <div class="feature-icon">
                                <i class="fas fa-check-circle"></i>
                            </div>
                            <div>
                                <h4>15+ Años de Experiencia</h4>
                                <p>Hemos ayudado a más de 5,000 familias en sus procesos migratorios.</p>
                            </div>
                        </div>
                        
                        <div class="feature">
                            <div class="feature-icon">
                                <i class="fas fa-check-circle"></i>
                            </div>
                            <div>
                                <h4>Equipo Multilingüe</h4>
                                <p>Nuestros asesores hablan inglés, español, francés y mandarín.</p>
                            </div>
                        </div>
                        
                        <div class="feature">
                            <div class="feature-icon">
                                <i class="fas fa-check-circle"></i>
                            </div>
                            <div>
                                <h4>Enfoque Personalizado</h4>
                                <p>Cada caso recibe atención individualizada y estrategias a medida.</p>
                            </div>
                        </div>
                    </div>
                    
                    <a href="#contact" class="btn">Contáctenos</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Contacto con Mapa de Google Maps -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Contáctenos</h2>
                <p>Póngase en contacto con nosotros para una consulta inicial gratuita y evalúe cómo podemos ayudarle en su proceso migratorio.</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Información de Contacto</h3>
                    <p>
                        <i class="fas fa-map-marker-alt map-icon"></i>
                        <a href="https://www.google.com/maps/search/?api=1&query=2193+Aquifer+Lane+Davenport+FL+33837" 
                           target="_blank" 
                           rel="noopener noreferrer" 
                           class="address-link">
                            2193 Aquifer Lane, Davenport, FL 33837
                        </a>
                    </p>
                    <p><i class="fas fa-phone"></i> +1 (555) 123-4567</p>
                    <p><i class="fas fa-envelope"></i> info@londonosimmigration.com</p>
                    <p><i class="fas fa-clock"></i> Lun-Vie: 9:00 AM - 6:00 PM</p>
                    
                    <h3 style="margin-top: 30px;">Síganos</h3>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                
                <div class="contact-form">
                    <form id="contactForm">
                        <input type="text" name="nombre" placeholder="Nombre completo" required>
                        <input type="email" name="email" placeholder="Correo electrónico" required>
                        <input type="tel" name="telefono" placeholder="Teléfono">
                        <select name="servicio" style="width: 100%; padding: 12px 15px; margin-bottom: 20px; border: none; border-radius: 4px; background-color: rgba(255, 255, 255, 0.1); color: var(--white); font-size: 1rem;">
                            <option value="" disabled selected>Seleccione un servicio</option>
                            <option value="work">Visas de Trabajo</option>
                            <option value="study">Visas de Estudio</option>
                            <option value="residence">Residencia Permanente</option>
                            <option value="family">Reunificación Familiar</option>
                            <option value="investment">Inversión y Negocios</option>
                        </select>
                        <textarea name="mensaje" placeholder="Su mensaje" required></textarea>
                        <button type="submit" class="btn btn-accent">Enviar Mensaje</button>
                    </form>
                </div>
            </div>
            
            <!-- Mapa de Google Maps -->
            <div class="map-container">
                <h3 class="map-title">Nuestra Ubicación</h3>
                <iframe 
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3508.424715866224!2d-81.64843632416694!3d28.42446607577829!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x88dd7a5d3e3b5a7b%3A0x8c1c7e7b3b5c5a5d!2s2193%20Aquifer%20Ln%2C%20Davenport%2C%20FL%2033837%2C%20EE.%20UU.!5e0!3m2!1ses!2ses!4v1680105600000!5m2!1ses!2ses" 
                    class="map-frame" 
                    allowfullscreen="" 
                    loading="lazy" 
                    referrerpolicy="no-referrer-when-downgrade"
                    title="Ubicación de Londono's Immigration Advisors en Google Maps">
                </iframe>
                <div class="map-overlay">
                    <h4>Londono's Immigration Advisors</h4>
                    <p>2193 Aquifer Lane, Davenport, FL 33837</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección CTA antes del Footer -->
    <section class="cta-section">
        <div class="container">
            <div class="cta-content">
                <h2>¿Listo para comenzar tu proceso migratorio?</h2>
                <p>¡Contáctanos hoy mismo! Nuestro equipo de expertos está listo para guiarte en cada paso del camino hacia tu nueva vida en el extranjero.</p>
                <a href="#contact" class="btn-cta">Agenda tu consulta gratis</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-col">
                    <div class="logo-container" style="align-items: flex-start;">
                        <img src="https://thumbs.dreamstime.com/z/dise%C3%B1o-del-logotipo-de-la-letra-lia-en-fondo-blanco-concepto-logo-carta-inicio-creativo-designlia-letras-246951203.jpg?ct=jpeg" alt="Logo LIA - Londono's Immigration Advisors" class="logo-img" style="height: 50px;">
                        <div class="logo-text">
                            <div class="logo-title">Londono's</div>
                            <div class="logo-subtitle">Immigration Advisors</div>
                        </div>
                    </div>
                    <p>Londono's Immigration Advisors es una firma de asesoría migratoria que ofrece soluciones personalizadas y estratégicas para personas y familias.</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                    </div>
                </div>
                
                <div class="footer-col">
                    <h4>Enlaces Rápidos</h4>
                    <ul class="footer-links">
                        <li><a href="#home">Inicio</a></li>
                        <li><a href="#families">Familias Felices</a></li>
                        <li><a href="#services">Servicios</a></li>
                        <li><a href="#quienes-somos">Quiénes Somos</a></li>
                        <li><a href="#testimonios">Testimonios</a></li>
                        <li><a href="#about">Nuestro Equipo</a></li>
                        <li><a href="#contact">Contacto</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h4>Servicios</h4>
                    <ul class="footer-links">
                        <li><a href="#">Visas de Trabajo</a></li>
                        <li><a href="#">Visas de Estudio</a></li>
                        <li><a href="#">Residencia Permanente</a></li>
                        <li><a href="#">Reunificación Familiar</a></li>
                        <li><a href="#">Inversión y Negocios</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h4>Contacto</h4>
                    <p>
                        <i class="fas fa-map-marker-alt map-icon"></i>
                        <a href="https://www.google.com/maps/search/?api=1&query=2193+Aquifer+Lane+Davenport+FL+33837" 
                           target="_blank" 
                           rel="noopener noreferrer" 
                           class="address-link">
                            2193 Aquifer Lane, Davenport, FL 33837
                        </a>
                    </p>
                    <p><i class="fas fa-phone"></i> +1 (555) 123-4567</p>
                    <p><i class="fas fa-envelope"></i> info@londonosimmigration.com</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 Londono's Immigration Advisors. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // Menú móvil
        document.getElementById('mobileMenuBtn').addEventListener('click', function() {
            document.getElementById('navMenu').classList.toggle('show');
            this.querySelector('i').classList.toggle('fa-bars');
            this.querySelector('i').classList.toggle('fa-times');
        });
        
        // Cerrar menú al hacer clic en un enlace
        document.querySelectorAll('#navMenu a').forEach(link => {
            link.addEventListener('click', function() {
                document.getElementById('navMenu').classList.remove('show');
                document.getElementById('mobileMenuBtn').querySelector('i').classList.add('fa-bars');
                document.getElementById('mobileMenuBtn').querySelector('i').classList.remove('fa-times');
            });
        });
        
        // Mejorar el manejo del formulario
        document.getElementById('contactForm').addEventListener('submit', async function(e) {
            e.preventDefault();
            
            // Validación básica
            const formData = new FormData(this);
            const nombre = formData.get('nombre') || this.querySelector('input[type="text"]').value;
            const email = formData.get('email') || this.querySelector('input[type="email"]').value;
            
            if (!nombre || !email) {
                alert('Por favor, complete los campos requeridos.');
                return;
            }
            
            // Validación de formato de email
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailRegex.test(email)) {
                alert('Por favor, ingrese un correo electrónico válido.');
                return;
            }
            
            // Mostrar estado de envío
            const submitBtn = this.querySelector('button[type="submit"]');
            const originalText = submitBtn.textContent;
            submitBtn.textContent = 'Enviando...';
            submitBtn.disabled = true;
            
            try {
                // En un caso real, aquí iría una petición fetch a un servidor
                await new Promise(resolve => setTimeout(resolve, 1500)); // Simulación de envío
                
                alert('¡Mensaje enviado con éxito! Nos pondremos en contacto con usted en un plazo de 24 horas.');
                this.reset();
            } catch (error) {
                alert('Hubo un error al enviar el mensaje. Por favor, intente nuevamente o contáctenos por teléfono.');
            } finally {
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            }
        });
        
        // Smooth scroll para enlaces internos
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Animación adicional para las tarjetas de familias
        document.querySelectorAll('.family-card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.zIndex = '10';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.zIndex = '1';
            });
        });
        
        // Reemplazar el script del carrusel con esta versión corregida
        document.addEventListener('DOMContentLoaded', function() {
            const track = document.querySelector('.testimonios-track');
            const cards = Array.from(track.children);
            const nextButton = document.querySelector('.testimonios-btn.next');
            const prevButton = document.querySelector('.testimonios-btn.prev');
            const dotsNav = document.querySelector('.testimonios-dots');
            const dots = Array.from(dotsNav.children);
            
            if (!track || cards.length === 0) return;
            
            // Calcular el ancho de una tarjeta
            const cardStyle = window.getComputedStyle(cards[0]);
            const cardWidth = cards[0].offsetWidth + parseInt(cardStyle.marginRight || 0);
            const gap = 30;
            
            // Crear dots dinámicamente según número de grupos
            const updateDots = () => {
                const visibleCards = getVisibleCards();
                const totalGroups = Math.ceil(cards.length / visibleCards);
                
                dotsNav.innerHTML = '';
                for (let i = 0; i < totalGroups; i++) {
                    const dot = document.createElement('div');
                    dot.className = 'testimonios-dot' + (i === 0 ? ' active' : '');
                    dot.dataset.slide = i;
                    dotsNav.appendChild(dot);
                }
                
                return totalGroups;
            };
            
            let currentGroup = 0;
            let totalGroups = updateDots();
            let visibleCards = getVisibleCards();
            
            // Función para obtener cuántas tarjetas son visibles
            function getVisibleCards() {
                const containerWidth = track.parentElement.offsetWidth;
                if (containerWidth >= 992) return 3;
                if (containerWidth >= 768) return 2;
                return 1;
            }
            
            // Función para mover al grupo específico
            const moveToGroup = (groupIndex) => {
                if (groupIndex < 0 || groupIndex >= totalGroups) return;
                
                const moveDistance = (cardWidth + gap) * groupIndex * visibleCards * -1;
                track.style.transform = `translateX(${moveDistance}px)`;
                currentGroup = groupIndex;
                
                // Actualizar dots
                const dots = Array.from(dotsNav.children);
                dots.forEach((dot, index) => {
                    dot.classList.toggle('active', index === groupIndex);
                });
            };
            
            // Event listeners para botones
            nextButton.addEventListener('click', function() {
                let nextGroup = currentGroup + 1;
                if (nextGroup >= totalGroups) nextGroup = 0;
                moveToGroup(nextGroup);
            });
            
            prevButton.addEventListener('click', function() {
                let prevGroup = currentGroup - 1;
                if (prevGroup < 0) prevGroup = totalGroups - 1;
                moveToGroup(prevGroup);
            });
            
            // Event listener para dots
            dotsNav.addEventListener('click', function(e) {
                const targetDot = e.target.closest('.testimonios-dot');
                if (!targetDot) return;
                
                const groupIndex = parseInt(targetDot.dataset.slide);
                moveToGroup(groupIndex);
            });
            
            // Actualizar en redimensionamiento
            window.addEventListener('resize', function() {
                visibleCards = getVisibleCards();
                totalGroups = updateDots();
                moveToGroup(0);
            });
            
            // Autoavance cada 8 segundos
            let autoSlide = setInterval(function() {
                let nextGroup = currentGroup + 1;
                if (nextGroup >= totalGroups) nextGroup = 0;
                moveToGroup(nextGroup);
            }, 8000);
            
            // Pausar autoavance al interactuar
            track.addEventListener('mouseenter', () => clearInterval(autoSlide));
            track.addEventListener('mouseleave', () => {
                autoSlide = setInterval(function() {
                    let nextGroup = currentGroup + 1;
                    if (nextGroup >= totalGroups) nextGroup = 0;
                    moveToGroup(nextGroup);
                }, 8000);
            });
        });
        
        // Efecto de scroll en header
        let lastScrollTop = 0;
        const header = document.querySelector('header');

        window.addEventListener('scroll', function() {
            const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
            
            if (scrollTop > 100) {
                header.classList.add('header-scrolled');
            } else {
                header.classList.remove('header-scrolled');
            }
            
            lastScrollTop = scrollTop;
        });
    </script>
</body>
</html>
