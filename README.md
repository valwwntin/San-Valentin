<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín? 💘</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffdde1;
        }
        h1 {
            color: #d63384;
            font-size: 24px;
        }
        .container {
            margin-top: 50px;
        }
        .btn {
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            cursor: pointer;
            margin: 10px;
        }
        .yes {
            background-color: #ff69b4;
            color: white;
            border-radius: 10px;
        }
        .no {
            background-color: #ff6f61;
            color: white;
            border-radius: 10px;
            position: absolute;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>¿Quieres ser mi San Valentín? 💖</h1>
        <button class="btn yes" onclick="aceptar()">Sí 💕</button>
        <button class="btn no" id="noBtn" onmouseover="moverBoton()">No 💔</button>
    </div>

    <script>
        function aceptar() {
            alert("¡Sabía que dirías que sí! 💖 Te amo mucho 😍");
        }

        function moverBoton() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            document.getElementById('noBtn').style.left = x + 'px';
            document.getElementById('noBtn').style.top = y + 'px';
        }
    </script>

</body>
</html>
