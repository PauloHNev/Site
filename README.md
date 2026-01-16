<!DOCTYPE html>
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
            background: linear-gradient(135deg, #111, #333);
            color: #fff;
            text-align: center;
        }

        header {
            padding: 60px 20px;
        }

        header h1 {
            font-size: 42px;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        header p {
            font-size: 18px;
            opacity: 0.85;
        }

        .names {
            margin: 30px 0;
            font-size: 22px;
            font-weight: bold;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            padding: 40px 20px;
            max-width: 1100px;
            margin: auto;
        }

        .gallery img {
            width: 100%;
            height: 350px;
            object-fit: cover;
            border-radius: 15px;
            transition: 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.05);
        }

        footer {
            padding: 25px;
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
