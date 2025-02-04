<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para mi Reni ❤️</title>
    <style>
        body {
            text-align: center;
            background-color: pink;
            font-family: 'Arial', sans-serif;
            position: relative;
        }
        .container {
            margin-top: 50px;
        }
        h1 {
            color: red;
            font-size: 30px;
        }
        .hello-kitty {
            width: 120px;
            height: auto;
            margin: 10px;
        }
        .hearts {
            font-size: 50px;
            color: red;
            margin: 10px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
        }
        .yes {
            background-color: red;
            color: white;
        }
        .no {
            background-color: gray;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>¿Me harías el honor de ser tu San Valentín, Reni? ❤️</h1>
        <div class="hearts">💕💖💞</div>
        <img src="https://upload.wikimedia.org/wikipedia/en/9/96/Hello_Kitty.svg" class="hello-kitty">
        <img src="https://upload.wikimedia.org/wikipedia/en/9/96/Hello_Kitty.svg" class="hello-kitty">
        <br>
        <div class="buttons">
            <button class="yes" onclick="showMessage()">Sí</button>
            <button class="no" onmouseover="moveNoButton()">No</button>
        </div>
        <p id="message" style="display:none; font-size: 20px; color: red;"></p>
    </div>

    <script>
        function showMessage() {
            document.getElementById("message").innerText = "Muchas gracias por darme otra oportunidad Mi Reni, te prometo que jamás te fallaré, prometo cuidarte y amarte hasta que la muerte nos separe <3";
            document.getElementById("message").style.display = "block";
        }

        function moveNoButton() {
            let x = Math.random() * window.innerWidth * 0.7;
            let y = Math.random() * window.innerHeight * 0.7;
            document.querySelector(".no").style.left = x + "px";
            document.querySelector(".no").style.top = y + "px";
        }
    </script>

</body>
</html>

