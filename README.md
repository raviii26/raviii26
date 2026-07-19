# Animated GitHub Profile — All Code in One File

> ⚠️ **Important:** GitHub strips animation tags from SVG pasted directly inline into a README. To keep the animations working, you still need to create these as **separate files** in your repo — but every piece of code is collected here in one place so you can copy them out easily.

**Repo structure you need:**
```
raviii26/raviii26/
├── README.md
├── banner.svg
├── banner-light.svg
├── lanyard.svg
├── stats.svg
├── langs.svg
├── trophies.svg
└── .github/
    └── workflows/
        └── github-snake.yml
```

---

## 1. README.md

```markdown
<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="banner.svg?v=1">
  <source media="(prefers-color-scheme: light)" srcset="banner-light.svg?v=1">
  <img src="banner.svg?v=1" alt="Ravi Sharma banner" width="100%">
</picture>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=raviii26&label=Profile%20Views&color=6366f1&style=for-the-badge" alt="profile views"/>
<img src="https://img.shields.io/github/followers/raviii26?label=Followers&style=for-the-badge&color=22D3EE" alt="followers"/>

<br/><br/>

<a href="https://www.linkedin.com/in/raviii26"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:youremail@example.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://twitter.com/raviii26"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white"/></a>

</div>

<br/>

<div align="center">
  <img src="lanyard.svg?v=1" alt="ID badge" width="260">
</div>

<br/>

## 🧑‍💻 About Me

- 🔭 Currently building **full-stack web applications** with modern JS frameworks
- 🌱 Deepening my skills in **System Design** and **Cloud Deployment**
- 👯 Looking to collaborate on **open-source** and **full-stack projects**
- 💬 Ask me about **React, Node.js, MongoDB, JavaScript/TypeScript**
- 📫 Reach me at: **youremail@example.com**

<br/>

## 🛠️ Tech Stack

<div align="center">
<img src="https://skillicons.dev/icons?i=js,ts,react,nodejs,express,mongodb,html,css,git,github,vscode,figma&theme=dark" />
</div>

<br/>

## 📊 GitHub Stats

<div align="center">
<img src="stats.svg?v=1" width="49%" alt="stats"/>
<img src="langs.svg?v=1" width="49%" alt="languages"/>
</div>

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=raviii26&theme=tokyo-night&hide_border=true" width="100%" alt="activity graph"/>
</div>

<br/>

## 🏆 Trophies

<div align="center">
<img src="trophies.svg?v=1" width="100%" alt="trophies"/>
</div>

<br/>

## 🐍 Contribution Snake

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/raviii26/raviii26/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/raviii26/raviii26/output/github-contribution-grid-snake.svg">
  <img src="https://raw.githubusercontent.com/raviii26/raviii26/output/github-contribution-grid-snake-dark.svg" width="100%" alt="snake animation">
</picture>
</div>

> The snake needs the GitHub Action below to run once — see setup notes.

<br/>

## 📌 Pinned Projects

| Project | Description | Tech |
|---|---|---|
| [your-repo-1](https://github.com/raviii26/your-repo-1) | Short description here | JavaScript |
| [your-repo-2](https://github.com/raviii26/your-repo-2) | Short description here | TypeScript |

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:22D3EE,100:6366F1&height=100&section=footer"/>
</div>
```

---

## 2. banner.svg (dark mode)

