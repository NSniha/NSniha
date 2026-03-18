<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nobonita Saha Niha — README Header</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,700&family=Sora:wght@300;400;600&family=Caveat:wght@600&display=swap" rel="stylesheet">
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background: #0a0a0a;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    font-family: 'Sora', sans-serif;
  }

  .banner {
    position: relative;
    width: 900px;
    height: 320px;
    overflow: hidden;
    border-radius: 16px;
    background: linear-gradient(135deg, #0b1a12 0%, #0d2818 30%, #143d24 60%, #1a5c35 100%);
    box-shadow: 0 30px 80px rgba(0, 0, 0, 0.6), 0 0 0 1px rgba(255,255,255,0.04);
  }

  /* === ANIMATED MESH GRID === */
  .mesh-grid {
    position: absolute;
    inset: 0;
    overflow: hidden;
    opacity: 0.12;
  }

  .mesh-grid svg {
    width: 100%;
    height: 100%;
  }

  /* === FLOATING ORB PARTICLES === */
  .orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(40px);
    animation: drift 8s ease-in-out infinite;
  }

  .orb-1 {
    width: 200px; height: 200px;
    background: radial-gradient(circle, rgba(34, 197, 94, 0.35), transparent 70%);
    top: -40px; right: 80px;
    animation-delay: 0s;
    animation-duration: 10s;
  }

  .orb-2 {
    width: 160px; height: 160px;
    background: radial-gradient(circle, rgba(16, 185, 129, 0.25), transparent 70%);
    bottom: -30px; left: 120px;
    animation-delay: -3s;
    animation-duration: 12s;
  }

  .orb-3 {
    width: 120px; height: 120px;
    background: radial-gradient(circle, rgba(52, 211, 153, 0.2), transparent 70%);
    top: 60px; left: 350px;
    animation-delay: -6s;
    animation-duration: 9s;
  }

  @keyframes drift {
    0%, 100% { transform: translate(0, 0) scale(1); }
    25% { transform: translate(15px, -20px) scale(1.05); }
    50% { transform: translate(-10px, 15px) scale(0.95); }
    75% { transform: translate(20px, 10px) scale(1.03); }
  }

  /* === GEOMETRIC WIRE SHAPES === */
  .geo-shapes {
    position: absolute;
    inset: 0;
    pointer-events: none;
  }

  .hex-ring {
    position: absolute;
    width: 180px; height: 180px;
    top: -30px; right: -20px;
    border: 1.5px solid rgba(34, 197, 94, 0.15);
    clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
    animation: spinSlow 25s linear infinite;
  }

  .hex-ring-2 {
    position: absolute;
    width: 100px; height: 100px;
    bottom: 20px; left: 40px;
    border: 1px solid rgba(52, 211, 153, 0.1);
    clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
    animation: spinSlow 20s linear infinite reverse;
  }

  .diamond {
    position: absolute;
    width: 60px; height: 60px;
    top: 40px; left: 260px;
    border: 1px solid rgba(34, 197, 94, 0.12);
    transform: rotate(45deg);
    animation: pulse 4s ease-in-out infinite;
  }

  .cross {
    position: absolute;
    width: 20px; height: 20px;
    bottom: 60px; right: 200px;
  }
  .cross::before, .cross::after {
    content: '';
    position: absolute;
    background: rgba(34, 197, 94, 0.2);
  }
  .cross::before { width: 2px; height: 100%; left: 50%; transform: translateX(-50%); }
  .cross::after { height: 2px; width: 100%; top: 50%; transform: translateY(-50%); }

  @keyframes spinSlow {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }

  @keyframes pulse {
    0%, 100% { opacity: 0.4; transform: rotate(45deg) scale(1); }
    50% { opacity: 1; transform: rotate(45deg) scale(1.15); }
  }

  /* === DOT CONSTELLATION === */
  .dots {
    position: absolute;
    inset: 0;
    pointer-events: none;
  }

  .dot {
    position: absolute;
    width: 3px; height: 3px;
    border-radius: 50%;
    background: rgba(52, 211, 153, 0.3);
    animation: twinkle 3s ease-in-out infinite;
  }

  .dot:nth-child(1) { top: 30px; left: 80px; animation-delay: 0s; }
  .dot:nth-child(2) { top: 90px; left: 180px; animation-delay: 0.5s; }
  .dot:nth-child(3) { top: 50px; left: 400px; animation-delay: 1s; }
  .dot:nth-child(4) { top: 200px; left: 60px; animation-delay: 1.5s; }
  .dot:nth-child(5) { top: 260px; left: 300px; animation-delay: 0.8s; }
  .dot:nth-child(6) { top: 140px; right: 100px; animation-delay: 2s; }
  .dot:nth-child(7) { bottom: 40px; right: 300px; animation-delay: 1.2s; }
  .dot:nth-child(8) { top: 180px; left: 500px; animation-delay: 0.3s; }

  @keyframes twinkle {
    0%, 100% { opacity: 0.2; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.8); }
  }

  /* === NOISE TEXTURE OVERLAY === */
  .noise {
    position: absolute;
    inset: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.03'/%3E%3C/svg%3E");
    pointer-events: none;
    mix-blend-mode: overlay;
  }

  /* === SCAN LINE ACCENT === */
  .scanline {
    position: absolute;
    top: 0; left: 0;
    width: 100%;
    height: 2px;
    background: linear-gradient(90deg, transparent, rgba(34, 197, 94, 0.4), transparent);
    animation: scan 4s ease-in-out infinite;
  }

  @keyframes scan {
    0% { top: -2px; opacity: 0; }
    10% { opacity: 1; }
    90% { opacity: 1; }
    100% { top: 318px; opacity: 0; }
  }

  /* === CONTENT === */
  .content {
    position: relative;
    z-index: 10;
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 100%;
    padding: 50px 60px;
  }

  .greeting {
    font-family: 'Caveat', cursive;
    font-size: 18px;
    color: rgba(52, 211, 153, 0.8);
    letter-spacing: 1px;
    margin-bottom: 6px;
    animation: fadeSlideIn 0.8s ease-out both;
  }

  .name {
    font-family: 'Playfair Display', serif;
    font-size: 46px;
    font-weight: 700;
    color: #f0fdf4;
    line-height: 1.1;
    letter-spacing: -0.5px;
    animation: fadeSlideIn 0.8s ease-out 0.15s both;
    text-shadow: 0 2px 30px rgba(0, 0, 0, 0.4);
  }

  .name span {
    color: #34d399;
  }

  .role {
    font-family: 'Sora', sans-serif;
    font-size: 14px;
    font-weight: 300;
    color: rgba(209, 250, 229, 0.6);
    letter-spacing: 4px;
    text-transform: uppercase;
    margin-top: 12px;
    animation: fadeSlideIn 0.8s ease-out 0.3s both;
  }

  .tagline {
    font-family: 'Playfair Display', serif;
    font-style: italic;
    font-size: 15px;
    color: rgba(52, 211, 153, 0.5);
    margin-top: 18px;
    animation: fadeSlideIn 0.8s ease-out 0.45s both;
  }

  .accent-line {
    width: 50px;
    height: 2px;
    background: linear-gradient(90deg, #34d399, transparent);
    margin-top: 16px;
    animation: fadeSlideIn 0.8s ease-out 0.55s both;
  }

  @keyframes fadeSlideIn {
    from { opacity: 0; transform: translateY(15px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* === CORNER ACCENTS === */
  .corner {
    position: absolute;
    width: 30px;
    height: 30px;
    z-index: 10;
  }

  .corner--tl { top: 16px; left: 16px; border-top: 1.5px solid rgba(52, 211, 153, 0.25); border-left: 1.5px solid rgba(52, 211, 153, 0.25); }
  .corner--tr { top: 16px; right: 16px; border-top: 1.5px solid rgba(52, 211, 153, 0.25); border-right: 1.5px solid rgba(52, 211, 153, 0.25); }
  .corner--bl { bottom: 16px; left: 16px; border-bottom: 1.5px solid rgba(52, 211, 153, 0.25); border-left: 1.5px solid rgba(52, 211, 153, 0.25); }
  .corner--br { bottom: 16px; right: 16px; border-bottom: 1.5px solid rgba(52, 211, 153, 0.25); border-right: 1.5px solid rgba(52, 211, 153, 0.25); }

  /* === SIDE DECORATION === */
  .side-deco {
    position: absolute;
    right: 55px;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 8px;
    z-index: 10;
  }

  .side-deco .bar {
    width: 3px;
    border-radius: 2px;
    background: rgba(34, 197, 94, 0.3);
    animation: barGrow 2s ease-in-out infinite;
  }

  .side-deco .bar:nth-child(1) { height: 20px; animation-delay: 0s; }
  .side-deco .bar:nth-child(2) { height: 35px; animation-delay: 0.2s; }
  .side-deco .bar:nth-child(3) { height: 55px; animation-delay: 0.4s; }
  .side-deco .bar:nth-child(4) { height: 40px; animation-delay: 0.6s; }
  .side-deco .bar:nth-child(5) { height: 25px; animation-delay: 0.8s; }

  @keyframes barGrow {
    0%, 100% { opacity: 0.3; transform: scaleY(1); }
    50% { opacity: 0.8; transform: scaleY(1.2); }
  }
</style>
</head>
<body>

<div class="banner">
  <!-- Background layers -->
  <div class="orb orb-1"></div>
  <div class="orb orb-2"></div>
  <div class="orb orb-3"></div>

  <div class="geo-shapes">
    <div class="hex-ring"></div>
    <div class="hex-ring-2"></div>
    <div class="diamond"></div>
    <div class="cross"></div>
  </div>

  <div class="dots">
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
    <div class="dot"></div>
  </div>

  <div class="noise"></div>
  <div class="scanline"></div>

  <!-- Corner accents -->
  <div class="corner corner--tl"></div>
  <div class="corner corner--tr"></div>
  <div class="corner corner--bl"></div>
  <div class="corner corner--br"></div>

  <!-- Side equalizer bars -->
  <div class="side-deco">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>

  <!-- Main content -->
  <div class="content">
    <div class="greeting">Hello, I'm</div>
    <h1 class="name">Nobonita Saha <span>Niha</span></h1>
    <p class="role">Front-End Developer</p>
    <p class="tagline">Think Beyond Boundaries</p>
    <div class="accent-line"></div>
  </div>
</div>

</body>
</html>


---

## 🧑‍💻 About Me

I'm **Nobonita Saha Niha**, a passionate **Front-End Developer** focused on building modern, responsive, and visually polished digital experiences. I enjoy transforming ideas into elegant user interfaces that feel clean, functional, and professional across every device.

- 🔭 Currently working on **front-end websites, landing pages, and modern UI projects**
- 🌱 Improving my expertise in **React.js, JavaScript, Tailwind CSS, and responsive development**
- 🎯 Focused on building interfaces that combine **clarity, usability, and strong visual appeal**
- ✨ Personal approach: *Design with purpose, build with precision.*

---

## 🛠️ Tech Stack

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React.js](https://img.shields.io/badge/React.js-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=NSniha&show_icons=true&theme=default&hide_border=true&bg_color=F7FBF8&title_color=0F6B4B&icon_color=0F6B4B&text_color=355B4C&ring_color=0F6B4B" height="170" alt="GitHub Stats" />
&nbsp;&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=NSniha&layout=compact&theme=default&hide_border=true&bg_color=F7FBF8&title_color=0F6B4B&text_color=355B4C" height="170" alt="Top Languages" />

</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=NSniha&theme=default&hide_border=true&background=F7FBF8&stroke=B7D4C4&ring=0F6B4B&fire=0F6B4B&currStreakLabel=0F6B4B&sideNums=355B4C&currStreakNum=355B4C&dates=6A8B7B&sideLabels=355B4C" alt="GitHub Streak" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=NSniha&bg_color=F7FBF8&color=355B4C&line=0F6B4B&point=0F6B4B&area=true&hide_border=true" width="95%" alt="Activity Graph"/>
</div>

---

## 📬 Connect With Me

<div align="center">

<a href="https://www.linkedin.com/in/nobonita-saha-niha-04b501214/">
  <img src="https://img.shields.io/badge/LinkedIn-Professional%20Profile-0F6B4B?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
<a href="https://github.com/NSniha">
  <img src="https://img.shields.io/badge/GitHub-My%20Projects-144D3B?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>
<a href="mailto:your-email@example.com">
  <img src="https://img.shields.io/badge/Email-Get%20in%20Touch-3A7A63?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:EAF4EE,50:DCEFE4,100:CFE8D8&height=140&section=footer&text=Thanks%20for%20visiting%20my%20profile&fontColor=0F6B4B&fontSize=26&fontAlignY=42&desc=Building%20modern%20interfaces%20with%20clean%20design%20and%20responsive%20thinking&descColor=4F7465&descSize=14&descAlignY=68" width="100%" />

<br />

<img src="https://komarev.com/ghpvc/?username=NSniha&style=for-the-badge&color=0F6B4B&label=PROFILE+VIEWS" alt="Profile Views" />

</div>
