<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Aqui o coro come</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }

        body {
            background: radial-gradient(circle at top, #222, #000);
            color: #fff;
            text-align: center;
        }

        header {
            padding: 70px 20px;
        }

        /* TÍTULO COM BRILHO */
        header h1 {
            font-size: 46px;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 3px;
            color: #fff;
            text-shadow:
                0 0 10px #ff004c,
                0 0 20px #ff004c,
                0 0 40px #ff004c;
            animation: glow 2s infinite alternate;
        }

        @keyframes glow {
            from {
                text-shadow:
                    0 0 10px #ff004c,
                    0 0 20px #ff004c,
                    0 0 40px #ff004c;
            }
            to {
                text-shadow:
                    0 0 20px #ff00ff,
                    0 0 40px #ff00ff,
                    0 0 60px #ff00ff;
            }
        }

        header p {
            font-size: 18px;
            opacity: 0.85;
        }

        /* NOMES COM NEON */
        .names {
            margin: 35px 0;
            font-size: 24px;
            font-weight: bold;
            color: #00eaff;
            text-shadow:
                0 0 10px #00eaff,
                0 0 20px #00eaff;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            padding: 40px 20px;
            max-width: 1100px;
            margin: auto;
        }

        /* IMAGENS COM BRILHO */
        .gallery img {
            width: 100%;
            height: 360px;
            object-fit: cover;
            border-radius: 18px;
            transition: 0.4s ease;
            box-shadow:
                0 0 15px rgba(255, 0, 140, 0.6),
                0 0 30px rgba(255, 0, 140, 0.4);
        }

        .gallery img:hover {
            transform: scale(1.07);
            box-shadow:
                0 0 25px rgba(0, 234, 255, 0.9),
                0 0 50px rgba(0, 234, 255, 0.7);
        }

        footer {
            padding: 30px;
            font-size: 14px;
            opacity: 0.6;
        }
    </style>
</head>
<body>

    <header>
        <h1>Aqui o coro come 🔥</h1>
        <p>Resenha, zoeira e amizade sem limites</p>

        <div class="names">
            Edio • Thiago • Paulo
        </div>
    </header>

    <section class="gallery">
        <img src="https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e" alt="Mulher bonita">
        <img src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c" alt="Mulher bonita">
        <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2" alt="Mulher bonita">
        <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330" alt="Mulher bonita">
    </section>

    <footer>
        © 2026 • Aqui o coro come
    </footer>

</body>
</html>
