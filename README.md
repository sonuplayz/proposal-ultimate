<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>iI love You !❤</title>
    <title>iDo You Love Me ? 💍</title>
    <style>
        body {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(to right, #ff758c, #ff7eb3);
            color: white;
            padding: 50px;
        }
        h1 {
            font-size: 40px;
        }
        p {
            font-size: 20px;
        }
        .buttons {
            margin-top: 20px;
            position: relative;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        #yesBtn {
            background-color: #28a745;
            color: white;
        }
        #noBtn {
            background-color: #dc3545;
            color: white;
            position: absolute;
            transition: all 0.3s ease;
        }
        #gifContainer {
            display: none;
            margin-top: 30px;
        }
        #gifContainer img {
            width: 50%;
            max-width: 400px;
            border-radius: 10px;
        }
        audio {
            display: none;
        }
    </style>
</head>
<body>

    <h1>Do You Love Me ? 💍❤</h1>
    <p>You are the best thing that ever happened to me!</p>
    
    <div class="buttons">
        <button id="yesBtn" onclick="showGif()">Yes</button>
        <button id="noBtn" onmouseover="moveButton()">No</button>
    </div>

    <div id="gifContainer">
        <h1>Yay! You said YES! ❤</h1>
        <img src="https://media.giphy.com/media/3oz8xKaR836UJOYeOc/giphy.gif" alt="Happy GIF">
    </div>

    <audio id="bgMusic" loop>
        <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3" type="audio/mp3">
    </audio>

    <script>
        function moveButton() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            document.getElementById('noBtn').style.left = ${x}px;
            document.getElementById('noBtn').style.top = ${y}px;
        }

        function showGif() {
            document.getElementById("gifContainer").style.display = "block";
            document.getElementById("bgMusic").play();
        }
    </script>

</body>
</html>
