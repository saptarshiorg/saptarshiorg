
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Saptarshi Samanta — Web developer & creator</title>
<meta name="description" content="Saptarshi Samanta (RISHI FORGE) builds web apps, streaming platforms and open-source projects from Kolkata, West Bengal.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Unbounded:wght@600;800&family=Figtree:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#ffffff;--fg:#0a0a0f;--mute:#5d5d6b;--line:#e4e2ee;--accent:#6d28ff;--accent-ink:#ffffff;--panel:#f6f4fc;
  --disp:"Unbounded","Arial Black",system-ui,sans-serif;--body:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;
  box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#000;--fg:#f5f5fa;--mute:#9a9aae;--line:#24232f;--accent:#9d6bff;--accent-ink:#000;--panel:#0d0c14}}
:root[data-theme="dark"]{--bg:#000;--fg:#f5f5fa;--mute:#9a9aae;--line:#24232f;--accent:#9d6bff;--accent-ink:#000;--panel:#0d0c14}
*,*::before,*::after{box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:calc(72px + env(safe-area-inset-top,0px))}
body{margin:0;background:var(--bg);color:var(--fg);font:400 17px/1.65 var(--body);-webkit-font-smoothing:antialiased}
a{color:inherit}
:focus-visible{outline:2px solid var(--accent);outline-offset:3px;border-radius:4px}
.wrap{max-width:1040px;margin:0 auto;padding:0 24px}
header{position:sticky;top:env(safe-area-inset-top,0px);z-index:10;background:color-mix(in srgb,var(--bg) 88%,transparent);backdrop-filter:blur(10px);border-bottom:1px solid var(--line)}
header .wrap{display:flex;align-items:center;justify-content:space-between;height:64px;gap:16px}
.logo{font:800 15px var(--disp);text-decoration:none;letter-spacing:.02em}
.logo b{color:var(--accent)}
nav{display:flex;gap:22px;align-items:center;font-size:15px}
nav a{text-decoration:none;color:var(--mute)}
nav a:hover{color:var(--fg)}
#theme{background:none;border:1px solid var(--line);color:var(--fg);width:36px;height:36px;border-radius:50%;cursor:pointer;font-size:16px}
#theme:hover{border-color:var(--accent)}
@media (max-width:640px){nav a{display:none}}

/* hero */
.hero{padding:clamp(56px,10vw,120px) 0 72px;border-bottom:1px solid var(--line)}
.hero .where{color:var(--mute);margin:0 0 20px}
h1{font:800 clamp(40px,10.5vw,112px)/.98 var(--disp);letter-spacing:-.035em;margin:0}
h1 span{display:block;overflow:hidden}
h1 span i{display:inline-block;font-style:normal;transform:translateY(105%);animation:up .9s cubic-bezier(.2,.8,.2,1) forwards}
h1 span:nth-child(2) i{animation-delay:.12s;color:var(--accent)}
@keyframes up{to{transform:none}}
.lede{max-width:540px;font-size:19px;margin:28px 0 0}
.age{margin-top:44px;display:inline-flex;flex-direction:column;border-left:3px solid var(--accent);padding-left:18px}
.age output{font:600 clamp(26px,5vw,40px)/1.1 var(--disp);font-variant-numeric:tabular-nums;letter-spacing:-.02em}
.age small{color:var(--mute);font-size:14px;margin:0 0 8px}
.bday{margin-top:36px}
.bday small{display:block;color:var(--mute);font-size:14px;margin-bottom:10px}
.units{display:flex;flex-wrap:wrap;gap:10px}
.units div{min-width:84px;border:1px solid var(--line);border-radius:14px;padding:12px 16px;background:var(--panel)}
.units b{display:block;font:800 clamp(22px,4.5vw,30px)/1 var(--disp);font-variant-numeric:tabular-nums;letter-spacing:-.02em}
.units span{color:var(--mute);font-size:13px}
.roles{display:flex;flex-wrap:wrap;gap:8px;list-style:none;margin:32px 0 0;padding:0}
.roles li{border:1px solid var(--line);padding:8px 16px;border-radius:999px;font-weight:600;font-size:15px}
.cta{display:flex;flex-wrap:wrap;gap:12px;margin-top:40px}
.btn{display:inline-block;padding:13px 22px;border-radius:999px;text-decoration:none;font-weight:600;border:1px solid var(--line);transition:transform .2s,background .2s}
.btn{display:inline-flex;align-items:center;gap:10px}
.ic{width:18px;height:18px;flex:none}
.btn.primary{background:var(--accent);color:var(--accent-ink);border-color:var(--accent)}
.btn:hover{transform:translateY(-2px)}

/* sections */
section{padding:84px 0;border-bottom:1px solid var(--line)}
h2{font:800 clamp(26px,4.4vw,40px)/1.1 var(--disp);letter-spacing:-.025em;margin:0 0 28px}
.two{display:grid;grid-template-columns:1fr 1fr;gap:48px}
@media (max-width:760px){.two{grid-template-columns:1fr;gap:28px}}
p{margin:0 0 16px;max-width:62ch}
.mute{color:var(--mute)}
.facts{list-style:none;margin:0;padding:0}
.facts li{display:flex;justify-content:space-between;gap:16px;padding:12px 0;border-bottom:1px solid var(--line)}
.facts li span:first-child{color:var(--mute)}

/* featured */
.feature{background:var(--panel);border:1px solid var(--line);border-radius:20px;padding:clamp(24px,5vw,48px)}
.feature h3{font:800 clamp(28px,5vw,48px)/1 var(--disp);letter-spacing:-.03em;margin:0 0 6px}
.feature .tag{color:var(--accent);font-weight:600;margin:0 0 18px}
.chips{display:flex;flex-wrap:wrap;gap:8px;margin:22px 0 28px;padding:0;list-style:none}
.chips li{border:1px solid var(--line);background:var(--bg);padding:6px 14px;border-radius:999px;font-size:15px}

/* project list */
.list{border-top:1px solid var(--line)}
.row{display:grid;grid-template-columns:1.1fr 2fr auto;gap:24px;align-items:baseline;padding:22px 0;border-bottom:1px solid var(--line);text-decoration:none;transition:padding .25s}
.row:hover{padding-left:12px}
.row:hover .name{color:var(--accent)}
.row .name{font:600 18px var(--disp);letter-spacing:-.01em;transition:color .2s}
.row .lang{color:var(--mute);font-size:15px}
@media (max-width:700px){.row{grid-template-columns:1fr;gap:4px}}

/* stack */
.stack{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:36px}
.stack h3{font:600 15px var(--disp);margin:0 0 12px}
.stack ul{list-style:none;margin:0;padding:0;color:var(--mute)}
.stack li{padding:3px 0}

/* stats */
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:0;border:1px solid var(--line);border-radius:16px;overflow:hidden}
.stats div{padding:26px;border-right:1px solid var(--line)}
.stats div:last-child{border-right:0}
.stats strong{display:block;font:800 36px/1 var(--disp);letter-spacing:-.03em}
.stats span{color:var(--mute);font-size:15px}
@media (max-width:640px){.stats div{border-right:0;border-bottom:1px solid var(--line)}.stats div:last-child{border-bottom:0}}

