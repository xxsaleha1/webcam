<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>webcam.exe</title>

  <style>
    body {
      margin: 0;
      min-height: 100vh;
      background: #ffc6e5;
      font-family: "Courier New", monospace;
      color: #111;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px;
      box-sizing: border-box;
    }

    .window {
      width: 100%;
      max-width: 420px;
      background: #f5f5f5;
      border: 3px solid #111;
      box-shadow: 8px 8px 0 #111;
    }

    .bar {
      background: #ff69b4;
      border-bottom: 3px solid #111;
      padding: 8px 10px;
      font-weight: bold;
      display: flex;
      justify-content: space-between;
    }

    .content {
      padding: 20px;
      text-align: center;
    }

    h1 {
      margin: 5px 0;
      font-size: 32px;
    }

    p {
      font-size: 14px;
    }

    .camera-box {
      margin: 20px 0;
      height: 250px;
      background: #222;
      border: 3px solid #111;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
    }

    button {
      background: #fff;
      border: 3px solid #111;
      padding: 12px 18px;
      font-family: inherit;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 4px 4px 0 #111;
    }

    button:active {
      transform: translate(3px, 3px);
      box-shadow: 1px 1px 0 #111;
    }

    .status {
      margin-top: 18px;
      font-size: 12px;
    }
  </style>
</head>

<body>

  <div class="window">

    <div class="bar">
      <span>webcam.exe</span>
      <span>×</span>
    </div>

    <div class="content">

      <h1>webcam.exe</h1>

      <p>your little corner of the internet ♡</p>

      <div class="camera-box">
        CAMERA OFFLINE
      </div>

      <button onclick="startCamera()">
        START WEBCAM
      </button>

      <div class="status" id="status">
        status: waiting...
      </div>

    </div>

  </div>

  <script>
    function startCamera() {
      document.getElementById("status").textContent =
        "status: camera coming soon...";
    }
  </script>

</body>
</html>
