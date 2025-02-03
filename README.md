# paramiluuuuu
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz San Valentín</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff6f61, #ffcccb);
            font-family: 'Arial', sans-serif;
            overflow: hidden;
        }

        .card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .card h1 {
            color: #ff6f61;
            font-size: 2.5em;
        }

        .card p {
            font-size: 1.2em;
            color: #333;
        }

        .card button {
            background: #ff6f61;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1em;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 20px;
        }

        .card button:hover {
            background: #ff4a3d;
        }

        .hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 0;
        }

        .hearts span {
            position: absolute;
            display: block;
            width: 20px;
            height: 20px;
            background: #ff6f61;
            clip-path: polygon(50% 0%, 100% 38%, 82% 100%, 50% 75%, 18% 100%, 0% 38%);
            animation: animate 5s linear infinite;
        }

        @keyframes animate {
            0% {
                transform: translateY(-100%);
            }
            100% {
                transform: translateY(100vh);
            }
        }
    </style>
</head>
<body>
    <div class="hearts">
        <span style="left: 5%; animation-delay: 0s;"></span>
        <span style="left: 15%; animation-delay: 1s;"></span>
        <span style="left: 25%; animation-delay: 2s;"></span>
        <span style="left: 35%; animation-delay: 3s;"></span>
        <span style="left: 45%; animation-delay: 4s;"></span>
        <span style="left: 55%; animation-delay: 5s;"></span>
        <span style="left: 65%; animation-delay: 6s;"></span>
        <span style="left: 75%; animation-delay: 7s;"></span>
        <span style="left: 85%; animation-delay: 8s;"></span>
        <span style="left: 95%; animation-delay: 9s;"></span>
    </div>

    <div class="card">
        <h1>¡Feliz San Valentín!</h1>
        <p id="message" style="display: none;">Eres el amor de mi vida. 💖</p>
        <button onclick="revealMessage()">Haz clic aquí</button>
    </div>

    <script>
        function revealMessage() {
            document.getElementById('message').style.display = 'block';
        }
    </script>
</body>
</html>