```xml
<svg width="1280" height="420" viewBox="0 0 1280 420" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <clipPath id="roundedBanner"><rect x="0" y="0" width="1280" height="420" rx="24"/></clipPath>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0b0f1a"/>
      <stop offset="45%" stop-color="#131b2e"/>
      <stop offset="100%" stop-color="#0b0f1a"/>
      <animate attributeName="x1" values="0%;30%;0%" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="100%;70%;100%" dur="10s" repeatCount="indefinite"/>
    </linearGradient>
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#6366F1"/>
      <stop offset="50%" stop-color="#22D3EE"/>
      <stop offset="100%" stop-color="#6366F1"/>
      <animate attributeName="x1" values="-100%;100%;-100%" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="0%;200%;0%" dur="6s" repeatCount="indefinite"/>
    </linearGradient>
    <linearGradient id="scanGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#22D3EE" stop-opacity="0"/>
      <stop offset="50%" stop-color="#22D3EE" stop-opacity="0.55"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
    </linearGradient>
    <radialGradient id="ringGlow" cx="50%" cy="50%" r="50%">
      <stop offset="70%" stop-color="#22D3EE" stop-opacity="0"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0.6"/>
    </radialGradient>
    <style>
      .mono { font-family: 'Courier New', monospace; }
      .sans { font-family: 'Segoe UI', Arial, sans-serif; }
      .pill { fill: #151d33; stroke: #2a3555; stroke-width: 1; }
      .pillText { fill: #9fb0e8; font-size: 15px; }
      @keyframes popIn { 0% { opacity:0; transform: translateY(14px);} 100% { opacity:1; transform: translateY(0);} }
      @keyframes flicker { 0%,19%,21%,23%,80%,100% { opacity:1;} 20%,22%,79% { opacity:0.25;} }
      @keyframes floatUp { 0% { transform: translateY(0); opacity:0;} 10% { opacity:1;} 100% { transform: translateY(-90px); opacity:0;} }
      @keyframes pulse { 0%,100% { opacity:0.55; r:34;} 50% { opacity:1; r:38;} }
      .pop1 { animation: popIn .6s ease-out .2s both; }
      .pop2 { animation: popIn .6s ease-out .5s both; }
      .pop3 { animation: popIn .6s ease-out .8s both; }
      .pop4 { animation: popIn .6s ease-out 1.1s both; }
      .pop5 { animation: popIn .6s ease-out 1.4s both; }
      .pop6 { animation: popIn .6s ease-out 1.7s both; }
      .neon { animation: flicker 4.5s infinite; }
    </style>
  </defs>

  <g clip-path="url(#roundedBanner)">
    <rect width="1280" height="420" fill="url(#bgGrad)"/>
    <rect width="1280" height="420" fill="none" stroke="#2a3555" stroke-width="2" rx="24"/>

    <!-- floating particles -->
    <circle cx="120" cy="380" r="2.5" fill="#22D3EE"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4s" begin="0s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4s" begin="0s" repeatCount="indefinite"/></circle>
    <circle cx="260" cy="400" r="2" fill="#6366F1"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="5s" begin="1s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="5s" begin="1s" repeatCount="indefinite"/></circle>
    <circle cx="980" cy="390" r="3" fill="#22D3EE"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4.5s" begin="2s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4.5s" begin="2s" repeatCount="indefinite"/></circle>
    <circle cx="1120" cy="410" r="2.2" fill="#6366F1"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="5.5s" begin="0.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="5.5s" begin="0.5s" repeatCount="indefinite"/></circle>
    <circle cx="700" cy="400" r="2.5" fill="#22D3EE"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4.2s" begin="1.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4.2s" begin="1.5s" repeatCount="indefinite"/></circle>
    <circle cx="450" cy="395" r="2" fill="#6366F1"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4.8s" begin="2.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4.8s" begin="2.5s" repeatCount="indefinite"/></circle>

    <!-- terminal line -->
    <g class="pop1">
      <rect x="48" y="36" width="560" height="26" fill="none"/>
      <text x="48" y="55" class="mono" font-size="16" fill="#22D3EE">user@dev:~$ <tspan fill="#c6d3ff">cat README.md</tspan></text>
      <rect x="268" y="42" width="9" height="16" fill="#22D3EE"><animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/></rect>
    </g>

    <!-- avatar hologram ring with initials -->
    <g transform="translate(1120,110)">
      <circle r="42" fill="#0f1626" stroke="#2a3555" stroke-width="2"/>
      <circle r="38" fill="url(#ringGlow)" style="animation: pulse 2.5s ease-in-out infinite;"/>
      <text x="0" y="10" text-anchor="middle" class="sans" font-size="30" font-weight="700" fill="url(#nameGrad)">RS</text>
      <rect x="-42" y="-42" width="84" height="0" fill="url(#scanGrad)">
        <animate attributeName="height" values="0;84;84" dur="1.6s" begin="0.3s" fill="freeze"/>
        <animate attributeName="y" values="-42;-42;46" dur="3.6s" begin="2s" repeatCount="indefinite"/>
      </rect>
    </g>

    <!-- name -->
    <g class="pop2">
      <text x="48" y="145" class="sans" font-size="58" font-weight="800" fill="url(#nameGrad)">Ravi Sharma</text>
    </g>

    <!-- cycling role titles -->
    <g class="pop3">
      <text x="50" y="185" class="mono" font-size="22" fill="#c6d3ff">
        <tspan opacity="0">
          <animate attributeName="opacity" values="0;1;1;0;0;0;0;0;0" keyTimes="0;0.02;0.3;0.33;0.66;0.68;0.98;0.99;1" dur="9s" repeatCount="indefinite"/>
          Full Stack Developer
        </tspan>
      </text>
      <text x="50" y="185" class="mono" font-size="22" fill="#c6d3ff">
        <tspan opacity="0">
          <animate attributeName="opacity" values="0;0;0;1;1;0;0;0;0" keyTimes="0;0.02;0.32;0.35;0.63;0.66;0.98;0.99;1" dur="9s" repeatCount="indefinite"/>
          MERN Stack Enthusiast
        </tspan>
      </text>
      <text x="50" y="185" class="mono" font-size="22" fill="#c6d3ff">
        <tspan opacity="0">
          <animate attributeName="opacity" values="0;0;0;0;0;0;1;1;0" keyTimes="0;0.02;0.32;0.35;0.65;0.68;0.7;0.97;1" dur="9s" repeatCount="indefinite"/>
          Building Things That Matter
        </tspan>
      </text>
    </g>

    <!-- tagline quote box -->
    <g class="pop4">
      <rect x="48" y="205" width="620" height="46" rx="8" class="pill"/>
      <text x="66" y="234" class="mono" font-size="15" fill="#8fa0d8">&gt; "Code craftsman — building things that matter."</text>
    </g>

    <!-- tech pills -->
    <g class="pop5">
      <g transform="translate(48,268)">
        <rect width="98" height="30" rx="15" class="pill"/><text x="49" y="20" text-anchor="middle" class="pillText">JavaScript</text>
      </g>
      <g transform="translate(154,268)">
        <rect width="98" height="30" rx="15" class="pill"/><text x="49" y="20" text-anchor="middle" class="pillText">TypeScript</text>
      </g>
      <g transform="translate(260,268)">
        <rect width="76" height="30" rx="15" class="pill"/><text x="38" y="20" text-anchor="middle" class="pillText">React</text>
      </g>
      <g transform="translate(344,268)">
        <rect width="92" height="30" rx="15" class="pill"/><text x="46" y="20" text-anchor="middle" class="pillText">Node.js</text>
      </g>
      <g transform="translate(444,268)">
        <rect width="102" height="30" rx="15" class="pill"/><text x="51" y="20" text-anchor="middle" class="pillText">MongoDB</text>
      </g>
      <g transform="translate(554,268)">
        <rect width="66" height="30" rx="15" class="pill"/><text x="33" y="20" text-anchor="middle" class="pillText">Git</text>
      </g>
    </g>

    <!-- stats bar -->
    <g class="pop6">
      <g transform="translate(48,330)">
        <text x="0" y="0" class="sans" font-size="24" font-weight="700" fill="#22D3EE">13</text>
        <text x="0" y="20" class="sans" font-size="12" fill="#7c8ab0">Public Repos</text>
      </g>
      <g transform="translate(160,330)">
        <text x="0" y="0" class="sans" font-size="24" font-weight="700" fill="#6366F1">2023</text>
        <text x="0" y="20" class="sans" font-size="12" fill="#7c8ab0">Coding Since</text>
      </g>
      <g transform="translate(300,330)">
        <text x="0" y="0" class="sans" font-size="24" font-weight="700" fill="#22D3EE">JS/TS</text>
        <text x="0" y="20" class="sans" font-size="12" fill="#7c8ab0">Top Stack</text>
      </g>
    </g>

    <!-- code editor card -->
    <g transform="translate(760,80)" class="pop3">
      <rect width="470" height="230" rx="12" fill="#0f1626" stroke="#2a3555" stroke-width="1.5"/>
      <rect width="470" height="30" rx="12" fill="#151d33"/>
      <circle cx="18" cy="15" r="5" fill="#ff5f56"/>
      <circle cx="36" cy="15" r="5" fill="#ffbd2e"/>
      <circle cx="54" cy="15" r="5" fill="#27c93f"/>
      <text x="235" y="20" text-anchor="middle" class="mono" font-size="12" fill="#7c8ab0">buildDreams.jsx</text>

      <text x="18" y="58" class="mono" font-size="14" fill="#c6d3ff" opacity="0"><animate attributeName="opacity" values="0;1" begin="1.8s" dur=".4s" fill="freeze"/><tspan fill="#6366F1">function</tspan> buildDreams() {</text>
      <text x="34" y="82" class="mono" font-size="14" fill="#c6d3ff" opacity="0"><animate attributeName="opacity" values="0;1" begin="2.3s" dur=".4s" fill="freeze"/><tspan fill="#22D3EE">const</tspan> passion = <tspan fill="#a6e3a1">"infinite"</tspan>;</text>
      <text x="34" y="106" class="mono" font-size="14" fill="#c6d3ff" opacity="0"><animate attributeName="opacity" values="0;1" begin="2.8s" dur=".4s" fill="freeze"/><tspan fill="#22D3EE">while</tspan> (learning) { ship(); }</text>
      <text x="34" y="130" class="mono" font-size="14" fill="#c6d3ff" opacity="0"><animate attributeName="opacity" values="0;1" begin="3.3s" dur=".4s" fill="freeze"/><tspan fill="#6366F1">return</tspan> passion;</text>
      <text x="18" y="154" class="mono" font-size="14" fill="#c6d3ff" opacity="0"><animate attributeName="opacity" values="0;1" begin="3.8s" dur=".4s" fill="freeze"/>}</text>
      <rect x="200" y="140" width="8" height="16" fill="#22D3EE" opacity="0"><animate attributeName="opacity" values="0;1;0;1;0;1" begin="4.2s" dur="1.5s" repeatCount="indefinite"/></rect>

      <text x="18" y="200" class="mono" font-size="12" fill="#7c8ab0" opacity="0"><animate attributeName="opacity" values="0;1" begin="4.5s" dur=".4s" fill="freeze"/>✓ Build successful — deployed with ♥</text>
    </g>

    <!-- neon sign -->
    <text x="640" y="392" text-anchor="middle" class="sans neon" font-size="20" font-weight="700" fill="#22D3EE" style="letter-spacing:3px;">KEEP CODING · KEEP GROWING</text>

    <!-- horizontal scanner sweep -->
    <rect x="0" y="0" width="1280" height="4" fill="url(#scanGrad)" opacity="0.8">
      <animate attributeName="y" values="0;420;0" dur="3.5s" repeatCount="indefinite" begin="2.5s"/>
    </rect>
  </g>
</svg>
```