/* location */
.map{border:1px solid var(--line);border-radius:20px;background:var(--panel);padding:12px;overflow:hidden}
.map svg{display:block;width:100%;height:auto}
.map .grid{stroke:var(--line);stroke-width:1}
.map .route{stroke:var(--accent);stroke-width:2;stroke-dasharray:6 7;fill:none}
.map .pt{fill:var(--accent)}
.map .ring{fill:none;stroke:var(--accent);stroke-width:2;opacity:.45;transform-box:fill-box;transform-origin:center;animation:ping 2.4s ease-out infinite}
@keyframes ping{from{transform:scale(.5);opacity:.7}to{transform:scale(2.2);opacity:0}}
.map text{fill:var(--fg);font:600 15px var(--body)}
.map text.sub{fill:var(--mute);font:400 13px var(--body)}
.loc-links{display:flex;flex-wrap:wrap;gap:12px;margin-top:20px}

footer{padding:56px 0 72px}
.mail{font:800 clamp(18px,3.8vw,40px)/1.15 var(--disp);letter-spacing:-.03em;text-decoration:none;display:block;margin-bottom:28px;overflow-wrap:anywhere}
.mail:hover{color:var(--accent)}
.links{display:flex;flex-wrap:wrap;gap:12px}
.fine{color:var(--mute);font-size:14px;margin-top:40px}

