<div align="center"> <!-- HEADER SECTION --> <img src="https://capsule-render.vercel.app/api?type=soft&color=00FFFF&height=190&section=header&text=IVERSON&fontSize=80&fontAlignY=40&animation=twinkling&desc=UI/UX%20%7C%20Front-End%20Developer&descSize=20&descAlignY=60" alt="Header" />
<!-- GLITCH EFFECT TYPING --><style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    background: #0a0f1e;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: 'Orbitron', monospace;
    font-weight: 900;
  }
  .typing {
    font-size: 32px;
    line-height: 1.4;
    text-align: center;
  }
  .line {
    white-space: nowrap;
    margin: 15px 0;
  }
  .line span {
    display: inline-block;
    animation: pop 0.1s ease-out;
  }
  @keyframes pop {
    0% { opacity: 0; transform: scale(0.8); }
    100% { opacity: 1; transform: scale(1); }
  }
</style>

<div class="typing">
  <div class="line" id="line1"></div>
  <div class="line" id="line2"></div>
</div>

<script>
  const phrases = [
    "WELCOME TO MY GITHUB",
    "BUILDING THE FUTURE WITH CODE"
  ];
  
  // Rainbow colors (vivid, cycling per letter)
  const rainbow = [
    "#FF3366", "#FF6633", "#FF9933", "#FFCC33", "#CCFF33", "#66FF33",
    "#33FF66", "#33FFCC", "#33CCFF", "#3399FF", "#3366FF", "#6633FF",
    "#9933FF", "#CC33FF", "#FF33CC", "#FF3399"
  ];

  async function typeLine(element, text, delayMs = 70) {
    element.innerHTML = "";           // clear
    for (let i = 0; i < text.length; i++) {
      const char = text[i];
      const span = document.createElement("span");
      span.textContent = char;
      // pick a different color for each letter (cycling through rainbow)
      const colorIndex = i % rainbow.length;
      span.style.color = rainbow[colorIndex];
      span.style.textShadow = `0 0 6px ${rainbow[colorIndex]}`;
      element.appendChild(span);
      // tiny random variation for organic feel
      const wait = delayMs + (Math.random() * 20 - 10);
      await new Promise(r => setTimeout(r, wait));
    }
  }

  async function startTyping() {
    const line1 = document.getElementById("line1");
    const line2 = document.getElementById("line2");
    
    while (true) {
      await typeLine(line1, phrases[0], 75);
      await new Promise(r => setTimeout(r, 400));
      await typeLine(line2, phrases[1], 75);
      await new Promise(r => setTimeout(r, 2500));
      // erase both lines gracefully
      await typeLine(line2, "", 40);
      await typeLine(line1, "", 40);
      await new Promise(r => setTimeout(r, 600));
    }
  }

  startTyping();
</script>

<div align="center">

🌐 FRONTEND

<img src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" /> <img src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" /> <img src="https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black" /> <img src="https://img.shields.io/badge/tailwind-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" /> <img src="https://img.shields.io/badge/laravel-%23FF2D20.svg?style=for-the-badge&logo=laravel&logoColor=white" />

⚙️ BACKEND & DATABASE

<img src="https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white" /> <img src="https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white" /> 

🛠️ TOOLS

<img src="https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white" /> <img src="https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" /> <img src="https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white" />

</div>
<img src="https://capsule-render.vercel.app/api?type=waving&color=00FFFF&height=80&section=footer"/>