---

## 3. banner-light.svg (light mode)

```xml
<svg width="1280" height="420" viewBox="0 0 1280 420" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <clipPath id="roundedBanner"><rect x="0" y="0" width="1280" height="420" rx="24"/></clipPath>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#f5f7fc"/>
      <stop offset="45%" stop-color="#eef1fb"/>
      <stop offset="100%" stop-color="#f5f7fc"/>
      <animate attributeName="x1" values="0%;30%;0%" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="100%;70%;100%" dur="10s" repeatCount="indefinite"/>
    </linearGradient>
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#6366F1"/>
      <stop offset="50%" stop-color="#22D3EE"/>
      <stop offset="100%" stop-color="#6366F1"/>
      <animate attributeName="x1" values="-100%;100%;-100%" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="0%;200%;0%" dur="6s" repeatCount="indefinite"/>
    </linearGradient>
    <linearGradient id="scanGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#22D3EE" stop-opacity="0"/>
      <stop offset="50%" stop-color="#22D3EE" stop-opacity="0.55"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
    </linearGradient>
    <radialGradient id="ringGlow" cx="50%" cy="50%" r="50%">
      <stop offset="70%" stop-color="#22D3EE" stop-opacity="0"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0.6"/>
    </radialGradient>
    <style>
      .mono { font-family: 'Courier New', monospace; }
      .sans { font-family: 'Segoe UI', Arial, sans-serif; }
      .pill { fill: #e7ebf9; stroke: #c9d3ee; stroke-width: 1; }
      .pillText { fill: #4a5580; font-size: 15px; }
      @keyframes popIn { 0% { opacity:0; transform: translateY(14px);} 100% { opacity:1; transform: translateY(0);} }
      @keyframes flicker { 0%,19%,21%,23%,80%,100% { opacity:1;} 20%,22%,79% { opacity:0.25;} }
      @keyframes floatUp { 0% { transform: translateY(0); opacity:0;} 10% { opacity:1;} 100% { transform: translateY(-90px); opacity:0;} }
      @keyframes pulse { 0%,100% { opacity:0.55; r:34;} 50% { opacity:1; r:38;} }
      .pop1 { animation: popIn .6s ease-out .2s both; }
      .pop2 { animation: popIn .6s ease-out .5s both; }
      .pop3 { animation: popIn .6s ease-out .8s both; }
      .pop4 { animation: popIn .6s ease-out 1.1s both; }
      .pop5 { animation: popIn .6s ease-out 1.4s both; }
      .pop6 { animation: popIn .6s ease-out 1.7s both; }
      .neon { animation: flicker 4.5s infinite; }
    </style>
  </defs>

  <g clip-path="url(#roundedBanner)">
    <rect width="1280" height="420" fill="url(#bgGrad)"/>
    <rect width="1280" height="420" fill="none" stroke="#c9d3ee" stroke-width="2" rx="24"/>

    <!-- floating particles -->
    <circle cx="120" cy="380" r="2.5" fill="#22D3EE"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4s" begin="0s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4s" begin="0s" repeatCount="indefinite"/></circle>
    <circle cx="260" cy="400" r="2" fill="#6366F1"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="5s" begin="1s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="5s" begin="1s" repeatCount="indefinite"/></circle>
    <circle cx="980" cy="390" r="3" fill="#22D3EE"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4.5s" begin="2s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4.5s" begin="2s" repeatCount="indefinite"/></circle>
    <circle cx="1120" cy="410" r="2.2" fill="#6366F1"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="5.5s" begin="0.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="5.5s" begin="0.5s" repeatCount="indefinite"/></circle>
    <circle cx="700" cy="400" r="2.5" fill="#22D3EE"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4.2s" begin="1.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4.2s" begin="1.5s" repeatCount="indefinite"/></circle>
    <circle cx="450" cy="395" r="2" fill="#6366F1"><animateTransform attributeName="transform" type="translate" values="0,0;0,-90" dur="4.8s" begin="2.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;1;0" dur="4.8s" begin="2.5s" repeatCount="indefinite"/></circle>

    <!-- terminal line -->
    <g class="pop1">
      <rect x="48" y="36" width="560" height="26" fill="none"/>
      <text x="48" y="55" class="mono" font-size="16" fill="#22D3EE">user@dev:~$ <tspan fill="#2a3555">cat README.md</tspan></text>
      <rect x="268" y="42" width="9" height="16" fill="#22D3EE"><animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/></rect>
    </g>

    <!-- avatar hologram ring with initials -->
    <g transform="translate(1120,110)">
      <circle r="42" fill="#ffffff" stroke="#c9d3ee" stroke-width="2"/>
      <circle r="38" fill="url(#ringGlow)" style="animation: pulse 2.5s ease-in-out infinite;"/>
      <text x="0" y="10" text-anchor="middle" class="sans" font-size="30" font-weight="700" fill="url(#nameGrad)">RS</text>
      <rect x="-42" y="-42" width="84" height="0" fill="url(#scanGrad)">
        <animate attributeName="height" values="0;84;84" dur="1.6s" begin="0.3s" fill="freeze"/>
        <animate attributeName="y" values="-42;-42;46" dur="3.6s" begin="2s" repeatCount="indefinite"/>
      </rect>
    </g>

    <!-- name -->
    <g class="pop2">
      <text x="48" y="145" class="sans" font-size="58" font-weight="800" fill="url(#nameGrad)">Ravi Sharma</text>
    </g>

    <!-- cycling role titles -->
    <g class="pop3">
      <text x="50" y="185" class="mono" font-size="22" fill="#2a3555">
        <tspan opacity="0">
          <animate attributeName="opacity" values="0;1;1;0;0;0;0;0;0" keyTimes="0;0.02;0.3;0.33;0.66;0.68;0.98;0.99;1" dur="9s" repeatCount="indefinite"/>
          Full Stack Developer
        </tspan>
      </text>
      <text x="50" y="185" class="mono" font-size="22" fill="#2a3555">
        <tspan opacity="0">
          <animate attributeName="opacity" values="0;0;0;1;1;0;0;0;0" keyTimes="0;0.02;0.32;0.35;0.63;0.66;0.98;0.99;1" dur="9s" repeatCount="indefinite"/>
          MERN Stack Enthusiast
        </tspan>
      </text>
      <text x="50" y="185" class="mono" font-size="22" fill="#2a3555">
        <tspan opacity="0">
          <animate attributeName="opacity" values="0;0;0;0;0;0;1;1;0" keyTimes="0;0.02;0.32;0.35;0.65;0.68;0.7;0.97;1" dur="9s" repeatCount="indefinite"/>
          Building Things That Matter
        </tspan>
      </text>
    </g>

    <!-- tagline quote box -->
    <g class="pop4">
      <rect x="48" y="205" width="620" height="46" rx="8" class="pill"/>
      <text x="66" y="234" class="mono" font-size="15" fill="#4a5580">&gt; "Code craftsman — building things that matter."</text>
    </g>

    <!-- tech pills -->
    <g class="pop5">
      <g transform="translate(48,268)">
        <rect width="98" height="30" rx="15" class="pill"/><text x="49" y="20" text-anchor="middle" class="pillText">JavaScript</text>
      </g>
      <g transform="translate(154,268)">
        <rect width="98" height="30" rx="15" class="pill"/><text x="49" y="20" text-anchor="middle" class="pillText">TypeScript</text>
      </g>
      <g transform="translate(260,268)">
        <rect width="76" height="30" rx="15" class="pill"/><text x="38" y="20" text-anchor="middle" class="pillText">React</text>
      </g>
      <g transform="translate(344,268)">
        <rect width="92" height="30" rx="15" class="pill"/><text x="46" y="20" text-anchor="middle" class="pillText">Node.js</text>
      </g>
      <g transform="translate(444,268)">
        <rect width="102" height="30" rx="15" class="pill"/><text x="51" y="20" text-anchor="middle" class="pillText">MongoDB</text>
      </g>
      <g transform="translate(554,268)">
        <rect width="66" height="30" rx="15" class="pill"/><text x="33" y="20" text-anchor="middle" class="pillText">Git</text>
      </g>
    </g>

    <!-- stats bar -->
    <g class="pop6">
      <g transform="translate(48,330)">
        <text x="0" y="0" class="sans" font-size="24" font-weight="700" fill="#22D3EE">13</text>
        <text x="0" y="20" class="sans" font-size="12" fill="#5c6690">Public Repos</text>
      </g>
      <g transform="translate(160,330)">
        <text x="0" y="0" class="sans" font-size="24" font-weight="700" fill="#6366F1">2023</text>
        <text x="0" y="20" class="sans" font-size="12" fill="#5c6690">Coding Since</text>
      </g>
      <g transform="translate(300,330)">
        <text x="0" y="0" class="sans" font-size="24" font-weight="700" fill="#22D3EE">JS/TS</text>
        <text x="0" y="20" class="sans" font-size="12" fill="#5c6690">Top Stack</text>
      </g>
    </g>

    <!-- code editor card -->
    <g transform="translate(760,80)" class="pop3">
      <rect width="470" height="230" rx="12" fill="#ffffff" stroke="#c9d3ee" stroke-width="1.5"/>
      <rect width="470" height="30" rx="12" fill="#e7ebf9"/>
      <circle cx="18" cy="15" r="5" fill="#ff5f56"/>
      <circle cx="36" cy="15" r="5" fill="#ffbd2e"/>
      <circle cx="54" cy="15" r="5" fill="#27c93f"/>
      <text x="235" y="20" text-anchor="middle" class="mono" font-size="12" fill="#5c6690">buildDreams.jsx</text>

      <text x="18" y="58" class="mono" font-size="14" fill="#2a3555" opacity="0"><animate attributeName="opacity" values="0;1" begin="1.8s" dur=".4s" fill="freeze"/><tspan fill="#6366F1">function</tspan> buildDreams() {</text>
      <text x="34" y="82" class="mono" font-size="14" fill="#2a3555" opacity="0"><animate attributeName="opacity" values="0;1" begin="2.3s" dur=".4s" fill="freeze"/><tspan fill="#22D3EE">const</tspan> passion = <tspan fill="#a6e3a1">"infinite"</tspan>;</text>
      <text x="34" y="106" class="mono" font-size="14" fill="#2a3555" opacity="0"><animate attributeName="opacity" values="0;1" begin="2.8s" dur=".4s" fill="freeze"/><tspan fill="#22D3EE">while</tspan> (learning) { ship(); }</text>
      <text x="34" y="130" class="mono" font-size="14" fill="#2a3555" opacity="0"><animate attributeName="opacity" values="0;1" begin="3.3s" dur=".4s" fill="freeze"/><tspan fill="#6366F1">return</tspan> passion;</text>
      <text x="18" y="154" class="mono" font-size="14" fill="#2a3555" opacity="0"><animate attributeName="opacity" values="0;1" begin="3.8s" dur=".4s" fill="freeze"/>}</text>
      <rect x="200" y="140" width="8" height="16" fill="#22D3EE" opacity="0"><animate attributeName="opacity" values="0;1;0;1;0;1" begin="4.2s" dur="1.5s" repeatCount="indefinite"/></rect>

      <text x="18" y="200" class="mono" font-size="12" fill="#5c6690" opacity="0"><animate attributeName="opacity" values="0;1" begin="4.5s" dur=".4s" fill="freeze"/>✓ Build successful — deployed with ♥</text>
    </g>

    <!-- neon sign -->
    <text x="640" y="392" text-anchor="middle" class="sans neon" font-size="20" font-weight="700" fill="#22D3EE" style="letter-spacing:3px;">KEEP CODING · KEEP GROWING</text>

    <!-- horizontal scanner sweep -->
    <rect x="0" y="0" width="1280" height="4" fill="url(#scanGrad)" opacity="0.8">
      <animate attributeName="y" values="0;420;0" dur="3.5s" repeatCount="indefinite" begin="2.5s"/>
    </rect>
  </g>
</svg>
```

