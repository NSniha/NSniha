<svg width="1600" height="500" viewBox="0 0 1600 500" fill="none" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1600" y2="500" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="#081C15"/>
      <stop offset="50%" stop-color="#0B3B2E"/>
      <stop offset="100%" stop-color="#123F33"/>
    </linearGradient>

    <linearGradient id="glass" x1="820" y1="80" x2="1480" y2="380" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="rgba(255,255,255,0.22)"/>
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)"/>
    </linearGradient>

    <linearGradient id="accent" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#6EE7B7"/>
      <stop offset="100%" stop-color="#D1FAE5"/>
    </linearGradient>

    <filter id="blur1" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="40"/>
    </filter>

    <filter id="shadow" x="-20%" y="-20%" width="140%" height="140%">
      <feDropShadow dx="0" dy="18" stdDeviation="25" flood-color="#02120D" flood-opacity="0.28"/>
    </filter>
  </defs>

  <!-- background -->
  <rect width="1600" height="500" rx="0" fill="url(#bg)"/>

  <!-- soft glow blobs -->
  <circle cx="180" cy="90" r="140" fill="#14532D" opacity="0.35" filter="url(#blur1)"/>
  <circle cx="470" cy="410" r="180" fill="#0F766E" opacity="0.18" filter="url(#blur1)"/>
  <circle cx="1380" cy="80" r="160" fill="#22C55E" opacity="0.10" filter="url(#blur1)"/>

  <!-- abstract rings -->
  <circle cx="220" cy="250" r="170" stroke="#D1FAE5" stroke-opacity="0.10" stroke-width="2"/>
  <circle cx="220" cy="250" r="210" stroke="#D1FAE5" stroke-opacity="0.06" stroke-width="2"/>
  <circle cx="220" cy="250" r="250" stroke="#D1FAE5" stroke-opacity="0.04" stroke-width="2"/>

  <!-- grid dots -->
  <g opacity="0.20">
    <circle cx="116" cy="126" r="3" fill="#ECFDF5"/>
    <circle cx="146" cy="126" r="3" fill="#ECFDF5"/>
    <circle cx="176" cy="126" r="3" fill="#ECFDF5"/>
    <circle cx="206" cy="126" r="3" fill="#ECFDF5"/>
    <circle cx="236" cy="126" r="3" fill="#ECFDF5"/>

    <circle cx="116" cy="156" r="3" fill="#ECFDF5"/>
    <circle cx="146" cy="156" r="3" fill="#ECFDF5"/>
    <circle cx="176" cy="156" r="3" fill="#ECFDF5"/>
    <circle cx="206" cy="156" r="3" fill="#ECFDF5"/>
    <circle cx="236" cy="156" r="3" fill="#ECFDF5"/>

    <circle cx="116" cy="186" r="3" fill="#ECFDF5"/>
    <circle cx="146" cy="186" r="3" fill="#ECFDF5"/>
    <circle cx="176" cy="186" r="3" fill="#ECFDF5"/>
    <circle cx="206" cy="186" r="3" fill="#ECFDF5"/>
    <circle cx="236" cy="186" r="3" fill="#ECFDF5"/>
  </g>

  <!-- decorative lines -->
  <path d="M0 410C180 360 300 350 470 400C610 440 760 445 910 395C1070 342 1240 330 1600 410V500H0V410Z" fill="#071611" opacity="0.35"/>
  <path d="M0 430C200 385 370 390 540 430C700 468 810 470 970 430C1140 388 1310 382 1600 445" stroke="#A7F3D0" stroke-opacity="0.13" stroke-width="2"/>

  <!-- right content card -->
  <g filter="url(#shadow)">
    <rect x="760" y="78" width="700" height="310" rx="28" fill="url(#glass)" stroke="rgba(255,255,255,0.16)"/>
  </g>

  <!-- small label -->
  <rect x="820" y="122" width="168" height="34" rx="17" fill="#ECFDF5" fill-opacity="0.10" stroke="#ECFDF5" stroke-opacity="0.18"/>
  <text x="904" y="144" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-size="16" font-weight="600" fill="#D1FAE5">
    Front-End Developer
  </text>

  <!-- main title -->
  <text x="820" y="220" font-family="Inter, Arial, sans-serif" font-size="54" font-weight="800" fill="#F0FDF4">
    Nobonita
  </text>
  <text x="820" y="282" font-family="Inter, Arial, sans-serif" font-size="54" font-weight="800" fill="#F0FDF4">
    Saha Niha
  </text>

  <!-- accent line -->
  <rect x="820" y="312" width="180" height="6" rx="3" fill="url(#accent)"/>

  <!-- subtitle -->
  <text x="820" y="356" font-family="Inter, Arial, sans-serif" font-size="24" font-weight="500" fill="#CFEFDF">
    Building modern, responsive, and polished web experiences
  </text>

  <!-- side stats blocks -->
  <rect x="1260" y="126" width="138" height="78" rx="18" fill="#ECFDF5" fill-opacity="0.08" stroke="#ECFDF5" stroke-opacity="0.15"/>
  <text x="1329" y="156" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-size="15" fill="#BFE7D4">Focus</text>
  <text x="1329" y="184" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-size="18" font-weight="700" fill="#F0FDF4">React UI</text>

  <rect x="1260" y="222" width="138" height="78" rx="18" fill="#ECFDF5" fill-opacity="0.08" stroke="#ECFDF5" stroke-opacity="0.15"/>
  <text x="1329" y="252" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-size="15" fill="#BFE7D4">Style</text>
  <text x="1329" y="280" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-size="18" font-weight="700" fill="#F0FDF4">Clean Design</text>

  <!-- left badge -->
  <g filter="url(#shadow)">
    <rect x="120" y="292" width="270" height="82" rx="22" fill="#ECFDF5" fill-opacity="0.08" stroke="#ECFDF5" stroke-opacity="0.14"/>
  </g>
  <text x="155" y="326" font-family="Inter, Arial, sans-serif" font-size="15" fill="#A7F3D0">Creative Direction</text>
  <text x="155" y="355" font-family="Inter, Arial, sans-serif" font-size="20" font-weight="700" fill="#F0FDF4">Design with clarity</text>
</svg>

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
