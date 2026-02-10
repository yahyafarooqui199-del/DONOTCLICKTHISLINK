<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>My Valentine 💖</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #fff0f5, #ffe4e1);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }

    .card {
      background: white;
      padding: 30px;
      border-radius: 16px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      max-width: 400px;
    }

    h1 {
      color: #d6336c;
    }

    p {
      font-size: 16px;
      color: #444;
    }

    button {
      padding: 12px 20px;
      font-size: 16px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      margin: 10px;
    }

    #yesBtn {
      background-color: #ff5c8a;
      color: white;
    }

    #noBtn {
      background-color: #ddd;
      position: relative;
    }

    #response {
      margin-top: 20px;
      font-weight: bold;
      color: #d6336c;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>My Love ❤️</h1>
    <p>
      We’ve been married for a year and a half,<br />
      Ramadan is almost here,<br />
      and my heart still chooses you every day.
    </p>

    <p><strong>Will you be my Valentine? 💕</strong></p>

    <button id="yesBtn" onclick="sayYes()">Yes 💖</button>
    <button id="noBtn" onmouseover="moveButton()">No 🙃</button>

    <div id="response"></div>
  </div>

  <script>
    function sayYes() {
      document.getElementById("response").innerHTML =
        "Alhamdulillah 💕 I’m so grateful for you. Happy Valentine’s Day, my forever ❤️";
    }

    function moveButton() {
      const btn = document.getElementById("noBtn");
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 200 - 100;
      btn.style.transform = `translate(${x}px, ${y}px)`;
    }
  </script>
</body>
</html>