---

## 4. lanyard.svg (swinging ID badge)

```xml
<svg width="360" height="480" viewBox="0 0 360 480" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="strapGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#6366F1"/>
      <stop offset="100%" stop-color="#22D3EE"/>
    </linearGradient>
    <linearGradient id="cardGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#111a2e"/>
      <stop offset="100%" stop-color="#0a0f1c"/>
    </linearGradient>
    <linearGradient id="shine" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0"/>
      <stop offset="45%" stop-color="#ffffff" stop-opacity="0.35"/>
      <stop offset="55%" stop-color="#ffffff" stop-opacity="0.35"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
    </linearGradient>
    <radialGradient id="avatarGlow" cx="50%" cy="50%" r="50%">
      <stop offset="65%" stop-color="#22D3EE" stop-opacity="0"/>
      <stop offset="100%" stop-color="#22D3EE" stop-opacity="0.7"/>
    </radialGradient>
    <style>
      .mono { font-family: 'Courier New', monospace; }
      .sans { font-family: 'Segoe UI', Arial, sans-serif; }
      @keyframes swing {
        0%   { transform: rotate(0deg); }
        8%   { transform: rotate(9deg); }
        20%  { transform: rotate(-7deg); }
        32%  { transform: rotate(5deg); }
        44%  { transform: rotate(-3.5deg); }
        56%  { transform: rotate(2.2deg); }
        68%  { transform: rotate(-1.3deg); }
        80%  { transform: rotate(0.7deg); }
        90%  { transform: rotate(-0.3deg); }
        100% { transform: rotate(0deg); }
      }
      @keyframes drop {
        0%   { transform: translateY(-260px); opacity: 0; }
        60%  { transform: translateY(10px); opacity: 1; }
        75%  { transform: translateY(-8px); }
        88%  { transform: translateY(4px); }
        100% { transform: translateY(0px); }
      }
      #rig {
        animation: drop 1.1s cubic-bezier(.34,1.4,.64,1) both,
                   swing 6s ease-in-out 1.1s infinite;
        transform-origin: 180px 40px;
      }
    </style>
  </defs>

  <!-- fixed anchor -->
  <rect x="164" y="0" width="32" height="14" rx="4" fill="#2a3555"/>

  <g id="rig">
    <!-- strap -->
    <polygon points="170,10 190,10 210,230 150,230" fill="url(#strapGrad)"/>
    <text x="180" y="120" text-anchor="middle" class="mono" font-size="11" fill="#0b0f1a" transform="rotate(90 180 120)" opacity="0.5">RAVI · DEV · RAVI · DEV</text>

    <!-- clasp + ring -->
    <rect x="160" y="222" width="40" height="18" rx="6" fill="#c9d3ee" stroke="#8b98c4" stroke-width="1.5"/>
    <circle cx="180" cy="248" r="12" fill="none" stroke="#c9d3ee" stroke-width="5"/>

    <!-- card -->
    <g transform="translate(30,255)">
      <rect x="0" y="0" width="300" height="200" rx="18" fill="url(#cardGrad)" stroke="#2a3555" stroke-width="1.5"/>

      <!-- avatar -->
      <g transform="translate(60,58)">
        <circle r="34" fill="url(#avatarGlow)"/>
        <circle r="30" fill="#0f1626" stroke="#22D3EE" stroke-width="2"/>
        <text x="0" y="9" text-anchor="middle" class="sans" font-size="24" font-weight="700" fill="#22D3EE">RS</text>
      </g>

      <text x="115" y="42" class="sans" font-size="19" font-weight="700" fill="#e7ebf9">Ravi Sharma</text>
      <text x="115" y="62" class="mono" font-size="12" fill="#22D3EE">Full Stack Developer</text>
      <text x="115" y="80" class="mono" font-size="11" fill="#7c8ab0">@raviii26</text>

      <line x1="18" y1="105" x2="282" y2="105" stroke="#2a3555" stroke-width="1"/>

      <!-- barcode -->
      <g transform="translate(18,120)">
        <rect x="0" y="0" width="2" height="34" fill="#7c8ab0"/>
        <rect x="5" y="0" width="1" height="34" fill="#7c8ab0"/>
        <rect x="9" y="0" width="3" height="34" fill="#7c8ab0"/>
        <rect x="15" y="0" width="1" height="34" fill="#7c8ab0"/>
        <rect x="19" y="0" width="2" height="34" fill="#7c8ab0"/>
        <rect x="24" y="0" width="1" height="34" fill="#7c8ab0"/>
        <rect x="28" y="0" width="4" height="34" fill="#7c8ab0"/>
        <rect x="35" y="0" width="1" height="34" fill="#7c8ab0"/>
        <rect x="39" y="0" width="2" height="34" fill="#7c8ab0"/>
        <rect x="44" y="0" width="1" height="34" fill="#7c8ab0"/>
        <rect x="48" y="0" width="3" height="34" fill="#7c8ab0"/>
        <rect x="54" y="0" width="1" height="34" fill="#7c8ab0"/>
        <rect x="58" y="0" width="2" height="34" fill="#7c8ab0"/>
        <text x="0" y="48" class="mono" font-size="9" fill="#5c6690">ID-2023-RS26</text>
      </g>

      <text x="18" y="185" class="mono" font-size="10" fill="#5c6690">ACCESS: FULL-STACK LAB</text>

      <!-- holographic shine sweep -->
      <rect x="-320" y="0" width="120" height="200" fill="url(#shine)" transform="skewX(-20)">
        <animate attributeName="x" values="-160;340" dur="3s" repeatCount="indefinite" begin="1.5s"/>
      </rect>
    </g>
  </g>
</svg>
```

