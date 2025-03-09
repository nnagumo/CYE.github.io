# CYE.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ENTERALT</title>
  <style>
    body { 
font-family: 'Great Vibes', cursive;
      text-align: center; 
      padding: 20px; 
      background: linear-gradient(to right, #a0c4ff, #fef9ef, #b08968); 
      color: #3d405b; 
    }
    #countdown { 
      font-size: 3rem; 
      margin-bottom: 20px; 
      font-weight: bold; 
    }
    iframe { 
      width: 90%; 
      max-width: 900px; 
      height: 500px; 
      margin-bottom: 20px; 
      border-radius: 10px; 
      border: 4px solid #b08968;
    }
    .social-links { 
      display: flex; 
      justify-content: center; 
      gap: 20px; 
      margin-top: 20px; 
    }
    .social-links a { 
      position: relative;
      text-decoration: none; 
      font-size: 24px; 
      color: #3d405b; 
      font-weight: bold; 
      background: rgba(176, 143, 94, 0.2); 
      padding: 10px 20px; 
      border-radius: 10px; 
      transition: 0.3s; 
    }
    .social-links a:hover { 
      background: rgba(176, 143, 94, 0.4); 
    }
    .social-links a .preview {
      display: none;
      position: absolute;
      bottom: 40px;
      left: 50%;
      transform: translateX(-50%);
      background: white;
      padding: 10px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
      width: 200px;
      text-align: center;
      z-index: 10;
    }
    .social-links a:hover .preview {
      display: block;
    }
    .preview img {
      width: 100%;
      border-radius: 5px;
    }
    .form-link { 
      display: block; 
      margin-top: 40px; 
      font-size: 20px; 
      color: #3d405b; 
      text-decoration: none; 
      font-weight: bold; 
      background: rgba(160, 196, 255, 0.3); 
      padding: 15px 30px; 
      border-radius: 10px; 
      transition: 0.3s; 
    }
    .form-link:hover { 
      background: rgba(160, 196, 255, 0.5); 
    }
  </style>
</head>
<body>
  <h1>COUNTDOWN TO CYE DEBUT</h1>
  <div id="countdown"></div>
  <iframe src="https://www.youtube.com/embed/o4Acsg5QubM?autoplay=1" frameborder="0" allowfullscreen></iframe>

  <div class="social-links">
    <a href="https://www.instagram.com/close.your.eyes.official/?hl=en" target="_blank">
      𝄋 Instagram
      <div class="preview">
        <img src="https://pbs.twimg.com/media/GlbSPrJbwAI2qY0?format=jpg&name=medium" alt="Instagram Preview">
        <p>Instagram of Close Your Eyes</p>
      </div>
    </a>
    <a href="https://x.com/closeyoureyes_7" target="_blank">
      𝄋 Twitter
      <div class="preview">
        <img src="https://pbs.twimg.com/media/GlbNtrgbwAUZsoz?format=jpg&name=4096x4096" alt="Twitter Preview">
        <p>Twitter of Close Your Eyes</p>
      </div>
    </a>
    <a href="https://www.youtube.com/@close.your.eyes.official" target="_blank">
      𝄋 YouTube
      <div class="preview">
        <img src="https://pbs.twimg.com/media/GlbN85kawAApvk4?format=jpg&name=4096x4096" alt="YouTube Preview">
        <p>YouTube of Close Your Eyes</p>
      </div>
    </a>
  </div>

  <a class="form-link" href="https://docs.google.com/forms/d/e/1FAIpQLSdsfHIKCAdJH-nA27Tezd_-kv6879h0VcptQ3zaQGSKppY7Lw/viewform?usp=sharing" target="_blank">📝 Share Your Thoughts Here!</a>

  <script>
    function updateCountdown() {
      const targetDate = new Date("2025-04-02T17:00:00").getTime();
      const now = new Date().getTime();
      const timeLeft = targetDate - now;
      
      if (timeLeft < 0) {
        document.getElementById("countdown").innerText = "The wait is over!";
        return;
      }
      
      const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
      const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);
      
      document.getElementById("countdown").innerText = `${days}d ${hours}h ${minutes}m ${seconds}s`;
    }
    
    setInterval(updateCountdown, 1000);
    updateCountdown();
  </script>
</body>
</html>
