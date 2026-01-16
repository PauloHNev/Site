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

        header h1 {
            font-size: 46px;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 3px;
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

        .names {
            margin: 35px 0;
            font-size: 24px;
            font-weight: bold;
            color: #00eaff;
            text-shadow: 0 0 15px #00eaff;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            padding: 40px 20px;
            max-width: 1100px;
            margin: auto;
        }

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

        /* COMENTÁRIOS */
        .comments {
            padding: 60px 20px;
            max-width: 1100px;
            margin: auto;
        }

        .comments h2 {
            margin-bottom: 35px;
            font-size: 32px;
            color: #ff00ff;
            text-shadow: 0 0 15px #ff00ff;
        }

        .comment-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 25px;
        }

        .comment {
            background: rgba(255, 255, 255, 0.08);
            border-radius: 18px;
            padding: 25px;
            text-align: left;
            box-shadow: 0 0 20px rgba(255, 0, 200, 0.3);
        }

        .comment p {
            font-size: 15px;
            line-height: 1.6;
            margin-bottom: 15px;
        }

        .comment span {
            font-size: 14px;
            color: #00eaff;
            font-weight: bold;
        }

        footer {
            padding: 30px;
            font-size: 14px;
            opacity: 0.6;
        }

        .music {
            position: fixed;
            bottom: 15px;
            right: 15px;
            background: #ff004c;
            color: #fff;
            padding: 12px 18px;
            border-radius: 50px;
            font-size: 14px;
            box-shadow: 0 0 20px #ff004c;
        }
    </style>
</head>
<body>

<!-- MÚSICA YOUTUBE -->
<iframe
    src="https://www.youtube.com/embed/NMnLpK8WCg0?autoplay=1&loop=1&playlist=NMnLpK8WCg0&controls=0&mute=1"
    style="width:0;height:0;border:0;position:absolute;"
    allow="autoplay">
</iframe>


    <header>
        <h1>Aqui o coro come 🔥</h1>
        <p>Resenha, zoeira e amizade sem limites</p>

        <div class="names">
            Edio • Thiago • Paulo
        </div>
    </header>

    <section class="gallery">
        <img src="https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e">
        <img src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c">
        <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2">
        <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330">
    </section>

    <!-- COMENTÁRIOS -->
    <section class="comments">
        <h2>💬 O que elas dizem</h2>

        <div class="comment-grid">
            <div class="comment">
                <p>“O Edio é aquele tipo de pessoa que chega e muda o clima do lugar. Educado, divertido e muito carismático.”</p>
                <span>— Amanda</span>
            </div>

            <div class="comment">
                <p>“Thiago é simplesmente incrível! Sempre de bom humor e sabe conversar como ninguém.”</p>
                <span>— Juliana</span>
            </div>

            <div class="comment">
                <p>“O Paulo tem uma energia surreal. Respeitoso, parceiro e muito gente boa.”</p>
                <span>— Camila</span>
            </div>

            <div class="comment">
                <p>“Os três juntos são pura resenha! Edio, Thiago e Paulo são diferenciados.”</p>
                <span>— Larissa</span>
            </div>
        </div>
    </section>

    <div class="music">🎵 Ovo de Codorna</div>

    <footer>
        © 2026 • Aqui o coro come
    </footer>

</body>
</html>
