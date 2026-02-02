<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موقع مقلب</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            transition: background 0.5s;
        }
        button {
            padding: 20px 40px;
            font-size: 24px;
            cursor: pointer;
            border: none;
            border-radius: 10px;
            background-color: #4CAF50;
            color: white;
            transition: transform 0.2s, background-color 0.2s;
        }
        button:hover {
            background-color: #45a049;
            transform: scale(1.1);
        }
        .center {
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="center">
        <button onclick="clicked()">اضغط هنا</button>
    </div>

    <audio id="laughSound" src="https://www.soundjay.com/human/laugh-01.mp3"></audio>

    <script>
        function clicked() {
            document.body.innerHTML = '<div class="center"><h1>ضحكت عليك 😆</h1></div>';
            document.body.style.background = 'linear-gradient(135deg, #a1c4fd, #c2e9fb)';
            document.getElementById('laughSound').play();
        }
    </script>
</body>
</html>
