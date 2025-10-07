<!-- Animated header - use on GitHub Pages or any HTML page -->
<div align="center" class="animated-header">
  <h1 id="headline">Hello, I'm <span class="name">Anshuman</span> <span class="hand">👋</span></h1>
  <h3 id="subtitle">Machine Learning | Deep Learning | Frontend & UI/UX | Always Exploring 🚀</h3>
</div>

<style>
/* container styling */
.animated-header { 
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  color: #e6f7ff;
  background: #0b0f12; /* optional page background */
  padding: 28px 12px;
  border-radius: 8px;
  display: inline-block;
}

/* headline look */
.animated-header h1 {
  font-size: 36px;
  margin: 0;
  letter-spacing: 0.5px;
  color: #00E0FF;
  white-space: nowrap;
  overflow: hidden;
}

/* name styling (keeps color consistent) */
.animated-header .name { font-weight: 700; }

/* wave animation for emoji */
.hand {
  display: inline-block;
  transform-origin: 70% 70%;
  animation: wave 2s ease-in-out infinite;
  margin-left: 6px;
  font-size: 1.05em;
}

/* subtitle fade-in */
#subtitle {
  opacity: 0;
  margin-top: 10px;
  font-weight: 400;
  font-size: 16px;
  color: #d6eefd;
  transition: opacity 0.6s ease 0.25s;
}

/* typewriter caret effect (for the typed part) */
.cursor {
  display: inline-block;
  width: 2px;
  height: 1em;
  background: #00E0FF;
  vertical-align: middle;
  margin-left: 6px;
  animation: blink 1s steps(2, start) infinite;
}

/* keyframes */
@keyframes wave {
  0% { transform: rotate(0deg); }
  15% { transform: rotate(14deg); }
  30% { transform: rotate(-8deg); }
  40% { transform: rotate(14deg); }
  50% { transform: rotate(-4deg); }
  60% { transform: rotate(10deg); }
  100% { transform: rotate(0deg); }
}

@keyframes blink {
  0%, 50% { opacity: 1; }
  50.01%, 100% { opacity: 0; }
}

/* small responsive tweak */
@media (max-width: 520px) {
  .animated-header h1 { font-size: 24px; }
  #subtitle { font-size: 14px; }
}
</style>

<script>
/* Typing effect - types "Hello, I'm Anshuman 👋" then shows subtitle */
(function() {
  const fullText = "Hello, I'm Anshuman ";
  const headline = document.getElementById('headline');
  const subtitle = document.getElementById('subtitle');

  // Clear existing text, keep markup for name & hand intact
  headline.innerHTML = '';
  const spanText = document.createElement('span');
  spanText.id = 'typed';
  headline.appendChild(spanText);

  const handSpan = document.createElement('span');
  handSpan.className = 'hand';
  handSpan.textContent = '👋';
  headline.appendChild(handSpan);

  // cursor
  const cursor = document.createElement('span');
  cursor.className = 'cursor';
  headline.appendChild(cursor);

  let i = 0;
  function typeStep() {
    if (i < fullText.length) {
      spanText.textContent += fullText[i++];
      setTimeout(typeStep, 75 + Math.random()*80);
    } else {
      // replace typed area with styled name + remove cursor
      const typed = document.getElementById('typed').textContent;
      const name = document.createElement('span');
      name.className = 'name';
      // keep full typed text but highlight 'Anshuman'
      const visible = typed.replace('Hello, I\'m ', '');
      name.textContent = visible;
      // rebuild headline: static prefix + highlighted name + hand + no cursor
      headline.innerHTML = 'Hello, I\'m ';
      headline.appendChild(name);
      const hand = document.createElement('span');
      hand.className = 'hand';
      hand.textContent = '👋';
      headline.appendChild(hand);
      // reveal subtitle
      setTimeout(()=> { subtitle.style.opacity = 1; }, 200);
    }
  }
  // start typing after a short delay
  setTimeout(typeStep, 300);
})();
</script>


## 🧰 Tech Stack
<div align="center" style="background:#0d1117; padding:10px; border-radius:8px;">
  <img src="https://skillicons.dev/icons?i=python,tensorflow,pytorch,sklearn,opencv,react,figma,git,github,vscode&perline=10" 
       alt="Tech Stack"
       style="width:100%; border-radius:8px; margin:0; padding:0; display:block;"/>
