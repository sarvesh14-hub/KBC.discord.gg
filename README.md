<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KBC Bot</title>
  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* === CSS START === */
    /* General */
    body {
      margin: 0;
      font-family: "Poppins", sans-serif;
      background: linear-gradient(135deg, #1e1e2f, #111123);
      color: #fff;
      text-align: center;
    }

    /* Top Header */
    .top-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 50px;
      background: #111123;
      border-bottom: 3px solid #ffcc00;
    }
    .top-left { font-size: 2em; color: #ffcc00; }
    .top-logo { width: 50px; border-radius: 10px; }

    /* Hero Box */
    .hero-box {
      background: linear-gradient(145deg, #222233, #1a1a2b);
      margin: 30px auto;
      padding: 40px 20px;
      width: 90%;
      max-width: 600px;
      border-radius: 20px;
      box-shadow: 0 0 25px rgba(255, 204, 0, 0.4);
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .hero-logo {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 3px solid #ffcc00;
      margin-bottom: 20px;
      box-shadow: 0 0 20px #ffcc00, 0 0 40px #ffcc00, 0 0 60px #ffcc00;
      animation: glow 2s infinite alternate;
    }
    @keyframes glow {
      0% { box-shadow: 0 0 10px #ffcc00, 0 0 20px #ffcc00; }
      50% { box-shadow: 0 0 20px #ffcc00, 0 0 40px #ffcc00; }
      100% { box-shadow: 0 0 30px #ffcc00, 0 0 60px #ffcc00; }
    }
    .hero-buttons {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 20px;
      flex-wrap: wrap;
    }
    .hero-buttons .btn {
      background: #ffcc00;
      color: #111123;
      padding: 12px 25px;
      border-radius: 12px;
      text-decoration: none;
      font-weight: 600;
      transition: all 0.3s ease;
      box-shadow: 0 0 10px #ffcc00;
    }
    .hero-buttons .btn:hover {
      background: #e6b800;
      transform: translateY(-3px);
      box-shadow: 0 0 20px #ffcc00, 0 0 40px #ffcc00;
    }

    /* Info Box */
    .info-box {
      background: #222233;
      margin: 20px auto;
      padding: 30px 25px;
      border-radius: 20px;
      width: 90%;
      max-width: 800px;
      box-shadow: 0 0 20px rgba(255, 204, 0, 0.2);
    }
    .info-box h2 { color: #ffcc00; margin-bottom: 15px; }
    .info-box p { font-size: 1.1em; line-height: 1.5em; }

    /* Command List */
    .command-box {
      background: #222233;
      margin: 20px auto;
      padding: 30px 20px;
      border-radius: 20px;
      width: 90%;
      max-width: 900px;
      box-shadow: 0 0 20px rgba(255, 204, 0, 0.2);
    }
    .command-box h2 { color: #ffcc00; margin-bottom: 25px; }
    .commands-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 15px;
    }
    .command-card {
      background: #111123;
      padding: 12px;
      border-radius: 10px;
      font-weight: 600;
      color: #ffcc00;
      box-shadow: 0 0 10px rgba(255, 204, 0, 0.2);
      transition: all 0.3s ease;
    }
    .command-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 20px #ffcc00, 0 0 40px #ffcc00;
    }

    /* Stats Box */
    .stats-box {
      display: flex;
      justify-content: center;
      gap: 50px;
      margin: 30px auto;
      flex-wrap: wrap;
    }
    .stat-card {
      background: #222233;
      padding: 30px 25px;
      border-radius: 20px;
      width: 200px;
      box-shadow: 0 0 20px rgba(255,204,0,0.3);
      text-align: center;
    }
    .stat-card h2 {
      font-size: 2em;
      color: #ffcc00;
      margin-bottom: 10px;
      text-shadow: 0 0 10px #ffcc00, 0 0 20px #ffcc00;
    }
    .stat-card p { font-weight: 600; }

    /* Footer */
    footer {
      padding: 25px;
      background: #111123;
      border-top: 3px solid #ffcc00;
    }

    /* Responsive */
    @media (max-width: 768px) {
      .commands-grid { grid-template-columns: repeat(auto-fit, minmax(100px, 1fr)); }
      .hero-logo { width: 100px; height: 100px; }
    }
    /* === CSS END === */
  </style>
</head>
<body>

  <!-- Top Header -->
  <header class="top-header">
    <div class="top-left">ᛕ᥇ᥴ</div>
    <img src="https://i.ibb.co/JJcfsGC/file-00000000bf0471fa99ca5491b7950f9e.png" alt="KBC Bot Logo" class="top-logo">
  </header>

  <!-- Hero Box -->
  <section class="hero-box">
    <img src="https://i.ibb.co/JJcfsGC/file-00000000bf0471fa99ca5491b7950f9e.png" alt="KBC Bot Logo" class="hero-logo">
    <div class="hero-buttons">
      <a href="https://discord.com/oauth2/authorize?client_id=1472196337050062920&permissions=8&scope=bot%20applications.commands" class="btn">Add to Server</a>
      <a href="https://discord.gg/TFfRv3yuQ" class="btn">Support Server</a>
    </div>
  </section>

  <!-- Information Box -->
  <section class="info-box">
    <h2>About KBC Bot</h2>
    <p>KBC Bot lets users play games like KBC, Dice, Quiz, Economy & more. Engage your community with fun commands, moderation tools, and interactive features!</p>
  </section>

  <!-- Command List Box -->
  <section class="command-box">
    <h2>Command List</h2>
    <div class="commands-grid">
      <div class="command-card">/kbc</div>
      <div class="command-card">/dice</div>
      <div class="command-card">/quiz</div>
      <div class="command-card">/rps</div>
      <div class="command-card">/credits</div>
      <div class="command-card">/avatar</div>
      <div class="command-card">/amitabh</div>
      <div class="command-card">/balance</div>
      <div class="command-card">/daily</div>
      <div class="command-card">/kick</div>
      <div class="command-card">/ban</div>
      <div class="command-card">/unban</div>
      <div class="command-card">/mute</div>
      <div class="command-card">/unmute</div>
      <div class="command-card">/warn</div>
      <div class="command-card">/resetwarn</div>
      <div class="command-card">/lock</div>
      <div class="command-card">/unlock</div>
      <div class="command-card">/clear</div>
      <div class="command-card">/nickname</div>
      <div class="command-card">/ticketcreate</div>
      <div class="command-card">/ticketclose</div>
      <div class="command-card">/ticketadd</div>
      <div class="command-card">/ticketremove</div>
    </div>
  </section>

  <!-- Stats Section -->
  <section class="stats-box">
    <div class="stat-card">
      <h2 id="users-counter">0</h2>
      <p>Trusted by Users</p>
    </div>
    <div class="stat-card">
      <h2 id="servers-counter">0</h2>
      <p>Joined in Servers</p>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>KBC Bot | © Powered by Open AI</p>
  </footer>

  <script>
    // === JS START ===
    function randomChange(value, range) {
      return value + Math.floor(Math.random() * (range * 2 + 1)) - range;
    }

    function updateCounter(id, value) {
      const element = document.getElementById(id);
      element.textContent = value.toLocaleString();
    }

    let users = 100559;
    let servers = 32064;

    updateCounter("users-counter", users);
    updateCounter("servers-counter", servers);

    setInterval(() => {
      users = randomChange(users, 150);
      updateCounter("users-counter", users);
    }, 5000);

    setInterval(() => {
      servers = randomChange(servers, 50);
      updateCounter("servers-counter", servers);
    }, 8000);

    // Amitabh Command Simulation
    function amitabhReply(message) {
      message = message.toLowerCase();
      if(message.includes('hello')) return "Namaskar! Kaise ho, beta?";
      if(message.includes('kbc')) return "KBC me hamesha dimag ka use karo!";
      return "Arre wah! Bahut accha sawaal hai, beta.";
    }

    console.log(amitabhReply("Hello"));
    console.log(amitabhReply("KBC game"));
    console.log(amitabhReply("Random question"));
    // === JS END ===
  </script>

</body>
</html>
