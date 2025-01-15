<meta name='viewport' content='width=device-width, initial-scale=1'/><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CP.V2 - Color Prediction HACK</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>CP.V2 - Color Prediction HACK</h1>
        <div class="prediction-container">
            <div id="prediction-box">
                <h2 id="prediction">Loading...</h2>
            </div>
            <p id="timer">Next prediction in: <span id="countdown">60</span> seconds</p>
        </div>
        <div class="links">
            <a class="register-link" href="https://www.dmwin2.com/#/register?invitationCode=221631110785" target="_blank" onclick="redirectToGoogle()">Register Here</a>
            <a class="game-link" href="https://www.dmwin2.com/#/register?invitationCode=221631110785" target="_blank">Play the Game</a>
            <a class="telegram-link" href="https://t.me/nZxfMvcpQmkwMTJl" target="_blank">Join our Telegram Channel</a>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html><style>/* General body styling */
body {
    font-family: "Courier New", Courier, monospace;
    color: #0f0;
    background-color: #000;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
}

/* Container styling for the app */
.container {
    width: 90%;
    max-width: 350px;
    background-color: #111;
    border: 2px solid #0f0;
    border-radius: 8px;
    padding: 15px;
    text-align: center;
    box-shadow: 0 0 15px #0f0;
}

/* Heading styles */
h1 {
    font-size: 20px;
    margin-bottom: 10px;
}

/* Prediction container box with colors */
#prediction-box {
    display: inline-block;
    margin: 20px 0;
    padding: 20px;
    border-radius: 10px;
    background-color: #222;
    border: 2px solid #0f0;
    box-shadow: 0 0 10px rgba(0, 255, 0, 0.7);
}

#prediction-box h2 {
    font-size: 32px;
    color: #0f0;
    margin: 0;
}

/* Timer style */
#timer {
    font-size: 14px;
    color: #fff;
}

/* Register button */
.register-link {
    display: inline-block;
    margin: 10px 5px;
    padding: 10px 20px;
    font-size: 16px;
    color: #fff;
    background-color: #f00;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s;
}

.register-link:hover {
    background-color: #b00;
}

/* Game link */
.game-link {
    display: block;
    margin-top: 10px;
    font-size: 14px;
    color: #0f0;
    text-decoration: none;
}

.game-link:hover {
    text-decoration: underline;
}

/* Telegram link styling */
.telegram-link {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    font-size: 16px;
    color: #fff;
    background-color: #0088cc; /* Telegram blue */
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s;
}

.telegram-link:hover {
    background-color: #006fa1; /* Darker Telegram blue */
}</style><script>// Function to generate a random prediction
function generatePrediction() {
    const predictions = ["Big", "Small"];
    return predictions[Math.floor(Math.random() * predictions.length)];
}

// Function to update the prediction
function updatePrediction() {
    const predictionElement = document.getElementById('prediction');
    predictionElement.textContent = generatePrediction();
}

// Countdown timer
function startCountdown() {
    let countdown = 60;
    const timerElement = document.getElementById('countdown');
    
    const interval = setInterval(() => {
        countdown--;
        timerElement.textContent = countdown;
        
        if (countdown <= 0) {
            clearInterval(interval);
            updatePrediction();
            startCountdown(); // Restart the countdown
        }
    }, 1000);
}

// Redirect to Google after registering
function redirectToGoogle() {
    setTimeout(() => {
        window.location.href = "https://www.google.com";
    }, 200
t