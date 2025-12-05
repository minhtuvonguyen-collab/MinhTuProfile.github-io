<!doctype html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Giới thiệu - Minh Tú</title>
  <style>
    :root {
      --bg: #faf5ff;
      --card: #ffffff;
      --primary: #e9d5ff;
      --secondary: #d8b4fe;
      --text: #4b2d75;
      --muted: #8a7fa3;
    }

    * { box-sizing: border-box; }
    body {
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, Arial;
      margin: 0;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
      overflow-x: hidden;
    }

    header {
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      color: #fff;
      padding: 48px 20px;
      text-align: center;
      position: relative;
    }
    header h1 { font-size: 36px; margin: 0 0 10px; }
    header p { font-size: 16px; margin: 0; opacity: 0.9; }

    .sparkles {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      background-image: radial-gradient(circle, rgba(255,255,255,0.6) 2px, transparent 2px);
      background-size: 40px 40px;
      animation: sparkle 6s linear infinite;
      opacity: 0.6;
      z-index: 5;
    }
    @keyframes sparkle {
      from { background-position: 0 0; }
      to { background-position: 200px 200px; }
    }

    .container {
      max-width: 960px;
      margin: 40px auto;
      padding: 20px;
      position: relative;
      z-index: 10;
    }

    .card {
      background: var(--card);
      border-radius: 16px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.08);
      overflow: hidden;
      display: flex;
      flex-wrap: wrap;
    }

    .left {
      flex: 1 1 280px;
      background: #f5f0ff;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 30px;
    }

    .avatar {
      width: 260px;
      height: 260px;
      border-radius: 14px;
      overflow: hidden;
      border: 5px solid rgba(255,255,255,0.6);
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
    }
    .avatar img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .right {
      flex: 2 1 320px;
      padding: 30px 40px;
    }
    .right h2 {
      margin: 0 0 8px;
      font-size: 28px;
    }
    .right .meta {
      color: var(--muted);
      margin-bottom: 16px;
    }

    .about {
      background: #fdfaff;
      padding: 16px;
      border-radius: 12px;
      border: 1px solid #ecd9ff;
      min-height: 120px;
    }

    footer {
      text-align: center;
      padding: 20px 0;
      color: var(--muted);
      font-size: 14px;
      z-index: 10;
      position: relative;
    }

    .home-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: linear-gradient(135deg, #f3e8ff, #e9d5ff);
      color: #4b2d75;
      padding: 12px 20px;
      font-size: 15px;
      font-weight: 600;
      border: none;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.25);
      cursor: pointer;
      transition: 0.25s;
      z-index: 20;
    }
    .home-btn:hover {
      transform: scale(1.06);
      box-shadow: 0 6px 16px rgba(0,0,0,0.3);
    }

    @media(max-width: 720px){
      .right { padding: 20px; }
      header h1 { font-size: 28px; }
    }
  </style>
</head>

<body>

  <div class="sparkles"></div>

  <header>
    <h1>Giới thiệu bản thân</h1>
    <p>Trang cá nhân của Võ Nguyễn Minh Tú</p>
  </header>

  <div class="container">
    <div class="card">
      <div class="left">
        <div class="avatar">
          <img src="https://github.com/minhtuvonguyen-collab/MinhTuProfile.github-io/blob/main/z7266046669069_8ee11924eac3c8593f8d8db1b2f4a8ef.jpg" alt="Ảnh cá nhân">
        </div>
      </div>

      <div class="right">
        <h2>Minh Tú</h2>
        <div class="meta">Học sinh lớp 12 Anh — THPT Chuyên Bến Tre</div>

        <div class="about">
          <p>
            Xin chào! Mình là <strong>Minh Tú</strong>, hiện là học sinh lớp 12 Anh tại trường THPT Chuyên Bến Tre.
            Đây sẽ là nơi mình chia sẻ đôi nét về bản thân để mọi người hiểu hơn về mình.
          </p>
        </div>
      </div>
    </div>
  </div>

  <button class="home-btn" onclick="window.location.href='index.html'">⬅ Quay lại trang chủ</button>

  <footer>© 2025 — Trang cá nhân của Minh Tú</footer>

</body>
</html>
