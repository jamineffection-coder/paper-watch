<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>北京时间</title>

  <!-- 数码感字体 -->
  <link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      width: 100vw;
      height: 100vh;
      background: #ffffff;
      color: #000000;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Arial, "Microsoft YaHei", sans-serif;
    }

    .container {
      text-align: center;
      padding: 24px;
    }

    .title {
      font-size: 22px;
      font-weight: 500;
      margin-bottom: 28px;
      letter-spacing: 1px;
    }

    .time {
      font-family: "Share Tech Mono", monospace;
      font-size: 64px;
      font-weight: bold;
      letter-spacing: 4px;
      margin-bottom: 26px;
      line-height: 1.2;
    }

    .wish {
      font-size: 16px;
      font-weight: 400;
      letter-spacing: 1px;
    }

    @media (max-width: 480px) {
      .title {
        font-size: 20px;
        margin-bottom: 24px;
      }

      .time {
        font-size: 52px;
        letter-spacing: 3px;
      }

      .wish {
        font-size: 15px;
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="title">现在是北京时间</div>
    <div class="time" id="time">00:00:00</div>
    <div class="wish">祝您生活愉快</div>
  </div>

  <script>
    function updateBeijingTime() {
      const now = new Date();

      // 转换为北京时间，Asia/Shanghai 时区
      const beijingTime = new Intl.DateTimeFormat("zh-CN", {
        timeZone: "Asia/Shanghai",
        hour: "2-digit",
        minute: "2-digit",
        second: "2-digit",
        hour12: false
      }).format(now);

      document.getElementById("time").textContent = beijingTime;
    }

    updateBeijingTime();
    setInterval(updateBeijingTime, 1000);
  </script>

</body>
</html>
