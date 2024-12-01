<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Merry Christmas</title>
  <style>
    body {
      margin: 0;
      background: linear-gradient(to bottom, #001f3f, #004d7a);
      color: #fff;
      font-family: 'Arial', sans-serif;
      overflow: hidden;
    }
    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .text {
      font-size: 3em;
      font-weight: bold;
      text-transform: uppercase;
      color: #f4d03f;
      text-shadow: 2px 2px 10px #ff5733, -2px -2px 10px #33c9ff;
      animation: glow 1.5s infinite alternate;
    }
    @keyframes glow {
      from {
        text-shadow: 2px 2px 10px #ff5733, -2px -2px 10px #33c9ff;
      }
      to {
        text-shadow: 4px 4px 20px #ff5733, -4px -4px 20px #33c9ff;
      }
    }
    .bells {
      display: flex;
      gap: 20px;
      margin-top: 20px;
    }
    .bell {
      width: 50px;
      height: 50px;
      background: gold;
      border-radius: 50%;
      position: relative;
      animation: swing 1s infinite alternate;
    }
    .bell:before {
      content: '';
      width: 10px;
      height: 10px;
      background: red;
      border-radius: 50%;
      position: absolute;
      bottom: 5px;
      left: 50%;
      transform: translateX(-50%);
    }
    .bell:after {
      content: '';
      width: 15px;
      height: 15px;
      background: brown;
      border-radius: 50%;
      position: absolute;
      top: -5px;
      left: 50%;
      transform: translateX(-50%);
    }
    @keyframes swing {
      0% { transform: rotate(-10deg); }
      100% { transform: rotate(10deg); }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="text">Merry Christmas</div>
    <div class="bells">
      <div class="bell"></div>
      <div class="bell"></div>
      <div class="bell"></div>
    </div>
  </div>
</body>
</html>
