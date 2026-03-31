<!DOCTYPE html>
<html>
<head>
    <title>Question for You ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            margin-top: 100px;
            background-color: #ffe6e6;
        }

        h1 {
            color: #ff4d4d;
        }

        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
            border-radius: 10px;
            border: none;
        }

        #yesBtn {
            background-color: #4CAF50;
            color: white;
        }

        #noBtn {
            background-color: #ff4d4d;
            color: white;
            position: absolute;
        }
    </style>
</head>

<body>

    <h1>Do you love me? ❤️</h1>

    <button id="yesBtn" onclick="yesClicked()">Yes 💖</button>
    <button id="noBtn">No 😢</button>

    <script>
        const noBtn = document.getElementById("noBtn");

        noBtn.addEventListener("mouseover", function() {
            const x = Math.random() * window.innerWidth;
            const y = Math.random() * window.innerHeight;

            noBtn.style.left = x + "px";
            noBtn.style.top = y + "px";
        });

        function yesClicked() {
            document.body.innerHTML = "<h1>I knew it! ❤️😍</h1><p>You make me so happy 💕</p>";
        }
    </script>

</body>
</html>