---

## 5. stats.svg (local stats card)

```xml
<svg width="480" height="230" viewBox="0 0 480 230" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="sRing" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#6366F1"/>
      <stop offset="100%" stop-color="#22D3EE"/>
    </linearGradient>
    <style>
      .mono { font-family: 'Courier New', monospace; }
      .sans { font-family: 'Segoe UI', Arial, sans-serif; }
      @keyframes slideIn { 0% { opacity:0; transform: translateX(-16px); } 100% { opacity:1; transform: translateX(0); } }
      .r1 { animation: slideIn .5s ease-out .1s both; }
      .r2 { animation: slideIn .5s ease-out .3s both; }
      .r3 { animation: slideIn .5s ease-out .5s both; }
      .r4 { animation: slideIn .5s ease-out .7s both; }
    </style>
  </defs>

  <rect x="1" y="1" width="478" height="228" rx="14" fill="#0d1320" stroke="#2a3555" stroke-width="1.5"/>
  <text x="24" y="36" class="sans" font-size="17" font-weight="700" fill="#e7ebf9">Ravi's GitHub Stats</text>

  <!-- rank ring -->
  <g transform="translate(100,140)">
    <circle r="52" fill="none" stroke="#1a2340" stroke-width="10"/>
    <circle r="52" fill="none" stroke="url(#sRing)" stroke-width="10" stroke-linecap="round"
      stroke-dasharray="326.7" stroke-dashoffset="326.7" transform="rotate(-90)">
      <animate attributeName="stroke-dashoffset" from="326.7" to="90" dur="1.4s" begin="0.3s" fill="freeze"/>
    </circle>
    <text x="0" y="-2" text-anchor="middle" class="sans" font-size="22" font-weight="700" fill="#22D3EE">B+</text>
    <text x="0" y="18" text-anchor="middle" class="mono" font-size="11" fill="#7c8ab0">RANK</text>
  </g>

  <!-- stat rows -->
  <g transform="translate(210,70)">
    <g class="r1">
      <text x="0" y="0" class="mono" font-size="14" fill="#c6d3ff">📦 Public Repos:</text>
      <text x="200" y="0" text-anchor="end" class="sans" font-size="14" font-weight="700" fill="#22D3EE">13</text>
    </g>
    <g class="r2">
      <text x="0" y="34" class="mono" font-size="14" fill="#c6d3ff">👥 Followers:</text>
      <text x="200" y="34" text-anchor="end" class="sans" font-size="14" font-weight="700" fill="#22D3EE">1</text>
    </g>
    <g class="r3">
      <text x="0" y="68" class="mono" font-size="14" fill="#c6d3ff">🗓️ Member Since:</text>
      <text x="200" y="68" text-anchor="end" class="sans" font-size="14" font-weight="700" fill="#22D3EE">2023</text>
    </g>
    <g class="r4">
      <text x="0" y="102" class="mono" font-size="14" fill="#c6d3ff">💻 Top Language:</text>
      <text x="200" y="102" text-anchor="end" class="sans" font-size="14" font-weight="700" fill="#22D3EE">JavaScript</text>
    </g>
  </g>
</svg>
```

