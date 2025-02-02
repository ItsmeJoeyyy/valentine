<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: pink;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        h1 {
            color: red;
            font-size: 3em;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 1.5em;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: red;
            color: white;
        }
        .no {
            background-color: white;
            color: red;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Will you be my Valentine? 💖</h1>
    <div class="buttons">
        <button class="yes" onclick="alert('Yay! Can’t wait for Valentine’s Day! ❤️')">Yes</button>
        <button class="no" id="noButton">No</button>
    </div>
    
    <script>
        document.getElementById("noButton").addEventListener("mouseover", function() {
            const x = Math.random() * window.innerWidth * 0.8;
            const y = Math.random() * window.innerHeight * 0.8;
            this.style.left = x + "px";
            this.style.top = y + "px";
        });
    </script>
</body>
</html>
