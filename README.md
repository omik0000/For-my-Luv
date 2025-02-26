<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Luv ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe4e1;
            color: #333;
            padding: 50px;
        }
        h1 {
            font-size: 26px;
        }
        .question {
            font-size: 22px;
            margin-bottom: 20px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        #yesBtn {
            background-color: #ff69b4;
            color: white;
        }
        #yesBtn:hover {
            background-color: #ff1493;
        }
        #noBtn {
            background-color: #ddd;
        }
        #noBtn:hover {
            background-color: #bbb;
        }
        #ticket {
            display: none;
            margin-top: 30px;
        }
        img {
            width: 80%;
            max-width: 500px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>

    <h1>For My Love ❤️</h1>
    <p class="question">Are you ready for a fun little game? 😊</p>
    
    <div class="buttons">
        <button id="yesBtn">Yes! 💖</button>
        <button id="noBtn">No 😢</button>
    </div>

    <div id="ticket">
        <h2>Yay! Here’s our flight ticket for June! ✈️💑</h2>
        <img src="your-flight-ticket-image-url.jpg" alt="Flight Ticket">
    </div>

    <script>
        const questions = [
            "Are you ready for a fun little game? 😊",
            "Do you promise to always be my best friend? 💕",
            "Will you laugh at my silly jokes even when they're bad? 😂",
            "Will you be my forever adventure buddy? 🌎",
            "Do you believe in soulmates? Because I do, and you're mine. 💫",
            "Will you keep stealing my hoodies forever? 🧥❤️",
            "Will you let me be your favorite person, always? 🥰",
            "Are you excited for all the memories we'll make? 📸",
            "Are you ready to spend forever with me? 💍",
            "One last question… want to see our flight ticket for June? ✈️"
        ];

        let questionIndex = 0;
        const questionElement = document.querySelector(".question");
        const yesBtn = document.getElementById("yesBtn");
        const noBtn = document.getElementById("noBtn");
        const buttonsDiv = document.querySelector(".buttons");
        const ticketDiv = document.getElementById("ticket");

        yesBtn.addEventListener("click", function() {
            questionIndex++;
            if (questionIndex < questions.length) {
                questionElement.innerText = questions[questionIndex];
            } else {
                questionElement.innerText = "Yay! I can’t wait to spend forever with you! ❤️";
                buttonsDiv.style.display = "none";
                ticketDiv.style.display = "block";
            }
        });

        noBtn.addEventListener("click", function() {
            alert("Wait, think again! Imagine all the adventures we'll have together! 🥺💞");
        });
    </script>

</body>
</html>
