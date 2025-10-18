<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>🎆 Happy Diwali 🎆</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff9933, #ffcc00, #ff6600);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-family: 'Poppins', sans-serif;
      color: #fff;
      text-align: center;
      overflow: hidden;
    }

    h1 {
      font-size: 2.5em;
      text-shadow: 0 0 20px #fff, 0 0 40px gold;
      margin-bottom: 20px;
      animation: glow 2s infinite alternate;
    }

    @keyframes glow {
      from { text-shadow: 0 0 10px #fff, 0 0 20px gold; }
      to { text-shadow: 0 0 30px #ffcc00, 0 0 60px orange; }
    }

    button {
      background: #ff0066;
      border: none;
      color: white;
      padding: 12px 25px;
      font-size: 18px;
      border-radius: 10px;
      cursor: pointer;
      box-shadow: 0 0 15px #fff;
      transition: transform 0.2s;
    }

    button:hover {
      transform: scale(1.1);
    }

    .popup {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.85);
      display: none;
      justify-content: center;
      align-items: center;
    }

    .popup img {
      max-width: 90%;
      max-height: 80%;
      border-radius: 15px;
      box-shadow: 0 0 30px gold;
    }
  </style>
</head>
<body>

  <h1>🎆 Happy Diwali 🎆</h1>
  <button onclick="showPopup()">Tap to collect your gift 🎁</button>

  <div class="popup" id="popup" onclick="hidePopup()">
    <img src="gift.jpg" alt="Your Gift"> <WhatsApp Image 2025-10-18 at 09.27.32_db61fa98.jpg>
  </div>

  <script>
    const popup = document.getElementById('popup');
    function showPopup() { popup.style.display = 'flex'; }
    function hidePopup() { popup.style.display = 'none'; }
  </script>

</body>
</html>
