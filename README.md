<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>PROJECT_NAME • Beautiful Repo Website</title>
  <meta name="description" content="A beautiful landing page for the PROJECT_NAME GitHub repository — features, install, usage, and contribution info." />

  <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>🌿</text></svg>">

  <style>
   
    :root{
      --bg: linear-gradient(180deg,#0f172a 0%, #071029 60%);
      --card: rgba(255,255,255,0.04);
      --glass: rgba(255,255,255,0.06);
      --accent: linear-gradient(90deg,#7C3AED,#06B6D4);
      --muted: #97a0b8;
      --glass-border: rgba(255,255,255,0.08);
      --radius: 14px;
      --fw-title: 700;
      --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, "Roboto Mono", "Courier New", monospace;
      color-scheme: dark;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: var(--bg);
      color: #e6eef8;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
      padding:40px 20px;
    }

    
    .container{max-width:1100px;margin:0 auto}
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;gap:14px;align-items:center}
    .logo{width:56px;height:56px;border-radius:12px;display:grid;place-items:center;background:var(--glass);backdrop-filter: blur(8px);border:1px solid var(--glass-border)}
    .logo svg{width:34px;height:34px}
    h1{font-size:28px;margin:0}
    p.lead{color:var(--muted);margin:4px 0 0;font-size:15px}

    nav{display:flex;gap:8px}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:10px 14px;border-radius:10px;background:transparent;border:1px solid transparent;cursor:pointer;text-decoration:none;color:inherit;font-weight:600}
    .btn.primary{background:var(--accent);box-shadow:0 6px 18px rgba(124,58,237,0.14);border:none}
    .btn.ghost{border:1px solid rgba(255,255,255,0.06);background:transparent}

    
    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;margin-top:32px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:var(--radius);padding:28px;border:1px solid var(--glass-border);box-shadow: 0 8px 30px rgba(2,6,23,0.6)}

    .feature-list{display:grid;grid-template-columns:repeat(2, minmax(0,1fr));gap:12px;margin-top:18px}
    .feature{display:flex;gap:12px;align-items:flex-start}
    .feature .icon{width:44px;height:44px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.03), rgba(255,255,255,0.02));display:grid;place-items:center;border:1px solid rgba(255,255,255,0.03)}
    .feature h4{margin:0;font-size:15px}
    .feature p{margin:4px 0 0;color:var(--muted);font-size:13px}

    
    .code{
      margin-top:16px;border-radius:10px;padding:12px;background:linear-gradient(180deg, rgba(6,8,15,0.6), rgba(6,8,15,0.38));font-family:var(--mono);font-size:13px;border:1px solid rgba(255,255,255,0.03);overflow:auto;max-height:300px
    }
    pre{margin:0;white-space:pre-wrap}

    /
    .grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px;margin-top:28px}
    .small-card{padding:18px;border-radius:12px;background:var(--card);border:1px solid var(--glass-border)}
    .small-card h5{margin:0 0 8px}
    .small-card p{margin:0;color:var(--muted);font-size:14px}

    
    footer{margin-top:36px;display:flex;align-items:center;justify-content:space-between;gap:12px}
    .footer-left{color:var(--muted)}

    
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .grid{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:600px){
      body{padding:18px}
      .grid{grid-template-columns:1fr}
      h1{font-size:22px}
      .logo{width:48px;height:48px}
    }

    
    .float{animation:float 6s ease-in-out infinite}
    @keyframes float{0%{transform:translateY(0)}50%{transform:translateY(-6px)}100%{transform:translateY(0)}}

    .glow{background:linear-gradient(90deg, rgba(124,58,237,0.18), rgba(6,182,212,0.12));padding:10px;border-radius:10px}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo float" aria-hidden>
          <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="24" height="24" rx="5" fill="url(#g)" />
            <defs>
              <linearGradient id="g" x1="0" x2="1">
                <stop offset="0" stop-color="#7C3AED" />
                <stop offset="1" stop-color="#06B6D4" />
              </linearGradient>
            </defs>
            <path d="M6 12c1.5-3 6-3 7.5 0 1.5 3-1.5 6-3.75 6S6 15 6 12z" fill="white" opacity="0.94"/>
          </svg>
        </div>
        <div>
          <h1 id="repo-title">PROJECT_NAME</h1>
          <p class="lead">Beautiful, well-documented, and ready to run. A delightful starting point for your next project.</p>
        </div>
      </div>
      <nav>
        <a class="btn ghost" href="#features">Features</a>
        <a class="btn ghost" href="#install">Install</a>
        <a class="btn primary" href="#get-started">Get Started</a>
      </nav>
    </header>
    <main>
      <section class="hero">
        <div class="card">
          <div style="display:flex;align-items:center;justify-content:space-between;gap:12px;">
            <div>
              <h2 style="margin:0;font-size:22px;font-weight:var(--fw-title)">Make your GitHub repo stand out</h2>
              <p style="margin:8px 0 0;color:var(--muted)">A minimal landing page that explains what your project does, why it matters, and how to use it — crafted for maintainers and contributors.</p>
              <div style="margin-top:18px;display:flex;gap:10px;flex-wrap:wrap">
                <a class="btn primary" href="#install">Install</a>
                <a class="btn ghost" href="https://github.com/USERNAME/REPO" target="_blank">View on GitHub</a>
              </div>
            </div>
            <div style="text-align:right;max-width:240px">
              <div class="glow" style="border-radius:12px;">
                <div style="font-family:var(--mono);font-weight:700">v1.0.0</div>
                <div style="font-size:13px;color:var(--muted);margin-top:6px">MIT · JavaScript · 290 lines</div>
              </div>
              <div style="margin-top:14px; font-size:13px;color:var(--muted)">⭐ <strong>120</strong> &nbsp; | &nbsp; Forks: <strong>32</strong></div>
            </div>
          </div>
          <div class="feature-list">
            <div class="feature">
              <div class="icon">⚡</div>
              <div>
                <h4>Fast to set up</h4>
                <p>Clone, install, and run — everything works out of the box with minimal config.</p>
              </div>
            </div>
            <div class="feature">
              <div class="icon">🎨</div>
              <div>
                <h4>Beautiful UI</h4>
                <p>Polished components, clean typography, and a modern color system for a delightful experience.</p>
              </div>
            </div>
            <div class="feature">
              <div class="icon">🔌</div>
              <div>
                <h4>Extensible</h4>
                <p>Well-structured code so you can extend and integrate with CI/CD, docs, and more.</p>
              </div>
            </div>
            <div class="feature">
              <div class="icon">📦</div>
              <div>
                <h4>Ready for production</h4>
                <p>Optimized assets and small footprint — suitable to host as a GitHub Pages site.</p>
              </div>
            </div>
          </div>
          <div class="code" aria-hidden>
