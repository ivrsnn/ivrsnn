<div align="center"> <!-- HEADER SECTION --> <img src="https://capsule-render.vercel.app/api?type=soft&color=00FFFF&height=190&section=header&text=IVERSON&fontSize=80&fontAlignY=40&animation=twinkling&desc=UI/UX%20%7C%20Front-End%20Developer&descSize=20&descAlignY=60" alt="Header" />
<!-- GLITCH EFFECT TYPING -->
<div style="font-family:'Orbitron',monospace;font-weight:900;font-size:32px;text-align:center;background:#0a0f1e;padding:20px;" id="typing"></div>
<script>
(async function(){
    const lines=["WELCOME TO MY GITHUB","BUILDING THE FUTURE WITH CODE"];
    const colors=["#ff0040","#ff8000","#ffff00","#80ff00","#00ff80","#00ffff","#0080ff","#8000ff","#ff00ff"];
    const el=document.getElementById("typing");
    async function type(line,index){
        let i=0;
        while(i<=line.length){
            let html='<div style="margin:10px 0">';
            for(let j=0;j<i;j++){
                const c=line[j];
                const col=colors[j%colors.length];
                html+=`<span style="display:inline-block;color:${col};text-shadow:0 0 8px ${col}">${c===' '?'&nbsp;':c}</span>`;
            }
            html+='</div>';
            if(index===0) el.innerHTML=html;
            else el.innerHTML=el.innerHTML.split('</div>')[0]+html.split('<div')[1];
            await new Promise(r=>setTimeout(r,70));
            i++;
        }
    }
    while(true){
        await type(lines[0],0);
        await new Promise(r=>setTimeout(r,400));
        await type(lines[1],1);
        await new Promise(r=>setTimeout(r,2500));
        await type('',1);
        await type('',0);
        await new Promise(r=>setTimeout(r,500));
    }
})();
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
