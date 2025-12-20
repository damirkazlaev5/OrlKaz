<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Светящаяся надпись</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #000;
        }
        .glow-text {
            font-family: Arial, sans-serif;
            font-size: 48px;
            color: #fff;
            text-align: center;
            animation: glow 1.5s ease-in-out infinite alternate;
        }
        @keyframes glow {
            from {
                text-shadow: 
                    0 0 5px #fff,
                    0 0 10px #fff,
                    0 0 15px #00ffff,
                    0 0 20px #00ffff;
            }
            to {
                text-shadow: 
                    0 0 10px #fff,
                    0 0 20px #fff,
                    0 0 30px #00ffff,
                    0 0 40px #00ffff;
            }
        }
    </style>
</head>
<body>
    <div class="glow-text">Привет</div>
</body>
</html>
