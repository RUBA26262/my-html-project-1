<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Boyfriend's Day 💖</title>
  <style>
    body {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #ffb6c1, #ff69b4);
      color: #fff;
      min-height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 20px;
    }
    h1 {
      font-size: 2.5rem;
      margin-bottom: 20px;
      animation: pop 1s ease-in-out;
    }
    p {
      font-size: 1.2rem;
      margin: 10px 0;
    }
    .buttons {
      margin-top: 20px;
    }
    button {
      background: #fff;
      color: #ff69b4;
      border: none;
      padding: 12px 20px;
      margin: 10px;
      border-radius: 25px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #ff1493;
      color: #fff;
    }
    .hidden-message {
      display: none;
      margin-top: 20px;
      font-size: 1.3rem;
      animation: fadeIn 1s ease-in-out;
    }
    #qrcode {
      margin-top: 30px;
    }
    @keyframes pop {
      0% { transform: scale(0.8); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>

  <h1>💝 Happy Boyfriend's Day 💝</h1>
  <p>My love, today is all about YOU 💕. Click the buttons for your surprises 😘</p>

  <div class="buttons">
    <button onclick="showMessage('msg1')">🐻Babee</button>
    <button onclick="showMessage('msg2')">🍫Thangoo</button>
    <button onclick="showMessage('msg3')">🌙Dear Hubbyy</button>
    <button onclick="showMessage('msg4')">🎶11:11</button>
  </div>

  <!-- Customize your messages -->
  <div id="msg1" class="hidden-message">No matter what happens
I want you to stay in my life forever
I miss you more than words can say...
I love you so much thangoo ❤🧸</div>
  <div id="msg2" class="hidden-message">No matter how many people I meet in my life, no one will ever make my heart feel the way you do. You’re my reason to smile every day, my comfort, and my forever. I love you more than words could ever explain 🍫💖</div>
  <div id="msg3" class="hidden-message">I’ll love you till the moon & back🌙</div>
  <div id="msg4" class="hidden-message">Manifesting us,
    forever and always..
  </div>

  <!-- Insert your QR code image here -->
  <h2 style="margin-top:40px;">Scan or Click this QR for your surprise video 🎥💕</h2>
  <div id="qrcode">
    <a href="https://qrco.de/bgM0xi" target="_blank">
      <img src="frame.png" alt="QR Code" width="250">
    </a>
  </div>

  <script>
    function showMessage(id) {
      document.querySelectorAll('.hidden-message').forEach(msg => {
        msg.style.display = 'none';
      });
      document.getElementById(id).style.display = 'block';
    }
  </script>

</body>
</html>