@media (prefers-reduced-motion:reduce){
  html{scroll-behavior:auto}
  h1 span i{animation:none;transform:none}
  .btn,.row{transition:none}
  .map .ring{animation:none;opacity:.4}
}
</style>
</head>
<body>
<header>
  <div class="wrap">
    <a class="logo" href="#top">RISHI<b>FORGE</b></a>
    <nav aria-label="Main">
      <a href="#about">About</a>
      <a href="#location">Location</a>
      <a href="#featured">EV STREAMS</a>
      <a href="#stack">Stack</a>
      <a href="#contact">Contact</a>
      <button id="theme" type="button" aria-label="Switch light or dark theme">◐</button>
    </nav>
  </div>
</header>

<main id="top">
  <div class="hero">
    <div class="wrap">
      <p class="where">Kolkata, West Bengal, India</p>
      <h1 aria-label="Saptarshi Samanta"><span><i>Saptarshi</i></span><span><i>Samanta</i></span></h1>
      <p class="lede">I build web apps, streaming platforms and open-source projects. I forge ideas into things people can open in a browser.</p>
      <div class="age" role="group" aria-label="Current age">
        <small>On Earth since</small>
        <output id="age">--</output>
      </div>
      <div class="bday" role="group" aria-label="Countdown to next birthday">
        <small id="bd-label">Next birthday in</small>
        <div class="units" id="bd-units">
          <div><b id="bd-d">--</b><span>days</span></div>
          <div><b id="bd-h">--</b><span>hours</span></div>
          <div><b id="bd-m">--</b><span>minutes</span></div>
          <div><b id="bd-s">--</b><span>seconds</span></div>
        </div>
      </div>
      <ul class="roles" aria-label="Roles">
        <li>API Developer</li><li>Graphic Poster Designer</li><li>Android App Developer</li>
      </ul>
      <div class="cta">
        <a class="btn primary" href="https://instagram.com/saaptaarshii" target="_blank" rel="noopener"><svg class="ic" viewBox="0 0 24 24" aria-hidden="true" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4.2"/><circle cx="17.3" cy="6.7" r="1" fill="currentColor" stroke="none"/></svg>Instagram</a>
        <a class="btn" href="https://github.com/saptarshiorg" target="_blank" rel="noopener"><svg class="ic" viewBox="0 0 16 16" aria-hidden="true"><path fill="currentColor" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/></svg>GitHub</a>
      </div>
    </div>
  </div>

  <section id="about">
    <div class="wrap two">
      <div>
        <h2>About</h2>
        <p>Hi, I'm Saptarshi, a developer and creator. I make websites, software and digital experiences, from the layout to the last line of code.</p>
        <p>My work centres on the web: fast pages, clean interfaces and tools that feel good to use. I also design posters, build APIs and Android apps, and write in Python, C, C++ and Java.</p>
        <p class="mute">Code. Build. Create. Repeat.</p>
      </div>
      <ul class="facts" aria-label="Quick facts">
        <li><span>Name</span><span>Saptarshi Samanta</span></li>
        <li><span>Brand</span><span>RISHI FORGE</span></li>
        <li><span>Based in</span><span>Kolkata, West Bengal</span></li>
        <li><span>Age</span><span id="age2">--</span></li>
        <li><span>Focus</span><span>Web, APIs, apps, design</span></li>
        <li><span>Email</span><a href="#contact">See contact</a></li>
        <li><span>Instagram</span><a href="https://instagram.com/saaptaarshii" target="_blank" rel="noopener">@saaptaarshii</a></li>
      </ul>
    </div>
  </section>


  <section id="location">
    <div class="wrap two">
      <div>
        <h2>Location</h2>
        <p>I'm based in Kolkata, West Bengal. The nearest airport is Netaji Subhas Chandra Bose International Airport, code CCU, about 13 km north-east of the city centre.</p>
        <p class="mute">The map is a schematic, not to scale for roads.</p>
        <div class="loc-links">
          <a class="btn primary" href="https://www.google.com/maps/search/?api=1&amp;query=Kolkata%2C+West+Bengal" target="_blank" rel="noopener">Kolkata on Maps</a>
          <a class="btn" href="https://www.google.com/maps/search/?api=1&amp;query=22.6547%2C88.4467" target="_blank" rel="noopener">CCU airport on Maps</a>
        </div>
      </div>
      <div class="map">
        <svg viewBox="0 0 520 380" role="img" aria-label="Schematic map: Kolkata city centre and CCU airport, about 13 kilometres apart">
          <g class="grid">
            <path d="M0 95H520M0 190H520M0 285H520M130 0V380M260 0V380M390 0V380"/>
          </g>
          <path class="route" d="M150 285 C 220 240, 300 150, 370 95"/>
          <circle class="ring" cx="150" cy="285" r="14"/>
          <circle class="pt" cx="150" cy="285" r="7"/>
          <text x="166" y="296">Kolkata</text>
          <text class="sub" x="166" y="314">City centre</text>
          <circle class="ring" cx="370" cy="95" r="14" style="animation-delay:1.2s"/>
          <circle class="pt" cx="370" cy="95" r="7"/>
          <text x="294" y="72">CCU airport</text>
          <text class="sub" x="294" y="56">Netaji Subhas Chandra Bose Intl</text>
          <text class="sub" x="236" y="205" transform="rotate(-38 236 205)">about 13 km</text>
          <text class="sub" x="478" y="28">N ↑</text>
        </svg>
      </div>
    </div>
  </section>

  <section id="featured">
    <div class="wrap">
      <h2>Project</h2>
      <div class="feature">
        <h3>EV STREAMS</h3>
        <p class="tag">All global OTT, sports, IPTV and live TV. A free streaming hub.</p>
        <p>One browser-based hub for global OTT, sports and IPTV channels, plus live TV. Football, cricket, basketball, tennis, motorsports and more, free to watch and built to work on any screen size.</p>
        <ul class="chips" aria-label="Features">
          <li>Live TV</li><li>Sports</li><li>Entertainment</li><li>Content discovery</li><li>Responsive</li><li>Modern UI</li>
        </ul>
        <div class="cta" style="margin-top:0">
          <a class="btn primary" href="https://evstreams.pages.dev" target="_blank" rel="noopener">Open EV STREAMS</a>
          <a class="btn" href="https://github.com/saptarshiorg/saptarshiorg.github.io" target="_blank" rel="noopener">View source on GitHub</a>
        </div>
      </div>
    </div>
  </section>


  <section id="stack">
    <div class="wrap">
      <h2>Stack</h2>
      <div class="stack">
        <div><h3>Languages</h3><ul><li>Python</li><li>C and C++</li><li>Java</li></ul></div>
        <div><h3>Web</h3><ul><li>HTML</li><li>CSS</li><li>JavaScript</li><li>Responsive UI</li><li>APIs</li></ul></div>
        <div><h3>Tools</h3><ul><li>Git and GitHub</li><li>GitHub Pages</li><li>Android apps</li></ul></div>
        <div><h3>Design</h3><ul><li>UI and UX</li><li>Branding</li><li>Poster design</li></ul></div>
      </div>
    </div>
  </section>

