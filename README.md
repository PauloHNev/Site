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

        /* 💖 FUNDO ROMÂNTICO */
        body {
            background-image: url("https://images.unsplash.com/photo-1517841905240-472988babdf9");
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
            color: #fff;
            text-align: center;
            position: relative;
        }

        /* CAMADA ESCURA PARA LEITURA */
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(
                rgba(0, 0, 0, 0.65),
                rgba(0, 0, 0, 0.85)
            );
            z-index: -1;
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
            box-shadow: 0 0 25px rgba(255, 0, 140, 0.6);
        }

        .gallery img:hover {
            transform: scale(1.05);
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
            cursor: pointer;
            z-index: 10;
        }

        footer {
            padding: 30px;
            font-size: 14px;
            opacity: 0.7;
        }
    </style>
</head>

<body>

<!-- 🎵 MÚSICA YOUTUBE -->
<iframe
    id="yt-music"
    src="https://www.youtube.com/embed/NMnLpK8WCg0?autoplay=1&loop=1&playlist=NMnLpK8WCg0&mute=1&controls=0&enablejsapi=1"
    allow="autoplay"
    style="width:0;height:0;border:0;position:absolute;">
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

<div class="music" onclick="ativarSom()">🔊 Ativar som</div>

<footer>
    © 2026 • Aqui o coro come
</footer>

<script>
    let somAtivo = false;
    let player;

    function onYouTubeIframeAPIReady() {
        player = new YT.Player('yt-music');
    }

    function ativarSom() {
        if (!player) return;

        if (!somAtivo) {
            player.unMute();
            player.setVolume(70);
            document.querySelector('.music').innerText = '🔇 Silenciar música';
            somAtivo = true;
        } else {
            player.mute();
            document.querySelector('.music').innerText = '🔊 Ativar som';
            somAtivo = false;
        }
    }
</script>

<script src="https://www.youtube.com/iframe_api"></script>

</body>
</html>
