<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Juego de Clicks</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f8ff;
            color: #333;
            margin: 0;
            padding: 20px;
        }
        h1 {
            margin-top: 50px;
        }
        button {
            padding: 15px 30px;
            font-size: 20px;
            margin: 20px;
            border: none;
            background-color: #28a745;
            color: white;
            border-radius: 10px;
            cursor: pointer;
        }
        button:hover {
            background-color: #218838;
        }
        #restartButton {
            background-color: #007bff;
        }
        #restartButton:hover {
            background-color: #0056b3;
        }
        #result {
            font-size: 24px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>¡Juego de Clicks!</h1>
    <p>Haz clic en el botón tantas veces como puedas en 10 segundos.</p>
    <button id="clickButton" onclick="clickGame()">¡Haz clic aquí!</button>
    <button id="restartButton" onclick="restartGame()">Reiniciar Juego</button>
    <div id="result"></div>

    <script>
        let clicks = 0;
        let gameStarted = false;

        function clickGame() {
            if (!gameStarted) {
                gameStarted = true;
                clicks = 0;
                document.getElementById("result").textContent = "¡El juego ha comenzado!";
                
                setTimeout(() => {
                    gameStarted = false;
                    document.getElementById("result").textContent = `Juego terminado. Hiciste ${clicks} clics.`;
                }, 10000);
            } else {
                clicks++;
            }
        }

        function restartGame() {
            gameStarted = false;
            clicks = 0;
            document.getElementById("result").textContent = "El juego ha sido reiniciado. Haz clic en el botón para comenzar.";
        }
    </script>
</body>
</html>