</div>

---

## 🎓 Certifications
<p align="center">
  <img src="https://img.shields.io/badge/Internshala-Web%20Development-blue?style=for-the-badge&logo=html5&logoColor=white" alt="Internshala Web Development"/>
  <img src="https://img.shields.io/badge/Google-UI%2FUX%20Design-orange?style=for-the-badge&logo=google&logoColor=white" alt="Google UI UX Design"/>
  <img src="https://img.shields.io/badge/Laundry%20Lift-Graphic%20Designer-purple?style=for-the-badge&logo=adobecreativecloud&logoColor=white" alt="Laundry Lift Graphic Designer"/>
</p>

---
## 📊 GitHub Stats

<div align="center" style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px;">

  <!-- GitHub Stats Card -->
  <div style="flex:1; min-width:280px; max-width:340px;">
    <img src="https://github-readme-stats.vercel.app/api?username=Scorpy-ansh&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&include_all_commits=true&count_private=true&v=2" 
         alt="Anshuman's GitHub Stats" style="width:100%; border-radius:10px;"/>
  </div>

  <!-- Most Used Languages Card -->
  <div style="flex:1; min-width:280px; max-width:340px;">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Scorpy-ansh&layout=compact&theme=tokyonight&hide_border=true&v=2" 
         alt="Top Languages" style="width:100%; border-radius:10px;"/>
  </div>

  <!-- Contribution Streak Card -->
  <div style="flex:1; min-width:280px; max-width:340px;">
    <img src="https://nirzak-streak-stats.vercel.app/?user=Scorpy-ansh&theme=tokyonight&hide_border=true&date_format=j%20M%5B%20Y%5D&v=2" 
         alt="GitHub Streak Stats" style="width:100%; border-radius:10px;"/>
  </div>

</div>

---

## 🏆 GitHub Trophies
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Scorpy-ansh&theme=tokyonight&no-frame=true&no-bg=true&margin-w=10&margin-h=10&v=3" />
</p>

---
## 🚀 Featured Projects
<p align="center">

  <a href="https://github.com/Scorpy-ansh/Hindi-asr-whisper">
    <img src="https://img.shields.io/badge/Hindi--ASR--Whisper-%2300BFFF?style=for-the-badge&logo=github&logoColor=white" alt="Hindi ASR Whisper"/>
  </a>
  <a href="https://github.com/Scorpy-ansh/pedestrian-safety">
    <img src="https://img.shields.io/badge/Pedestrian--Safety-%23FF007F?style=for-the-badge&logo=github&logoColor=white" alt="Pedestrian Safety"/>
  </a>
  <a href="https://github.com/Scorpy-ansh/VGG-Image-Classification">
    <img src="https://img.shields.io/badge/VGG--Image--Classification-%23FF6F00?style=for-the-badge&logo=github&logoColor=white" alt="VGG Image Classification"/>
  </a>
  <a href="https://github.com/Scorpy-ansh/Resnet50-Image-Classification">
    <img src="https://img.shields.io/badge/ResNet50--Image--Classification-%237B68EE?style=for-the-badge&logo=github&logoColor=white" alt="ResNet50 Image Classification"/>
  </a>

</p>


## 🕹️ Contribution Graph
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Scorpy-ansh&bg_color=000000&color=00FFFF&line=ff00ff&point=ffffff&area=true&hide_border=true&v=3" alt="Anshuman's contribution graph" />
</p>

---

## 🌐 Connect With Me
<p align="center">
  <a href="https://www.linkedin.com/in/anshuman-pattanayak-3ba579338/">
    <img src="https://img.shields.io/badge/LinkedIn-0078D4?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:anshumanp1006@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://github.com/Scorpy-ansh">
    <img src="https://img.shields.io/badge/GitHub-171515?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://www.behance.net/anshumapattana4">
    <img src="https://img.shields.io/badge/Behance-1769FF?style=for-the-badge&logo=behance&logoColor=white" alt="Behance"/>
  </a>
</p>

---

## 👀 Visitor Counter
<p align="center">
  <img src="https://moe-counter.glitch.me/get/@Scorpy-ansh?theme=rule34" alt="visitor counter" />
</p>
