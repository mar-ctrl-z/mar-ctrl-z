[marina_stardew_readme.html](https://github.com/user-attachments/files/27168615/marina_stardew_readme.html)
<style>
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&family=VT323&display=swap');

  :root {
    --sv-green: #558e34;
    --sv-green-light: #76b361;
    --sv-green-dark: #2d5a1b;
    --sv-gold: #e8c84a;
    --sv-gold-dark: #b89520;
    --sv-brown: #7a4f2e;
    --sv-brown-light: #c8956c;
    --sv-cream: #f5edd6;
    --sv-sky: #a8d8ea;
    --sv-dirt: #8b6340;
    --sv-purple: #5c3d7a;
    --sv-red: #c94444;
    --sv-teal: #3aafa9;
    --sv-border: #3d2b1a;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; image-rendering: pixelated; }

  body { background: transparent; }

  .readme-wrap {
    font-family: 'VT323', monospace;
    background: var(--sv-cream);
    color: var(--sv-border);
    padding: 0;
    position: relative;
    overflow: hidden;
    border: 4px solid var(--sv-border);
    image-rendering: pixelated;
  }

  .pixel-border {
    border: 4px solid var(--sv-border);
    box-shadow: 4px 4px 0 var(--sv-border);
  }

  /* ---- HEADER ---- */
  .header {
    background: linear-gradient(180deg, #a8d8ea 0%, #c5e8b4 60%, #76b361 100%);
    padding: 32px 24px 0;
    position: relative;
    text-align: center;
    border-bottom: 4px solid var(--sv-border);
  }

  .sun {
    position: absolute; top: 14px; right: 30px;
    width: 36px; height: 36px;
    background: var(--sv-gold);
    border: 3px solid var(--sv-gold-dark);
    border-radius: 0;
    clip-path: polygon(50% 0%,61% 35%,98% 35%,68% 57%,79% 91%,50% 70%,21% 91%,32% 57%,2% 35%,39% 35%);
    animation: spin 8s linear infinite;
  }
  @keyframes spin { to { transform: rotate(360deg); } }

  .cloud {
    position: absolute; top: 12px; left: 20px;
    width: 60px; height: 22px;
    background: #fff;
    border: 3px solid #ddd;
    border-radius: 0;
    animation: float 6s ease-in-out infinite;
  }
  .cloud::before {
    content: ''; position: absolute; top: -12px; left: 10px;
    width: 24px; height: 24px; background: #fff; border: 3px solid #ddd;
  }
  .cloud::after {
    content: ''; position: absolute; top: -8px; left: 28px;
    width: 18px; height: 18px; background: #fff; border: 3px solid #ddd;
  }
  @keyframes float { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-5px)} }

  .header-title {
    font-family: 'Press Start 2P', monospace;
    font-size: 13px;
    color: var(--sv-green-dark);
    text-shadow: 2px 2px 0 var(--sv-gold);
    margin-bottom: 6px;
    letter-spacing: 1px;
  }

  .header-subtitle {
    font-size: 22px;
    color: var(--sv-brown);
    margin-bottom: 4px;
  }

  .avatar-ring {
    display: inline-block;
    border: 5px solid var(--sv-green);
    box-shadow: 0 0 0 3px var(--sv-gold), 4px 4px 0 var(--sv-border);
    background: var(--sv-sky);
    width: 90px; height: 90px;
    position: relative;
    overflow: hidden;
    margin: 12px auto 0;
    display: flex; align-items: center; justify-content: center;
  }

  .avatar-emoji { font-size: 52px; line-height: 1; }

  .ground {
    background: var(--sv-green);
    border-top: 4px solid var(--sv-green-dark);
    height: 18px;
    position: relative;
    display: flex; align-items: center; justify-content: center; gap: 12px;
    padding: 0 8px;
  }
  .crop { font-size: 14px; }

  /* ---- BADGES ---- */
  .badges {
    display: flex; flex-wrap: wrap; gap: 6px;
    padding: 14px 18px;
    background: var(--sv-brown-light);
    border-bottom: 4px solid var(--sv-border);
    justify-content: center;
  }

  .badge {
    font-family: 'Press Start 2P', monospace;
    font-size: 7px;
    padding: 5px 10px;
    border: 3px solid var(--sv-border);
    box-shadow: 2px 2px 0 var(--sv-border);
    display: inline-flex; align-items: center; gap: 4px;
    cursor: default;
    transition: transform 0.1s;
    white-space: nowrap;
  }
  .badge:hover { transform: translate(-1px,-1px); box-shadow: 3px 3px 0 var(--sv-border); }

  .badge-green { background: var(--sv-green); color: var(--sv-cream); }
  .badge-purple { background: var(--sv-purple); color: var(--sv-cream); }
  .badge-teal { background: var(--sv-teal); color: #fff; }
  .badge-brown { background: var(--sv-brown); color: var(--sv-cream); }

  /* ---- BODY ---- */
  .body { padding: 0; }

  /* ---- SECTION ---- */
  .section {
    margin: 14px;
    border: 3px solid var(--sv-border);
    box-shadow: 3px 3px 0 var(--sv-border);
  }

  .section-header {
    font-family: 'Press Start 2P', monospace;
    font-size: 9px;
    background: var(--sv-green);
    color: var(--sv-cream);
    padding: 8px 12px;
    border-bottom: 3px solid var(--sv-border);
    display: flex; align-items: center; gap: 8px;
  }

  .section-header.gold { background: var(--sv-gold); color: var(--sv-border); }
  .section-header.brown { background: var(--sv-brown); color: var(--sv-cream); }
  .section-header.purple { background: var(--sv-purple); color: var(--sv-cream); }
  .section-header.teal { background: var(--sv-teal); color: #fff; }

  .section-body {
    background: #fffdf4;
    padding: 12px 14px;
  }

  /* ---- QUEST ---- */
  .quest {
    background: #fff9e8;
    border: 2px solid var(--sv-gold-dark);
    padding: 10px 12px;
    margin-bottom: 10px;
    font-size: 18px;
    position: relative;
  }
  .quest:last-child { margin-bottom: 0; }

  .quest-title {
    font-family: 'Press Start 2P', monospace;
    font-size: 8px;
    color: var(--sv-brown);
    margin-bottom: 5px;
    display: flex; align-items: center; gap: 6px;
  }

  .quest-status {
    display: inline-block;
    font-family: 'Press Start 2P', monospace;
    font-size: 6px;
    padding: 2px 5px;
    border: 2px solid var(--sv-border);
    background: var(--sv-green); color: var(--sv-cream);
    box-shadow: 1px 1px 0 var(--sv-border);
  }

  .quest-desc { font-size: 17px; color: var(--sv-border); line-height: 1.4; }
  .quest-reward { font-size: 15px; color: var(--sv-gold-dark); margin-top: 4px; }

  /* ---- SKILLS GRID ---- */
  .skills-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 8px;
  }

  .skill-card {
    background: #fff9e8;
    border: 2px solid var(--sv-border);
    box-shadow: 2px 2px 0 var(--sv-border);
    padding: 8px 10px;
  }

  .skill-card-title {
    font-family: 'Press Start 2P', monospace;
    font-size: 7px;
    color: var(--sv-green-dark);
    margin-bottom: 6px;
    padding-bottom: 4px;
    border-bottom: 2px solid var(--sv-green-light);
  }

  .skill-tag {
    display: inline-block;
    font-size: 14px;
    background: var(--sv-green-light);
    color: var(--sv-green-dark);
    border: 1px solid var(--sv-green-dark);
    padding: 1px 6px;
    margin: 2px 2px 0 0;
    cursor: default;
  }
  .skill-tag.blue { background: #b3d9f5; color: #1a4a72; border-color: #1a4a72; }
  .skill-tag.purple { background: #d5c4f0; color: var(--sv-purple); border-color: var(--sv-purple); }
  .skill-tag.brown { background: #e8cdb2; color: var(--sv-brown); border-color: var(--sv-brown); }

  /* ---- STATS BAR ---- */
  .stat-row { display: flex; align-items: center; gap: 8px; margin-bottom: 8px; }
  .stat-label { font-size: 17px; min-width: 110px; color: var(--sv-border); }
  .stat-bar-bg {
    flex: 1; height: 14px; background: #ddd;
    border: 2px solid var(--sv-border);
    position: relative; overflow: hidden;
  }
  .stat-bar-fill {
    height: 100%;
    background: var(--sv-green);
    animation: grow 1.5s ease-out both;
  }
  @keyframes grow { from { width: 0 } }
  .stat-bar-fill.gold { background: var(--sv-gold); }
  .stat-bar-fill.purple { background: var(--sv-purple); }
  .stat-bar-fill.teal { background: var(--sv-teal); }

  /* ---- QUOTE ---- */
  .quote-box {
    margin: 14px;
    background: var(--sv-green-dark);
    border: 3px solid var(--sv-border);
    box-shadow: 3px 3px 0 var(--sv-border);
    padding: 14px 18px;
    color: var(--sv-cream);
    font-size: 17px;
    line-height: 1.5;
    text-align: center;
  }

  .quote-mark {
    font-family: 'Press Start 2P', monospace;
    font-size: 20px;
    color: var(--sv-gold);
    display: block;
    margin-bottom: 6px;
  }

  /* ---- LINKS ---- */
  .links-row {
    display: flex; gap: 8px; flex-wrap: wrap;
    padding: 12px 14px;
    background: var(--sv-brown-light);
    border-top: 4px solid var(--sv-border);
    justify-content: center;
  }

  .sv-link {
    font-family: 'Press Start 2P', monospace;
    font-size: 7px;
    padding: 7px 12px;
    border: 3px solid var(--sv-border);
    box-shadow: 2px 2px 0 var(--sv-border);
    text-decoration: none;
    display: inline-flex; align-items: center; gap: 5px;
    transition: transform 0.1s, box-shadow 0.1s;
  }
  .sv-link:hover { transform: translate(-1px,-1px); box-shadow: 3px 3px 0 var(--sv-border); }
  .sv-link.li { background: #0077B5; color: #fff; }
  .sv-link.gm { background: #D14836; color: #fff; }
  .sv-link.lt { background: #fff; color: var(--sv-border); }

  /* ---- PIXEL DIVIDER ---- */
  .px-div {
    height: 8px;
    background: repeating-linear-gradient(90deg, var(--sv-green) 0 8px, var(--sv-gold) 8px 16px);
    border-top: 2px solid var(--sv-border);
    border-bottom: 2px solid var(--sv-border);
  }

  .info-row {
    font-family: 'Press Start 2P', monospace;
    font-size: 7px;
    text-align: center;
    padding: 8px;
    background: var(--sv-cream);
    color: var(--sv-brown);
    border-bottom: 3px solid var(--sv-border);
    letter-spacing: 1px;
  }
</style>

<div class="readme-wrap">

  <!-- HEADER -->
  <div class="header">
    <div class="sun"></div>
    <div class="cloud"></div>
    <div class="header-title">✦ PERFIL DA FAZENDEIRA ✦</div>
    <div class="avatar-ring">
      <span class="avatar-emoji">👩‍💻</span>
    </div>
    <div style="margin-top:8px;">
      <span style="font-family:'Press Start 2P',monospace;font-size:11px;color:var(--sv-green-dark);text-shadow:1px 1px 0 var(--sv-gold)">Marina Conrado</span>
    </div>
    <div style="font-size:18px;color:var(--sv-brown);margin:4px 0 10px;">Picos, Piauí  🌾  IA & Visão Computacional</div>
    <div class="ground">
      <span class="crop">🌾</span><span class="crop">🌿</span><span class="crop">🌻</span><span class="crop">🌾</span><span class="crop">🍄</span><span class="crop">🌿</span><span class="crop">🌾</span>
    </div>
  </div>

  <!-- BADGES -->
  <div class="badges">
    <span class="badge badge-green">🌾 Fazendeira de Dados</span>
    <span class="badge badge-purple">🤖 IA &amp; ML</span>
    <span class="badge badge-teal">☁️ Cloud &amp; DevOps</span>
    <span class="badge badge-brown">📚 Pesquisadora</span>
  </div>

  <div class="px-div"></div>
  <div class="info-row">📍 Nível: Desenvolvedor ★★★★☆ &nbsp;|&nbsp; Estação: Primavera 2026 🌸</div>

  <div class="body">

    <!-- QUEST LOG -->
    <div class="section">
      <div class="section-header gold">📜 Quest Log — Missões Ativas</div>
      <div class="section-body">

        <div class="quest">
          <div class="quest-title">
            🐾 RASTREAMENTO DE RUMINANTES
            <span class="quest-status">🟢 EM PROGRESSO</span>
          </div>
          <div class="quest-desc">YOLOv8 para detecção de pequenos ruminantes em ambientes semiáridos.</div>
          <div class="quest-reward">✨ Recompensa: +1000g XP · Gestão Rural Inteligente</div>
        </div>

        <div class="quest">
          <div class="quest-title">
            💻 PROJETOS EM CULTIVO
            <span class="quest-status" style="background:var(--sv-teal)">🔵 ATIVO</span>
          </div>
          <div class="quest-desc">Deep Learning · Kubernetes · Análise de Dados · UX Research</div>
          <div class="quest-reward">✨ Recompensa: Soluções inovadoras para o campo</div>
        </div>

      </div>
    </div>

    <!-- INVENTÁRIO -->
    <div class="section">
      <div class="section-header brown">🎒 Inventário — Tech Stack</div>
      <div class="section-body">
        <div class="skills-grid">
          <div class="skill-card">
            <div class="skill-card-title">🧠 IA &amp; Dados</div>
            <span class="skill-tag">Python</span>
            <span class="skill-tag">PyTorch</span>
            <span class="skill-tag">YOLOv8</span>
            <span class="skill-tag">Scikit-learn</span>
            <span class="skill-tag">Pandas</span>
          </div>
          <div class="skill-card">
            <div class="skill-card-title">🏗️ DevOps</div>
            <span class="skill-tag blue">Docker</span>
            <span class="skill-tag blue">Kubernetes</span>
            <span class="skill-tag blue">AWS</span>
            <span class="skill-tag blue">PostgreSQL</span>
          </div>
          <div class="skill-card">
            <div class="skill-card-title">🎨 Design</div>
            <span class="skill-tag purple">Figma</span>
            <span class="skill-tag purple">UX Research</span>
            <span class="skill-tag purple">SUS/UES</span>
          </div>
          <div class="skill-card">
            <div class="skill-card-title">📚 Acadêmico</div>
            <span class="skill-tag brown">LaTeX</span>
            <span class="skill-tag brown">BibTeX</span>
            <span class="skill-tag brown">Escrita Cient.</span>
          </div>
        </div>
      </div>
    </div>

    <!-- ATRIBUTOS -->
    <div class="section">
      <div class="section-header teal">⚡ Atributos da Fazendeira</div>
      <div class="section-body">
        <div class="stat-row">
          <span class="stat-label">🌾 Organização</span>
          <div class="stat-bar-bg"><div class="stat-bar-fill" style="width:90%"></div></div>
        </div>
        <div class="stat-row">
          <span class="stat-label">💪 Resiliência</span>
          <div class="stat-bar-bg"><div class="stat-bar-fill gold" style="width:95%;animation-delay:.2s"></div></div>
        </div>
        <div class="stat-row">
          <span class="stat-label">🤝 Colaboração</span>
          <div class="stat-bar-bg"><div class="stat-bar-fill teal" style="width:88%;animation-delay:.4s"></div></div>
        </div>
        <div class="stat-row">
          <span class="stat-label">🧠 Aprendizado</span>
          <div class="stat-bar-bg"><div class="stat-bar-fill purple" style="width:99%;animation-delay:.6s"></div></div>
        </div>
      </div>
    </div>

  </div>

  <!-- QUOTE -->
  <div class="quote-box">
    <span class="quote-mark">"</span>
    Assim como uma fazenda, o dev requer planejamento, dedicação e cuidado constante.
    A cada linha de código, colho algo maior que eu mesma.
    <span class="quote-mark">"</span>
  </div>

  <!-- LINKS -->
  <div class="links-row">
    <a class="sv-link li" href="https://www.linkedin.com/in/marina-conrado-a3640532b/" target="_blank">🔗 LinkedIn</a>
    <a class="sv-link gm" href="mailto:marinacms19@gmail.com">✉️ Gmail</a>
    <a class="sv-link lt" href="http://lattes.cnpq.br/5225020120155051" target="_blank">📄 Lattes</a>
  </div>

</div>
