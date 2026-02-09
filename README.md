<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bolt UI</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: radial-gradient(circle at top, #1a0a12, #000);
      color: white;
      min-height: 100vh;
      overflow-y: auto;
    }

    /* NAVBAR */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 50px;
      border-bottom: 1px solid rgba(255,255,255,0.1);
    }

    .logo {
      font-size: 24px;
      font-weight: bold;
      letter-spacing: 2px;
    }

    .nav-links a {
      margin-left: 25px;
      text-decoration: none;
      color: #ccc;
      transition: 0.3s;
    }

    .nav-links a:hover {
      color: #ff2a7a;
    }

    /* HERO */
    .hero {
      display: grid;
      grid-template-columns: 1.2fr 1fr;
      gap: 50px;
      padding: 80px 60px;
      background-image:
        linear-gradient(rgba(255,0,85,0.15) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,0,85,0.15) 1px, transparent 1px);
      background-size: 60px 60px;
    }

    .hero h1 {
      font-size: 52px;
      line-height: 1.2;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #ff2a7a;
      text-shadow: 0 0 15px #ff2a7a;
    }

    .hero p {
      font-size: 18px;
      color: #ccc;
      max-width: 520px;
      margin-bottom: 30px;
    }

    .btn {
      display: inline-block;
      padding: 14px 32px;
      background: #ff0055;
      color: white;
      border-radius: 10px;
      text-decoration: none;
      font-weight: bold;
      box-shadow: 0 0 20px rgba(255,0,85,0.6);
      transition: 0.3s;
    }

    .btn:hover {
      box-shadow: 0 0 35px #ff0055;
      transform: scale(1.05);
    }

    /* FRIEND CARDS */
    .friends {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 30px;
    }

    .friend {
      padding: 35px 20px;
      text-align: center;
      font-size: 22px;
      font-weight: 600;
      border-radius: 16px;
      background: rgba(255,0,85,0.08);
      border: 1px solid rgba(255,0,85,0.4);
      color: #ff2a7a;
      cursor: pointer;
      box-shadow: 0 0 15px rgba(255,0,85,0.25);
      transition: 0.35s;
    }

    .friend:hover {
      transform: translateY(-8px) scale(1.04);
      box-shadow: 0 0 25px #ff0055, 0 0 45px #ff0055;
      background: rgba(255,0,85,0.15);
      color: white;
    }

    .friend:last-child {
      grid-column: span 2;
    }

    /* RESPONSIVE */
    @media (max-width: 900px) {
      .hero {
        grid-template-columns: 1fr;
      }
      .friends {
        grid-template-columns: 1fr;
      }
      .friend:last-child {
        grid-column: span 1;
      }
    }
  </style>
</head>

<body>

  <!-- NAVBAR -->
  <div class="navbar">
    <div class="logo">BOLT UI</div>
    <div class="nav-links">
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Community</a>
    </div>
  </div>

  <!-- HERO SECTION -->
  <div class="hero">
    <div>
      <h1>Next-Gen <span>Neon UI</span><br>Landing Page</h1>
      <p>
        A clean, futuristic and professional landing page inspired by premium
        tech websites. Fully built using pure HTML & CSS with neon glow effects.
      </p>
      <a class="btn" href="#">Get Started</a>
    </div>

    <!-- FRIENDS -->
    <div class="friends">
      <div class="friend">Azeem</div>
      <div class="friend">Vinayak</div>
      <div class="friend">Satvik</div>
      <div class="friend">Rajveer</div>
      <div class="friend">Nadim</div>
    </div>
  </div>

</body>
</html>
