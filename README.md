<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz Aniversário!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background-color: #ffccff;
            overflow: hidden;
            position: relative;
        }

        h1 {
            font-size: 6rem;
            color: #ff3366;
            text-align: center;
            text-shadow: 0 0 20px #ff6666, 0 0 30px #ff6699, 0 0 40px #ff33cc, 0 0 50px #ff33cc;
            animation: shine 2s infinite alternate, bounce 1s ease infinite;
            z-index: 1;
        }

        @keyframes shine {
            0% {
                text-shadow: 0 0 20px #ff6666, 0 0 30px #ff6699, 0 0 40px #ff33cc, 0 0 50px #ff33cc;
            }
            100% {
                text-shadow: 0 0 30px #ff6666, 0 0 40px #ff6699, 0 0 50px #ff33cc, 0 0 60px #ff33cc;
            }
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-30px);
            }
        }

        .balloon {
            position: absolute;
            width: 60px;
            height: 80px;
            background-color: #66ccff;
            border-radius: 50%;
            animation: float 5s infinite ease-in-out, spin 6s infinite linear;
        }

        .balloon::after {
            content: '';
            position: absolute;
            bottom: -20px;
            left: 50%;
            width: 2px;
            height: 20px;
            background-color: #999;
        }

        @keyframes float {
            0% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-30px);
            }
            100% {
                transform: translateY(0);
            }
        }

        @keyframes spin {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }

        .heart {
            position: absolute;
            width: 60px;
            height: 60px;
            background-color: #ff6699;
            clip-path: polygon(50% 0%, 100% 35%, 80% 100%, 50% 75%, 20% 100%, 0% 35%);
            animation: heartbeat 1s infinite, rotateHeart 3s infinite linear;
        }

        @keyframes heartbeat {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
        }

        @keyframes rotateHeart {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }

        .balloon1 {
            top: 10%;
            left: 30%;
            animation-duration: 4s;
        }

        .balloon2 {
            top: 25%;
            left: 60%;
            animation-duration: 6s;
        }

        .balloon3 {
            top: 50%;
            left: 40%;
            animation-duration: 7s;
        }

        .balloon4 {
            top: 15%;
            left: 70%;
            animation-duration: 5s;
        }

        .balloon5 {
            top: 35%;
            left: 80%;
            animation-duration: 4s;
        }

        .balloon6 {
            top: 55%;
            left: 20%;
            animation-duration: 6s;
        }

        .heart1 {
            top: 20%;
            left: 20%;
        }

        .heart2 {
            top: 60%;
            left: 70%;
        }

        .heart3 {
            top: 40%;
            left: 50%;
        }

        .heart4 {
            top: 15%;
            left: 80%;
        }

        .heart5 {
            top: 75%;
            left: 25%;
        }

        .heart6 {
            top: 55%;
            left: 40%;
        }

        .message {
            font-size: 2.5rem;
            color: #ff33cc;
            font-weight: bold;
            margin-top: 30px;
            text-align: center;
            animation: fadeIn 3s ease-out, moveUp 2s infinite alternate;
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }

        @keyframes moveUp {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(-10px);
            }
        }

        /* Confetes */
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: #ff3366;
            animation: confettiFall 2s infinite;
        }

        @keyframes confettiFall {
            0% {
                opacity: 1;
                transform: translateY(0) rotate(0deg);
            }
            100% {
                opacity: 1;
                transform: translateY(100vh) rotate(360deg);
            }
        }

    </style>
</head>
<body>

    <h1>Feliz Aniversário Alemoa braba!</h1>

    <!-- Balões -->
    <div class="balloon balloon1"></div>
    <div class="balloon balloon2"></div>
    <div class="balloon balloon3"></div>
    <div class="balloon balloon4"></div>
    <div class="balloon balloon5"></div>
    <div class="balloon balloon6"></div>

    <!-- Corações melhorados -->
    <div class="heart heart1"></div>
    <div class="heart heart2"></div>
    <div class="heart heart3"></div>
    <div class="heart heart4"></div>
    <div class="heart heart5"></div>
    <div class="heart heart6"></div>

    <!-- Mensagem -->
    <div class="message">Espero que goste do presente que eu escolhi. Desejo tudo de bom meu amor!</div>

    <!-- Confetes -->
    <div class="confetti" style="top: 10%; left: 5%; animation-duration: 2s; animation-delay: 0s;"></div>
    <div class="confetti" style="top: 20%; left: 30%; animation-duration: 2s; animation-delay: 1s;"></div>
    <div class="confetti" style="top: 30%; left: 50%; animation-duration: 2s; animation-delay: 2s;"></div>
    <div class="confetti" style="top: 40%; left: 70%; animation-duration: 2s; animation-delay: 3s;"></div>
    <div class="confetti" style="top: 50%; left: 80%; animation-duration: 2s; animation-delay: 4s;"></div>
    <div class="confetti" style="top: 60%; left: 90%; animation-duration: 2s; animation-delay: 5s;"></div>

</body>
</html>
