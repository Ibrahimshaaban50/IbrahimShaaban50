<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Personal Landing</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: #111;
      color: white;
      font-family: Arial, sans-serif;
      overflow: hidden;
    }

    .container {
      text-align: center;
    }

    .name {
      font-size: 3em;
      font-weight: bold;
      margin-bottom: 20px;
    }

    .title {
      font-size: 1.8em;
      font-weight: normal;
      animation: fade 6s infinite;
    }

    @keyframes fade {
      0%, 20% { opacity: 1; }
      25%, 95% { opacity: 0; }
      100% { opacity: 1; }
    }

    .titles {
      position: relative;
      height: 2em;
    }

    .titles span {
      position: absolute;
      left: 0;
      right: 0;
      opacity: 0;
      animation: fade 9s infinite;
    }

    .titles span:nth-child(1) { animation-delay: 0s; }
    .titles span:nth-child(2) { animation-delay: 3s; }
    .titles span:nth-child(3) { animation-delay: 6s; }

    .separator {
      margin-top: 20px;
      height: 4px;
      width: 200px;
      background: linear-gradient(90deg, red, green, blue, red);
      background-size: 400% 400%;
      border-radius: 2px;
      margin-left: auto;
      margin-right: auto;
      animation: rgbMove 6s linear infinite;
    }

    @keyframes rgbMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="name">Ibrahim Shaaban</div>
    <div class="titles">
      <span>Junior Embedded Engineer</span>
      <span>Data Analyst</span>
      <span>Automotive Enthusiast</span>
    </div>
    <div class="separator"></div>
  </div>
</body>
</html>