</main>

<footer id="contact">
  <div class="wrap">
    <h2>Let's build something</h2>
    <a class="mail" id="mail" href="#contact">Email me</a>
    <div class="links">
      <a class="btn primary" href="https://github.com/saptarshiorg" target="_blank" rel="noopener"><svg class="ic" viewBox="0 0 16 16" aria-hidden="true"><path fill="currentColor" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/></svg>GitHub</a>
      <a class="btn" href="https://instagram.com/saaptaarshii" target="_blank" rel="noopener"><svg class="ic" viewBox="0 0 24 24" aria-hidden="true" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4.2"/><circle cx="17.3" cy="6.7" r="1" fill="currentColor" stroke="none"/></svg>Instagram</a>
    </div>
    <p class="fine">© <span id="yr"></span> Saptarshi Samanta. Forge your ideas. Build the future.</p>
  </div>
</footer>

<script>
/* ---- CONFIG: edit these ---- */
var DOB = new Date(2010, 5, 12); /* year, month (0 = Jan), day: 12 June 2010 */
/* ---------------------------- */
var MS_YEAR = 365.2425 * 24 * 3600 * 1000;
function exactAge(now){
  var y = now.getFullYear() - DOB.getFullYear();
  var last = new Date(DOB.getFullYear() + y, DOB.getMonth(), DOB.getDate());
  if (last > now) { y--; last = new Date(DOB.getFullYear() + y, DOB.getMonth(), DOB.getDate()); }
  var next = new Date(DOB.getFullYear() + y + 1, DOB.getMonth(), DOB.getDate());
  return y + (now - last) / (next - last);
}
var out = document.getElementById('age'), out2 = document.getElementById('age2');
var reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
function tick(){
  var a = exactAge(new Date());
  out.textContent = a.toFixed(reduce ? 0 : 9);
  out2.textContent = Math.floor(a) + ' years';
}
tick();
if (!reduce) setInterval(tick, 50);
document.getElementById('yr').textContent = new Date().getFullYear();



