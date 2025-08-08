<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Raphael Pires — Portfólio</title>
  <meta name="description" content="Portfólio de Raphael Pires — Desenvolvedor e futuro Cientista de Dados para Negócios." />

  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

  <style>
    /* ===== Reset & Variables ===== */
    :root{
      --bg:#0b0b0f; --card:#0f1720; --muted:#9aa0a6; --accent:#4CAF50; --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
    }
    [data-theme="light"]{ --bg:#f3f4f6; --card:#ffffff; --muted:#555; --accent:#0077b6; --glass: rgba(0,0,0,0.04); --glass-2: rgba(0,0,0,0.02);}    

    *{box-sizing:border-box;margin:0;padding:0}
    html,body{height:100%}
    body{
      font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;
      background:linear-gradient(180deg,var(--bg), #07101a); color:var(--muted); -webkit-font-smoothing:antialiased;
      padding-bottom:48px;
    }

    /* ===== Layout ===== */
    .container{max-width:1100px;margin:32px auto;padding:24px}
    header{display:flex;gap:16px;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:12px;align-items:center}
    .brand h1{color:var(--accent);font-size:20px}
    nav ul{display:flex;gap:14px;list-style:none}
    nav a{color:var(--muted);text-decoration:none;padding:8px;border-radius:8px}
    nav a:hover{background:var(--glass);color:inherit}

    .theme-btn{background:transparent;border:1px solid var(--glass);padding:8px;border-radius:10px;cursor:pointer;color:var(--muted)}

    /* ===== Hero ===== */
    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:center;margin-top:28px}
    .card{background:linear-gradient(180deg,var(--card), rgba(0,0,0,0.04));border-radius:14px;padding:20px;border:1px solid var(--glass-2)}
    .intro h2{color:var(--accent);font-size:28px;margin-bottom:6px}
    .intro p{color:var(--muted);margin-bottom:12px}
    .badges{display:flex;gap:8px;flex-wrap:wrap;margin:12px 0}
    .badge{background:rgba(255,255,255,0.04);padding:6px 10px;border-radius:999px;font-size:13px;color:var(--muted)}

    .socials a{margin-right:8px;color:var(--muted);font-size:20px}
    .socials a:hover{color:var(--accent)}

    .hero-image img{width:100%;border-radius:10px}

    /* ===== Sections ===== */
    section{margin-top:20px}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .project{padding:14px;border-radius:12px;background:var(--card);border:1px solid var(--glass-2)}
    .project h3{color:var(--accent);margin-bottom:8px}
    .skills ul{list-style:none;display:flex;flex-wrap:wrap;gap:8px}
    .skill{background:var(--glass);padding:8px 10px;border-radius:8px}

    /* Contact */
    .contact .links a{display:inline-block;margin-right:12px;padding:8px 12px;border-radius:10px;background:var(--glass);text-decoration:none;color:var(--muted)}

    footer{margin-top:28px;text-align:center;color:var(--muted);font-size:14px}

    /* Responsive */
    @media (max-width:1000px){.hero{grid-template-columns:1fr 320px}}
    @media (max-width:820px){
      .hero{grid-template-columns:1fr;}
      .grid{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:520px){
      nav ul{display:none}
      .grid{grid-template-columns:1fr}
      .brand h1{font-size:16px}
    }

    /* Small helpers */
    .muted{color:var(--muted)}
    .btn{display:inline-block;padding:10px 14px;border-radius:10px;background:var(--accent);color:white;text-decoration:none}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <img src="https://capsule-render.vercel.app/api?type=waving&height=48&color=4CAF50" alt="wave" style="height:48px;border-radius:8px">
        <div>
          <h1>Raphael Pires</h1>
          <div style="font-size:12px;color:var(--muted)">Desenvolvedor · Futuro Cientista de Dados para Negócios</div>
        </div>
      </div>

      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#projetos">Projetos</a></li>
          <li><a href="#sobre">Sobre</a></li>
          <li><a href="#contato">Contato</a></li>
        </ul>
      </nav>

      <div style="display:flex;gap:8px;align-items:center">
        <button class="theme-btn" id="themeToggle" title="Alternar tema"><i class="fa fa-moon"></i></button>
        <a class="btn" href="https://github.com/raphaelpireshp" target="_blank">Ver GitHub</a>
      </div>
    </header>

    <!-- HERO -->
    <main id="home" class="hero">
      <div class="card intro">
        <h2>Olá — eu sou o Raphael 👋</h2>
        <p>Desenvolvedor em evolução, apaixonado por tecnologia, programação e soluções criativas. Foco: <strong>Ciência de Dados para Negócios</strong>.</p>

        <div class="badges">
          <span class="badge">Python</span>
          <span class="badge">HTML</span>
          <span class="badge">CSS</span>
          <span class="badge">JavaScript</span>
          <span class="badge">Node.js</span>
          <span class="badge">MySQL</span>
        </div>

        <div style="margin-top:10px">
          <a class="btn" href="#projetos">Ver projetos</a>
        </div>

        <div style="margin-top:14px">
          <div class="socials">
            <a href="https://github.com/raphaelpireshp" target="_blank" aria-label="GitHub"><i class="fab fa-github"></i></a>
            <a href="https://www.linkedin.com/in/raphaelpireshp" target="_blank" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
            <a href="mailto:raphaelpireshp@gmail.com" aria-label="Email"><i class="fa fa-envelope"></i></a>
          </div>
        </div>

        <div style="margin-top:16px;color:var(--muted);font-size:14px">
          <strong>Sobre:</strong>
          <p class="muted">Estudo Desenvolvimento de Sistemas e quero me especializar em Ciência de Dados para Negócios. Curto projetos práticos, mapas, APIs e automação.</p>
        </div>
      </div>

      <div class="card hero-image">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=raphaelpireshp&layout=compact&theme=transparent" alt="GitHub stats" style="margin-bottom:10px">
        <img src="https://github-readme-stats.vercel.app/api?username=raphaelpireshp&show_icons=true&theme=transparent&hide=contribs,prs" alt="More stats">
      </div>
    </main>

    <!-- PROJECTS -->
    <section id="projetos">
      <h2 style="color:var(--accent);margin-bottom:12px">Projetos</h2>
      <div class="grid">
        <article class="project">
          <h3>OilSmart (mapas & oficina)</h3>
          <p class="muted">Mapa interativo com integração MySQL, busca de oficinas e agendamento. Tecnologias: Leaflet, Node.js, MySQL.</p>
          <div style="margin-top:10px"><a class="btn" href="#contato">Quero esse projeto</a></div>
        </article>

        <article class="project">
          <h3>Mini Blog (localStorage)</h3>
          <p class="muted">Blog em JavaScript que salva posts e comentários no localStorage — ótimo para protótipos rápidos.</p>
        </article>

        <article class="project">
          <h3>Sistema de Login (Node + MySQL)</h3>
          <p class="muted">Login local + OAuth (Google/Facebook) com MySQL. Função: autenticação e seleção de peças/óleos.</p>
        </article>
      </div>
    </section>

    <!-- SKILLS & ABOUT -->
    <section id="sobre">
      <h2 style="color:var(--accent);margin-bottom:12px">Habilidades</h2>
      <div class="card skills">
        <ul>
          <li class="skill">HTML & CSS</li>
          <li class="skill">JavaScript (Vanilla)</li>
          <li class="skill">Node.js / Express</li>
          <li class="skill">MySQL</li>
          <li class="skill">Python</li>
          <li class="skill">Leaflet / Mapas</li>
        </ul>

        <h3 style="color:var(--accent);margin-top:14px">Cursos e objetivos</h3>
        <p class="muted">Primeiro: Ciência de Dados para Negócios na FATEC Sebrae. Depois: especializações e projetos aplicados.</p>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contato">
      <h2 style="color:var(--accent);margin-bottom:12px">Contato</h2>
      <div class="card contact">
        <p class="muted">Quer trabalhar junto, pedir um projeto ou só trocar uma ideia? Me chama:</p>
        <div class="links" style="margin-top:12px">
          <a href="mailto:raphaelpireshp@gmail.com">✉ raphaelpireshp@gmail.com</a>
          <a href="https://www.linkedin.com/in/raphaelpireshp" target="_blank">🔗 LinkedIn</a>
          <a href="https://github.com/raphaelpireshp" target="_blank">🐙 GitHub</a>
        </div>

        <div style="margin-top:14px;color:var(--muted)">
          <small>Visit counter:</small>
          <div style="margin-top:8px"><img src="https://visit-counter.vercel.app/counter.png?page=https%3A%2F%2Fgithub.com%2Fraphaelpireshp&s=21&c=4CAF50&bg=00000000&no=2&ff=digi&tb=Visitas%3A++&ta=" alt="contador" style="height:36px"></div>
        </div>
      </div>
    </section>

    <footer>
      <p>&copy; 2025 <strong>raphaelpireshp</strong> — Feito com ☕ & código.</p>
    </footer>
  </div>

  <script>
    // Tema persistente
    (function(){
      const html = document.documentElement;
      const btn = document.getElementById('themeToggle');
      const saved = localStorage.getItem('theme') || 'dark';
      if(saved === 'light') html.setAttribute('data-theme','light');

      function updateIcon(){
        const i = btn.querySelector('i');
        const t = html.getAttribute('data-theme') === 'light' ? 'light' : 'dark';
        i.className = t === 'light' ? 'fa fa-sun' : 'fa fa-moon';
      }

      btn.addEventListener('click', ()=>{
        const cur = html.getAttribute('data-theme') === 'light' ? 'light' : 'dark';
        const next = cur === 'light' ? 'dark' : 'light';
        html.setAttribute('data-theme', next);
        localStorage.setItem('theme', next);
        updateIcon();
      });

      updateIcon();

      // Smooth anchor scroll
      document.querySelectorAll('a[href^="#"]').forEach(a=>{
        a.addEventListener('click', e=>{
          const href = a.getAttribute('href');
          if(href.length>1){ e.preventDefault(); document.querySelector(href).scrollIntoView({behavior:'smooth'}); }
        })
      });
    })();
  </script>
</body>
</html>
