<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>m2hcs — Offensive Security</title>

    <meta name="title" content="m2hcs" />
    <meta name="description" content="Senior Offensive Security Engineer — APT Emulation, Exploit Research, Red Team, Cloud & DevSecOps." />

    <meta property="og:type" content="website" />
    <meta property="og:title" content="m2hcs — Offensive Security" />
    <meta property="og:description" content="Senior Offensive Security Engineer — APT Emulation, Exploit Research, Red Team, Cloud & DevSecOps." />
    <meta name="twitter:card" content="summary_large_image" />
    <meta property="twitter:title" content="m2hcs — Offensive Security" />
    <meta property="twitter:description" content="Senior Offensive Security Engineer — APT Emulation, Exploit Research, Red Team, Cloud & DevSecOps." />
    <meta name="theme-color" content="#000000" />

    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=Afacad+Flux:wght@400;600;800&display=swap" rel="stylesheet" />

    <style>
      :root {
        --bg: #000000;
        --surface: #0a0a0a;
        --text: #f3f4f6;
        --muted: #a0a7b4;
        --chip: #0f0f10;
        --link: #e5e7eb;
        --line: #1a1a1a;
        --ring: rgba(255,255,255,0.15);
      }
      * { box-sizing: border-box; }
      html, body { height: 100%; }
      html { scroll-behavior: smooth; }
      body {
        margin: 0;
        font-family: "Afacad Flux", system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, "Helvetica Neue", Arial, "Noto Sans";
        color: var(--text);
        background: var(--bg);
        letter-spacing: .2px;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        overflow-x: hidden;
      }

      .container { width: min(1100px, 92vw); margin: 0 auto; padding: 48px 0 80px; position: relative; z-index: 1; }

      header {
        display: flex; align-items: center; justify-content: space-between; gap: 16px; padding: 14px 18px; border-radius: 16px;
        background: var(--surface);
        box-shadow: 0 0 0 1px var(--line), 0 8px 28px rgba(0,0,0,0.5);
        position: sticky; top: 12px; z-index: 10;
      }
      .brand { display: flex; align-items: center; gap: 12px; text-decoration: none; color: inherit; }
      .avatar-ring { width: 44px; height: 44px; border-radius: 999px; padding: 2px; background: #000000; box-shadow: 0 0 0 1px var(--line) inset; }
      .avatar-ring img { width: 100%; height: 100%; border-radius: 999px; display: block; border: 1px solid var(--line); background:#000000; }
      .brand b { font-weight: 800; letter-spacing: 0.3px; }
      nav a { text-decoration: none; color: var(--link); margin-left: 16px; font-weight: 600; opacity: .9; }
      nav a:hover { opacity: 1; }

      .hero { display: grid; grid-template-columns: 200px 1fr; gap: 28px; align-items: center; padding: 36px; margin-top: 28px; border-radius: 20px; background: #000000; box-shadow: 0 0 0 1px var(--line), 0 24px 70px rgba(0,0,0,0.6); }
      .hero .pfp-wrap { position: relative; width: 200px; aspect-ratio: 1/1; border-radius: 24px; padding: 10px; background: #000000; box-shadow: 0 0 0 1px var(--line) inset; }
      .hero .pfp { position: relative; border-radius: 18px; overflow: hidden; width: 100%; height: 100%; box-shadow: 0 12px 36px rgba(0,0,0,0.6); background:#000000; }
      .hero .pfp img { width: 100%; height: 100%; object-fit: cover; display: block; background:#000000; }

      .eyebrow { font-weight: 800; letter-spacing: .3px; text-transform: uppercase; font-size: 13px; color: var(--muted); }
      .hero h1 { font-size: clamp(28px, 4.2vw, 48px); margin: 6px 0 8px; }
      .hero p { margin: 0 0 18px; color: var(--muted); font-size: 18px; }

      .actions { display: flex; gap: 12px; flex-wrap: wrap; }
      .btn { appearance: none; border: 1px solid var(--line); padding: 11px 16px; border-radius: 12px; font-weight: 700; cursor: pointer; text-decoration: none; color: var(--text); background: #101010; box-shadow: 0 6px 18px rgba(0,0,0,0.5); transition: transform .12s ease, box-shadow .2s ease, background .2s ease; }
      .btn:hover { transform: translateY(-1px); background: #141414; }
      .btn:focus-visible { outline: 2px solid var(--ring); outline-offset: 2px; }
      .btn-ghost { background: transparent; color: var(--link); border-style: dashed; }

      .section { margin-top: 42px; background: var(--surface); border-radius: 18px; padding: 28px; box-shadow: 0 0 0 1px var(--line), 0 12px 38px rgba(0,0,0,0.55); scroll-margin-top: 96px; }
      .section h2 { margin: 0 0 12px; font-size: 22px; }
      .section p { margin: 0; color: var(--muted); }

      .list { margin: 10px 0 0; padding: 0; list-style: none; color: var(--muted); }
      .list li { padding: 8px 0; border-bottom: 1px dashed var(--line); }
      .list li:last-child { border-bottom: 0; }

      .two-col { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 18px; }
      .card { background: #0b0b0b; border-radius: 16px; padding: 18px; box-shadow: 0 0 0 1px var(--line), 0 10px 30px rgba(0,0,0,0.55); }
      .card h3 { margin: 0 0 8px; }
      .badges { display: flex; gap: 10px; flex-wrap: wrap; }
      .badge { padding: 8px 12px; border-radius: 999px; font-weight: 700; color: var(--text); background: #101010; border: 1px solid var(--line); box-shadow: 0 8px 20px rgba(0,0,0,0.5); }

      .contacts { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 14px; margin-top: 14px; }
      .contact { display: flex; align-items: center; gap: 12px; padding: 12px 14px; border-radius: 12px; text-decoration: none; color: var(--text); background: #0b0b0b; box-shadow: 0 0 0 1px var(--line), 0 8px 18px rgba(0,0,0,0.5); }
      .contact span { color: var(--muted); }
      .contact:hover { transform: translateY(-1px); }

      .analytics { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px; margin-top: 12px; }
      .analytics img { width: 100%; height: auto; border-radius: 14px; box-shadow: 0 0 0 1px var(--line), 0 8px 24px rgba(0,0,0,0.6); }

      blockquote { margin: 22px 0 0; padding: 14px 18px; border-left: 4px solid var(--line); background: #0b0b0b; border-radius: 12px; color: var(--muted); box-shadow: 0 0 0 1px var(--line); }

      footer { margin: 46px 0 0; padding: 18px; color: var(--muted); text-align: center; font-size: 14px; }

      a { color: var(--link); }
      a:hover { filter: brightness(1.05); }
      img { max-width: 100%; display: block; }

      @media (max-width: 860px) {
        .hero { grid-template-columns: 1fr; padding: 24px; }
        .hero .pfp-wrap { width: 180px; justify-self: center; }
        .actions { justify-content: center; }
        .two-col { grid-template-columns: 1fr; }
      }
      @media (prefers-reduced-motion: reduce) {
        .btn, .contact { transition: none; }
      }
    </style>
  </head>
  <body>
    <div class="container">
      <header>
        <a class="brand" href="#top">
          <span class="avatar-ring"><img src="/assets/img/avatar.png" alt="Avatar" loading="lazy" /></span>
          <b>m2hcs</b>
        </a>
        <nav>
          <a href="#about">About</a>
          <a href="#focus">Focus</a>
          <a href="#arsenal">Arsenal</a>
          <a href="#analytics">Analytics</a>
          <a href="#connect">Connect</a>
        </nav>
      </header>

      <section class="hero" id="top">
        <div class="pfp-wrap">
          <div class="pfp">
            <img src="/assets/img/avatar.png" alt="Profile picture" />
          </div>
        </div>
        <div>
          <div class="eyebrow">Senior Offensive Security Engineer</div>
          <h1>m2hcs</h1>
          <p><em>APT Emulation & Exploit Research</em></p>
          <div class="actions">
            <a class="btn" href="#connect" aria-label="Contact">Contact</a>
            <a class="btn" href="#about" aria-label="About">About</a>
            <a class="btn btn-ghost" href="#arsenal" aria-label="Arsenal">Arsenal</a>
          </div>
        </div>
      </section>

      <section class="section" id="about">
        <h2>About Me</h2>
        <p>Offensive Security Engineer with <strong>8+ years</strong> of experience in APT emulation, zero-day research, and custom exploit development. Driven to turn curiosity into code and complexity into clarity.</p>
      </section>

      <section class="section" id="focus">
        <h2>Current Focus</h2>
        <ul class="list">
          <li>Advanced Persistent Threat (APT) Emulation</li>
          <li>Zero-day Vulnerability Research & Custom Exploits</li>
          <li>Red Team Operations & TIBER-EU Assessments</li>
          <li>Security Tool Development (Python, Rust, Go)</li>
          <li>Cloud Security & DevSecOps (AWS, Azure, Kubernetes)</li>
        </ul>
      </section>

      <section class="section" id="arsenal">
        <h2>Arsenal & Tech Stack</h2>
        <div class="two-col">
          <div class="card">
            <h3>Languages</h3>
            <div class="badges">
              <span class="badge">Python</span>
              <span class="badge">Rust</span>
              <span class="badge">C</span>
              <span class="badge">C++</span>
            </div>
            <h3 style="margin-top:14px;">Security Tools</h3>
            <ul class="list">
              <li>Web: Burp Suite Pro, OWASP ZAP, Custom Tools</li>
              <li>Network: Nmap, Masscan, Nuclei, ffuf</li>
              <li>Reversing: Ghidra, IDA Pro, x64dbg, Binary Ninja</li>
              <li>Exploitation: Metasploit, Cobalt Strike, Custom Frameworks</li>
            </ul>
          </div>
          <div class="card">
            <h3>Cloud & Infrastructure</h3>
            <div style="margin:8px 0 10px;">
              <img src="https://skillicons.dev/icons?i=aws,docker,kubernetes,terraform,ansible,linux&theme=dark" alt="Cloud & Infra" loading="lazy"/>
            </div>
            <h3 style="margin-top:6px;">DevSecOps & Automation</h3>
            <ul class="list">
              <li>CI/CD: GitHub Actions, GitLab CI, Jenkins</li>
              <li>Containers: Docker, Kubernetes Security</li>
              <li>IaC: Terraform, CloudFormation, Pulumi</li>
              <li>Monitoring: ELK Stack, Splunk, Prometheus</li>
            </ul>
          </div>
        </div>
      </section>

      <section class="section" id="analytics">
        <h2>GitHub Analytics</h2>
        <div class="analytics">
          <img src="https://github-readme-stats.vercel.app/api?username=m2hcz&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&border_color=0a0a0a" alt="GitHub stats"/>
          <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=m2hcz&layout=compact&theme=tokyonight&border_color=0a0a0a" alt="Top languages"/>
          <img src="https://github-readme-streak-stats.herokuapp.com/?user=m2hcz&theme=tokyonight&border=0a0a0a" alt="Contrib streak"/>
        </div>
      </section>

      <section class="section" id="connect">
        <h2>Let’s Connect</h2>
        <div class="contacts">
          <a class="contact" href="https://x.com/inf0secc" target="_blank" rel="noopener">
            <strong>X (Twitter)</strong><span>@inf0secc</span>
          </a>
          <a class="contact" href="https://github.com/m2hcz" target="_blank" rel="noopener">
            <strong>GitHub</strong><span>m2hcz</span>
          </a>
          <a class="contact" href="mailto:m2hczs@proton.me">
            <strong>ProtonMail</strong><span>m2hczs@proton.me</span>
          </a>
        </div>
        <blockquote>
          <em>“The best defense is a good offense.”</em><br/>
          <em>Open to collaborations, conference talks & advanced security discussions.</em>
        </blockquote>
      </section>

      <footer>
        © <span id="year"></span> m2hcs • All rights reserved
      </footer>
    </div>

    <script>
      document.getElementById('year').textContent = new Date().getFullYear();

      function scrollToTarget(hash) {
        var el = document.querySelector(hash);
        if (!el) return;
        var header = document.querySelector('header');
        var offset = (header ? header.offsetHeight : 0) + 16;
        var y = el.getBoundingClientRect().top + window.pageYOffset - offset;
        window.scrollTo({ top: y, behavior: 'smooth' });
      }

      document.addEventListener('click', function (e) {
        var a = e.target.closest('a[href^="#"]');
        if (!a) return;
        e.preventDefault();
        scrollToTarget(a.getAttribute('href'));
      }, { passive: false });
    </script>
  </body>
</html>
