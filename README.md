<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: pink;
            margin-top: 100px;
        }

        h1 {
            font-size: 2.5em;
            color: red;
        }

        .container {
            position: relative;
            display: inline-block;
        }

        .btn {
            font-size: 1.5em;
            padding: 15px 30px;
            margin: 20px;
            border: none;
            cursor: pointer;
            transition: all 0.3s ease-in-out;
        }

        #yes {
            background-color: green;
            color: white;
        }

        #no {
            background-color: red;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

    <h1>Will You Be My Valentine? ❤️</h1>
    <h2>Can I Take You Out? 💘</h2>

    <div class="container">
        <button id="yes" class="btn" onclick="alert('Yay! ❤️ Can’t wait!')">YES ✅</button>
        <button id="no" class="btn" onmouseover="moveButton()">NO ❌</button>
    </div>

    <script>
        function moveButton() {
            let x = Math.random() * window.innerWidth * 0.7;
            let y = Math.random() * window.innerHeight * 0.7;
            document.getElementById("no").style.left = x + "px";
            document.getElementById("no").style.top = y + "px";
        }
    </script>

</body>
</html>