---

## 6. langs.svg (local languages card)

```xml
<svg width="480" height="230" viewBox="0 0 480 230" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      .mono { font-family: 'Courier New', monospace; }
      .sans { font-family: 'Segoe UI', Arial, sans-serif; }
    </style>
  </defs>

  <rect x="1" y="1" width="478" height="228" rx="14" fill="#0d1320" stroke="#2a3555" stroke-width="1.5"/>
  <text x="24" y="36" class="sans" font-size="17" font-weight="700" fill="#e7ebf9">Most Used Languages</text>

  <g transform="translate(24,80)" class="mono" font-size="13">
    <text y="0" fill="#c6d3ff">JavaScript</text>
    <rect x="0" y="10" width="432" height="16" rx="8" fill="#1a2340"/>
    <rect x="0" y="10" width="0" height="16" rx="8" fill="#f1e05a">
      <animate attributeName="width" from="0" to="346" dur="1s" begin="0.2s" fill="freeze"/>
    </rect>
    <text x="440" y="22" text-anchor="end" fill="#f1e05a">80%</text>

    <text y="70" fill="#c6d3ff">TypeScript</text>
    <rect x="0" y="80" width="432" height="16" rx="8" fill="#1a2340"/>
    <rect x="0" y="80" width="0" height="16" rx="8" fill="#3178c6">
      <animate attributeName="width" from="0" to="86" dur="1s" begin="0.4s" fill="freeze"/>
    </rect>
    <text x="440" y="92" text-anchor="end" fill="#3178c6">20%</text>
  </g>

  <text x="24" y="205" class="mono" font-size="11" fill="#5c6690">based on primary language across public repos</text>
</svg>
```