/* birthday countdown */
function nextBirthday(now){
  var d = new Date(now.getFullYear(), DOB.getMonth(), DOB.getDate());
  var today = new Date(now.getFullYear(), now.getMonth(), now.getDate());
  if (d < today) d = new Date(now.getFullYear() + 1, DOB.getMonth(), DOB.getDate());
  return d;
}
function pad(n){ return n < 10 ? '0' + n : '' + n; }
function bdTick(){
  var now = new Date(), nb = nextBirthday(now);
  var isToday = now.getMonth() === DOB.getMonth() && now.getDate() === DOB.getDate();
  var turning = nb.getFullYear() - DOB.getFullYear();
  var label = document.getElementById('bd-label');
  if (isToday){
    label.textContent = 'Happy birthday! Turning ' + (now.getFullYear() - DOB.getFullYear()) + ' today';
    ['d','h','m','s'].forEach(function(k){ document.getElementById('bd-' + k).textContent = '00'; });
    return;
  }
  label.textContent = 'Turning ' + turning + ' in';
  var diff = Math.max(0, nb - now), sec = Math.floor(diff / 1000);
  document.getElementById('bd-d').textContent = Math.floor(sec / 86400);
  document.getElementById('bd-h').textContent = pad(Math.floor(sec % 86400 / 3600));
  document.getElementById('bd-m').textContent = pad(Math.floor(sec % 3600 / 60));
  document.getElementById('bd-s').textContent = pad(sec % 60);
}
bdTick(); setInterval(bdTick, 1000);

/* email (assembled at load to avoid scrapers) */
var u = ['saptarshirishi11','gmail.com'], addr = u[0] + '@' + u[1];
var m = document.getElementById('mail');
m.href = 'mailto:' + addr; m.textContent = addr;

/* theme toggle */
var root = document.documentElement, btn = document.getElementById('theme');
btn.addEventListener('click', function(){
  var dark = root.getAttribute('data-theme') === 'dark' ||
    (!root.getAttribute('data-theme') && window.matchMedia('(prefers-color-scheme: dark)').matches);
  root.setAttribute('data-theme', dark ? 'light' : 'dark');
});
</script>
</body>
</html>