<pre><code>git clone https://github.com/USERNAME/REPO.git
cd REPO
# open index.html or serve with a static server
# e.g. npm i -g serve
serve .
</code></pre>
          </div>
        </div>
        <!-- Right column: quick stats / screenshot -->
        <aside>
          <div class="card" style="display:flex;flex-direction:column;gap:14px">
            <div style="display:flex;gap:12px;align-items:center;justify-content:space-between">
              <div>
                <div style="font-size:13px;color:var(--muted)">Maintainer</div>
                <div style="font-weight:700">Your Name</div>
              </div>
              <div style="text-align:right">
                <div style="font-size:13px;color:var(--muted)">License</div>
                <div style="font-weight:700">MIT</div>
              </div>
            </div>
            <div style="border-radius:10px;overflow:hidden;border:1px solid rgba(255,255,255,0.03)">
              <!-- fake screenshot -->
              <div style="height:220px;background:linear-gradient(180deg,#061226,#09233a);display:grid;place-items:center;color:var(--muted);font-family:var(--mono)">
                <div>
                  <div style="font-size:13px;margin-bottom:8px">Live preview</div>
                  <div style="font-size:12px;color:var(--muted)">Drop your README or screenshot here</div>
                </div>
              </div>
            </div>
            <div style="display:flex;gap:8px;justify-content:center">
              <a class="btn ghost" href="#contribute">Contribute</a>
              <a class="btn primary" href="#get-started">Download</a>
            </div>
          </div>
        </aside>
      </section>
      <!-- Features grid -->
      <section id="features" class="grid" aria-label="features">
        <div class="small-card card">
          <h5>Clear docs</h5>
          <p>Step-by-step guides and an example app to help new contributors get started quickly.</p>
        </div>
        <div class="small-card card">
          <h5>Themeable</h5>
          <p>Tweak colors, fonts, and spacing using CSS variables — use dark or light modes as needed.</p>
        </div>
        <div class="small-card card">
          <h5>CI Ready</h5>
          <p>Sample GitHub Actions are included so you can publish and test automatically on push.</p>
        </div>
      </section>
      <!-- Install / Usage -->
      <section id="install" style="margin-top:26px">
        <div class="card">
          <h3 style="margin-top:0">Install & run</h3>
          <p style="color:var(--muted)">Quick guide to get the site running locally or deployed to GitHub Pages.</p>
          <div style="display:flex;gap:18px;flex-wrap:wrap;margin-top:18px">
            <div style="flex:1;min-width:240px">
              <h4 style="margin:0 0 8px">Local</h4>
              <pre class="code"><code>npm install
npm run build
npm run start</code></pre>
            </div>
            <div style="flex:1;min-width:240px">
              <h4 style="margin:0 0 8px">Deploy</h4>
              <pre class="code"><code># push to main
git push origin main
# enable GitHub Pages on the repo settings</code></pre>
            </div>
          </div>
          <div style="margin-top:14px;display:flex;gap:10px">
            <a class="btn primary" id="get-started" href="#">Get started</a>
            <a class="btn ghost" href="#contribute">Contribute</a>
          </div>
        </div>
      </section>
      <!-- Contributing -->
      <section id="contribute" style="margin-top:24px">
        <div class="card">
          <h3 style="margin-top:0">Contributing</h3>
          <p style="color:var(--muted)">We welcome contributions — whether it's reporting issues, improving docs, or adding features.</p>
          <ol style="color:var(--muted);margin-top:12px">
            <li>Fork the repository</li>
            <li>Create a feature branch (<code>git checkout -b feature/your-idea</code>)</li>
            <li>Open a pull request with a clear description</li>
          </ol>
          <div style="margin-top:12px;font-size:13px;color:var(--muted)">Prefer to follow a code of conduct? Add a <code>CODE_OF_CONDUCT.md</code> to your repo and link it here.</div>
        </div>
      </section>
    </main>
    <footer>
      <div class="footer-left">© <span id="year"></span> PROJECT_NAME • Built with ❤️</div>
      <div>
        <a class="btn ghost" href="#">License</a>
        <a class="btn ghost" href="#">Changelog</a>
      </div>
    </footer>
  </div>

  <script>
    // small runtime helpers to make it feel alive
    document.getElementById('year').textContent = new Date().getFullYear();
    // Replace placeholders: PROJECT_NAME, USERNAME, REPO
    const REPO = { name: 'PROJECT_NAME', repo: 'REPO', user: 'USERNAME' };
    document.getElementById('repo-title').textContent = REPO.name;

    // Optional: add copy-to-clipboard for install snippet
    // (left simple to avoid external libs)
  </script>
</body>
</html>
