<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mohamed Khalel — React Front-End Developer</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@latest/tabler-icons.min.css">
<style>
  *{box-sizing:border-box;margin:0;padding:0}
  :root{
    --color-text-primary:#111;
    --color-text-secondary:#555;
    --color-text-tertiary:#888;
    --color-text-info:#185FA5;
    --color-background-primary:#fff;
    --color-background-secondary:#f5f5f3;
    --color-border-tertiary:rgba(0,0,0,0.12);
    --color-border-secondary:rgba(0,0,0,0.22);
    --border-radius-md:8px;
    --border-radius-lg:12px;
    --font-sans:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;
  }
  @media(prefers-color-scheme:dark){
    :root{
      --color-text-primary:#f0f0f0;
      --color-text-secondary:#aaa;
      --color-text-tertiary:#666;
      --color-text-info:#85B7EB;
      --color-background-primary:#1a1a1a;
      --color-background-secondary:#222;
      --color-border-tertiary:rgba(255,255,255,0.1);
      --color-border-secondary:rgba(255,255,255,0.2);
    }
    .avatar{background:#0C447C!important;border-color:#378ADD!important;color:#B5D4F4!important}
    .tag.blue{background:#0C447C!important;color:#B5D4F4!important;border-color:#378ADD!important}
    .tag.teal{background:#085041!important;color:#9FE1CB!important;border-color:#1D9E75!important}
    .tag.purple{background:#3C3489!important;color:#CECBF6!important;border-color:#7F77DD!important}
    .tag.green{background:#27500A!important;color:#C0DD97!important;border-color:#639922!important}
    .tag.amber{background:#412402!important;color:#FAC775!important;border-color:#EF9F27!important}
  }
  body{
    font-family:var(--font-sans);
    background:var(--color-background-primary);
    color:var(--color-text-primary);
    padding:2.5rem 1.5rem;
    max-width:760px;
    margin:0 auto;
    line-height:1.6;
  }
  .avatar{
    width:60px;height:60px;border-radius:50%;
    background:#E6F1FB;border:0.5px solid #85B7EB;
    display:flex;align-items:center;justify-content:center;
    font-size:20px;font-weight:500;color:#0C447C;flex-shrink:0;
  }
  .tag{
    display:inline-flex;align-items:center;gap:5px;
    font-size:11px;font-weight:500;
    padding:3px 10px;border-radius:99px;
    border:0.5px solid var(--color-border-secondary);
    color:var(--color-text-secondary);
    background:var(--color-background-secondary);
    text-decoration:none;
  }
  .tag.blue{background:#E6F1FB;color:#0C447C;border-color:#85B7EB}
  .tag.teal{background:#E1F5EE;color:#085041;border-color:#5DCAA5}
  .tag.purple{background:#EEEDFE;color:#3C3489;border-color:#AFA9EC}
  .tag.green{background:#EAF3DE;color:#27500A;border-color:#97C459}
  .tag.amber{background:#FAEEDA;color:#633806;border-color:#EF9F27}
  .section-label{
    font-size:11px;font-weight:500;
    color:var(--color-text-tertiary);
    text-transform:uppercase;letter-spacing:0.8px;
    margin-bottom:12px;
  }
  .card{
    background:var(--color-background-primary);
    border:0.5px solid var(--color-border-tertiary);
    border-radius:var(--border-radius-lg);
    padding:16px 18px;
  }
  .link-row{display:flex;gap:16px;flex-wrap:wrap;margin-top:12px}
  .link-row a{
    font-size:13px;color:var(--color-text-info);
    text-decoration:none;display:flex;align-items:center;gap:5px;
  }
  .link-row a:hover{text-decoration:underline}
  .skill-row{display:flex;flex-wrap:wrap;gap:6px}
  .proj-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:10px}
  .proj-card{
    background:var(--color-background-primary);
    border:0.5px solid var(--color-border-tertiary);
    border-radius:var(--border-radius-lg);
    padding:14px 16px;
    display:flex;flex-direction:column;gap:6px;
  }
  .proj-card:hover{border-color:var(--color-border-secondary)}
  .proj-title{font-size:14px;font-weight:500;color:var(--color-text-primary);display:flex;align-items:center;gap:6px}
  .proj-desc{font-size:12px;color:var(--color-text-secondary);line-height:1.6}
  .ext-link{font-size:11px;color:var(--color-text-tertiary);text-decoration:none;margin-left:auto}
  .ext-link:hover{color:var(--color-text-info)}
  .stat-img{width:100%;border-radius:8px;display:block}
  .divider{border:none;border-top:0.5px solid var(--color-border-tertiary)}
  .exp-row{display:flex;flex-direction:column;gap:4px}
  .exp-title{font-size:14px;font-weight:500;color:var(--color-text-primary)}
  .exp-desc{font-size:13px;color:var(--color-text-secondary);line-height:1.6;margin-top:4px}
  .src-link{font-size:12px;color:var(--color-text-tertiary);text-decoration:none;display:flex;align-items:center;gap:4px;margin-top:4px}
  .src-link:hover{color:var(--color-text-info)}
  section{display:flex;flex-direction:column;gap:2.2rem}
</style>
</head>
<body>
<section>

  <!-- Header -->
  <div style="display:flex;align-items:flex-start;gap:18px">
    <div class="avatar">MK</div>
    <div style="flex:1">
      <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap;margin-bottom:6px">
        <span style="font-size:20px;font-weight:500">Mohamed Khalel</span>
        <span class="tag blue">React Developer</span>
        <span class="tag green">Open to work</span>
      </div>
      <p style="font-size:14px;color:var(--color-text-secondary);line-height:1.7;max-width:540px">
        Building React applications that handle real data, real users, and real edge cases.
        Currently interning at <strong style="color:var(--color-text-primary);font-weight:500">CASCOTEC</strong>
        and finishing the React track at <strong style="color:var(--color-text-primary);font-weight:500">DEPI</strong>.
      </p>
      <div class="link-row">
        <a href="https://www.linkedin.com/in/mohamed-khalel1" target="_blank" rel="noopener">
          <i class="ti ti-brand-linkedin" style="font-size:15px" aria-hidden="true"></i> LinkedIn
        </a>
        <a href="https://clever-mermaid-3734dd.netlify.app/" target="_blank" rel="noopener">
          <i class="ti ti-world" style="font-size:15px" aria-hidden="true"></i> Portfolio
        </a>
        <a href="mailto:mohamedkhalel852@gmail.com">
          <i class="ti ti-mail" style="font-size:15px" aria-hidden="true"></i> mohamedkhalel852@gmail.com
        </a>
        <a href="https://github.com/medokalel" target="_blank" rel="noopener">
          <i class="ti ti-brand-github" style="font-size:15px" aria-hidden="true"></i> medokalel
        </a>
        <span style="font-size:13px;color:var(--color-text-tertiary);display:flex;align-items:center;gap:5px">
          <i class="ti ti-map-pin" style="font-size:15px" aria-hidden="true"></i> Egypt
        </span>
      </div>
    </div>
  </div>

  <hr class="divider">

  <!-- About -->
  <div>
    <p class="section-label">About</p>
    <p style="font-size:14px;color:var(--color-text-secondary);line-height:1.8;max-width:600px">
      I build React applications — the kind that handle real data, real users, and real edge cases.
      Right now I'm interning at CASCOTEC converting Figma designs into responsive layouts and building
      an internal icon library. Alongside that, I'm finishing my React track at DEPI where I worked
      through JWT authentication, API integration, and state management across complex component trees.
    </p>
  </div>

  <hr class="divider">

  <!-- Tech Stack -->
  <div>
    <p class="section-label">Tech stack</p>
    <div class="skill-row">
      <span class="tag blue"><i class="ti ti-brand-react" style="font-size:12px" aria-hidden="true"></i> React</span>
      <span class="tag blue"><i class="ti ti-brand-typescript" style="font-size:12px" aria-hidden="true"></i> TypeScript</span>
      <span class="tag blue">JavaScript ES6+</span>
      <span class="tag purple">React Query</span>
      <span class="tag purple">Context API</span>
      <span class="tag purple">React Router</span>
      <span class="tag teal">REST APIs · Axios</span>
      <span class="tag teal">Formik + Yup</span>
      <span class="tag">HTML5 · CSS3</span>
      <span class="tag">Bootstrap</span>
      <span class="tag"><i class="ti ti-brand-figma" style="font-size:12px" aria-hidden="true"></i> Figma</span>
      <span class="tag"><i class="ti ti-brand-git" style="font-size:12px" aria-hidden="true"></i> Git · GitHub</span>
    </div>
  </div>

  <hr class="divider">

  <!-- Experience -->
  <div>
    <p class="section-label">Experience</p>
    <div style="display:flex;flex-direction:column;gap:18px">
      <div class="exp-row">
        <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap">
          <span class="exp-title">Front-End Development Intern</span>
          <span class="tag blue">CASCOTEC</span>
          <span style="font-size:12px;color:var(--color-text-tertiary);margin-left:auto">Jan 2026 – Present</span>
        </div>
        <p class="exp-desc">Building an internal icon library in Figma, converting desktop designs to responsive mobile layouts, and taking ownership of front-end implementation on a live project.</p>
      </div>
      <div style="height:0.5px;background:var(--color-border-tertiary)"></div>
      <div class="exp-row">
        <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap">
          <span class="exp-title">Front-End React Track Trainee</span>
          <span class="tag purple">DEPI</span>
          <span style="font-size:12px;color:var(--color-text-tertiary);margin-left:auto">Oct 2025 – Present</span>
        </div>
        <p class="exp-desc">Built real-world React apps with JWT auth, REST API integration, cart management, protected routes, and state management via Context API.</p>
      </div>
    </div>
  </div>

  <hr class="divider">

  <!-- Projects -->
  <div>
    <p class="section-label">Projects</p>
    <div class="proj-grid">

      <div class="proj-card">
        <div style="display:flex;align-items:center">
          <span class="proj-title">
            <i class="ti ti-shopping-cart" style="font-size:15px;color:#378ADD" aria-hidden="true"></i>
            E-Commerce App
          </span>
          <a href="https://jolly-crisp-1b2e2d.netlify.app/" class="ext-link" target="_blank" rel="noopener" aria-label="Live demo">
            <i class="ti ti-external-link" style="font-size:14px"></i>
          </a>
        </div>
        <p class="proj-desc">JWT auth, Stripe payments, React Query caching, protected routes, cart management.</p>
        <div class="skill-row" style="margin-top:4px">
          <span class="tag blue">React</span>
          <span class="tag purple">React Query</span>
          <span class="tag">Stripe</span>
          <span class="tag">Formik</span>
        </div>
        <a href="https://github.com/medokalel/react-ecommerce-app" target="_blank" rel="noopener" class="src-link">
          <i class="ti ti-brand-github" style="font-size:13px" aria-hidden="true"></i> Source
        </a>
      </div>

      <div class="proj-card">
        <div style="display:flex;align-items:center">
          <span class="proj-title">
            <i class="ti ti-cloud" style="font-size:15px;color:#1D9E75" aria-hidden="true"></i>
            Weather Forecast
          </span>
          <a href="https://medokalel.github.io/weather-forecast-app/" class="ext-link" target="_blank" rel="noopener" aria-label="Live demo">
            <i class="ti ti-external-link" style="font-size:14px"></i>
          </a>
        </div>
        <p class="proj-desc">Real-time weather data, auto geolocation, 3-day forecast, edge case handling.</p>
        <div class="skill-row" style="margin-top:4px">
          <span class="tag blue">React</span>
          <span class="tag teal">WeatherAPI</span>
          <span class="tag">Geolocation</span>
        </div>
        <a href="https://github.com/medokalel/weather-forecast-app" target="_blank" rel="noopener" class="src-link">
          <i class="ti ti-brand-github" style="font-size:13px" aria-hidden="true"></i> Source
        </a>
      </div>

      <div class="proj-card">
        <div style="display:flex;align-items:center">
          <span class="proj-title">
            <i class="ti ti-layout" style="font-size:15px;color:#7F77DD" aria-hidden="true"></i>
            DevFolio
          </span>
          <a href="https://medokalel.github.io/devfolio-portfolio/" class="ext-link" target="_blank" rel="noopener" aria-label="Live demo">
            <i class="ti ti-external-link" style="font-size:14px"></i>
          </a>
        </div>
        <p class="proj-desc">Responsive portfolio, typing animation, smooth scrolling, SwiperJS sliders.</p>
        <div class="skill-row" style="margin-top:4px">
          <span class="tag">HTML5</span>
          <span class="tag">CSS3</span>
          <span class="tag">Bootstrap 5</span>
        </div>
        <a href="https://github.com/medokalel/devfolio-portfolio" target="_blank" rel="noopener" class="src-link">
          <i class="ti ti-brand-github" style="font-size:13px" aria-hidden="true"></i> Source
        </a>
      </div>

    </div>
  </div>

  <hr class="divider">

  <!-- Stats -->
  <div>
    <p class="section-label">GitHub stats</p>
    <div style="display:flex;flex-direction:column;gap:10px">
      <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:10px">
        <img src="https://github-readme-stats.vercel.app/api?username=medokalel&show_icons=true&theme=tokyonight&hide_border=true&hide_title=true" class="stat-img" alt="GitHub stats">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=medokalel&theme=tokyonight&hide_border=true" class="stat-img" alt="GitHub streak">
      </div>
      <img src="https://github-readme-activity-graph.vercel.app/graph?username=medokalel&theme=tokyo-night&hide_border=true" class="stat-img" alt="Activity graph">
      <div style="text-align:center;margin-top:4px">
        <img src="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake.svg" style="max-width:100%" alt="Contribution snake">
      </div>
    </div>
  </div>

  <hr class="divider">

  <!-- Footer -->
  <div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:10px;padding-bottom:1rem">
    <div>
      <p style="font-size:13px;font-weight:500;color:var(--color-text-primary)">Mohamed Khalel</p>
      <p style="font-size:12px;color:var(--color-text-tertiary)">Communications &amp; Computer Engineering · Tanta · Expected 2028</p>
    </div>
    <div style="display:flex;gap:8px;flex-wrap:wrap">
      <a href="https://mostaql.com/u/mohamedkhalel3" target="_blank" rel="noopener" class="tag teal">Mostaql</a>
      <a href="https://khamsat.com/user/mohamedkhalel2" target="_blank" rel="noopener" class="tag amber">Khamsat</a>
    </div>
  </div>

</section>
</body>
</html>
