![IMG_20260228_225618](https://github.com/user-attachments/assets/4c1ca7c4-4188-4768-bfe0-533b39530930)
# richika-birthday
Happy Birthday richika page
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device‑width, initial‑scale=1.0"/>
  <title>Happy Birthday Richika</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
      font-family: 'Arial', sans-serif;
      overflow: hidden;
    }

    #runButton {
      padding: 12px 24px;
      font-size: 18px;
      background-color: #ff4757;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    #runButton:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 14px rgba(0,0,0,0.3);
    }

    #message {
      margin-top: 40px;
      font-size: 48px;
      font-weight: bold;
      color: #ff4757;
      text-shadow: 0 2px 10px rgba(255,255,255,0.5);
      opacity: 0;
      transform: scale(0.8);
      transition: all 1s ease;
    }

    #message.show {
      opacity: 1;
      transform: scale(1);
    }

    /* Hide audio player UI */
    audio {
      display: none;
    }
  </style>
</head>
<body>
  <button id="runButton">Run</button>
  <div id="message">Happy Birthday Richika!</div>

  <!-- Background music -->
  <audio id="birthdayMusic" loop>
    <source src="music.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <script>
    const runBtn = document.getElementById("runButton");
    const message = document.getElementById("message");
    const music = document.getElementById("birthdayMusic");

    runBtn.addEventListener("click", function () {
      // Show the animated text
      message.classList.add("show");

      // Start background music
      music.volume = 0.6; // adjust volume (0.0 to 1.0)
      music
        .play()
        .catch(error => {
          console.log("Autoplay blocked. User may need to tap/click first.", error);
        });

      // Disable button after click
      this.disabled = true;
    });
  </script>
</body>
</html>![IMG_20251219_123412](https://github.com/user-attachments/assets/a76dd30c-f260-4f78-bbc9-368aa628f213)