---

## 7. trophies.svg (local trophy card)

```xml
<svg width="920" height="200" viewBox="0 0 920 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      .mono { font-family: 'Courier New', monospace; }
      .sans { font-family: 'Segoe UI', Arial, sans-serif; }
      @keyframes pop { 0% { opacity:0; transform: scale(.7); } 80% { transform: scale(1.05); } 100% { opacity:1; transform: scale(1); } }
      .t1 { animation: pop .5s ease-out .1s both; transform-origin: center; }
      .t2 { animation: pop .5s ease-out .3s both; transform-origin: center; }
      .t3 { animation: pop .5s ease-out .5s both; transform-origin: center; }
      .t4 { animation: pop .5s ease-out .7s both; transform-origin: center; }
    </style>
    <linearGradient id="shine2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0"/>
      <stop offset="50%" stop-color="#ffffff" stop-opacity="0.25"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
    </linearGradient>
  </defs>

  <!-- cell template x4 -->
  <g class="t1" transform="translate(20,15)">
    <rect width="200" height="170" rx="14" fill="#0d1320" stroke="#f1e05a" stroke-width="1.5"/>
    <text x="100" y="55" text-anchor="middle" font-size="40">🏆</text>
    <text x="100" y="90" text-anchor="middle" class="sans" font-size="13" font-weight="700" fill="#e7ebf9">Repositories</text>
    <text x="100" y="112" text-anchor="middle" class="mono" font-size="11" fill="#f1e05a">Rank C</text>
    <text x="100" y="140" text-anchor="middle" class="mono" font-size="18" fill="#7c8ab0">13</text>
    <rect x="-100" y="0" width="60" height="170" fill="url(#shine2)"><animate attributeName="x" values="-100;300" dur="2.5s" begin="1.2s" repeatCount="indefinite"/></rect>
  </g>

  <g class="t2" transform="translate(240,15)">
    <rect width="200" height="170" rx="14" fill="#0d1320" stroke="#22D3EE" stroke-width="1.5"/>
    <text x="100" y="55" text-anchor="middle" font-size="40">🌱</text>
    <text x="100" y="90" text-anchor="middle" class="sans" font-size="13" font-weight="700" fill="#e7ebf9">Experience</text>
    <text x="100" y="112" text-anchor="middle" class="mono" font-size="11" fill="#22D3EE">Growing</text>
    <text x="100" y="140" text-anchor="middle" class="mono" font-size="18" fill="#7c8ab0">since 2023</text>
    <rect x="-100" y="0" width="60" height="170" fill="url(#shine2)"><animate attributeName="x" values="-100;300" dur="2.5s" begin="1.5s" repeatCount="indefinite"/></rect>
  </g>

  <g class="t3" transform="translate(460,15)">
    <rect width="200" height="170" rx="14" fill="#0d1320" stroke="#6366F1" stroke-width="1.5"/>
    <text x="100" y="55" text-anchor="middle" font-size="40">👥</text>
    <text x="100" y="90" text-anchor="middle" class="sans" font-size="13" font-weight="700" fill="#e7ebf9">Community</text>
    <text x="100" y="112" text-anchor="middle" class="mono" font-size="11" fill="#6366F1">Building</text>
    <text x="100" y="140" text-anchor="middle" class="mono" font-size="18" fill="#7c8ab0">followers</text>
    <rect x="-100" y="0" width="60" height="170" fill="url(#shine2)"><animate attributeName="x" values="-100;300" dur="2.5s" begin="1.8s" repeatCount="indefinite"/></rect>
  </g>

  <g class="t4" transform="translate(680,15)">
    <rect width="200" height="170" rx="14" fill="#0d1320" stroke="#a6e3a1" stroke-width="1.5"/>
    <text x="100" y="55" text-anchor="middle" font-size="40">🚀</text>
    <text x="100" y="90" text-anchor="middle" class="sans" font-size="13" font-weight="700" fill="#e7ebf9">Momentum</text>
    <text x="100" y="112" text-anchor="middle" class="mono" font-size="11" fill="#a6e3a1">Shipping</text>
    <text x="100" y="140" text-anchor="middle" class="mono" font-size="18" fill="#7c8ab0">JS &amp; TS</text>
    <rect x="-100" y="0" width="60" height="170" fill="url(#shine2)"><animate attributeName="x" values="-100;300" dur="2.5s" begin="2.1s" repeatCount="indefinite"/></rect>
  </g>
</svg>
```

---

## 8. .github/workflows/github-snake.yml

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
  push:
    branches: [ main ]

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: raviii26
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark,color:#6366F1,#22D3EE,dot:#1a2340
      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

---

## Setup steps

1. Create a public repo named exactly `raviii26` (must match your username exactly)
2. Create each file above at the paths shown, pasting in its code block content
3. Before uploading, replace: `youremail@example.com` → your real email, `your-repo-1` / `your-repo-2` → your real repo names, LinkedIn/Twitter URLs → your real profiles
4. Commit everything
5. Go to the repo's **Actions** tab → enable workflows if prompted → run "Generate Snake" once
6. Visit `github.com/raviii26` — your profile is live

**Cache tip:** if you edit an SVG later and GitHub shows the old version, bump every `?v=1` in README.md to `?v=2` — that forces a fresh fetch.
