<!DOCTYPE html>
<html lang="en">

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
