<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>TERRA — Pitch Shark Tank</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;0,400;0,500;0,600;1,400&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#F7F4EC;
    --bg-panel:#FFFFFF;
    --navy:#101E33;
    --navy-2:#1C3358;
    --gold:#9C7C3C;
    --gold-2:#B79654;
    --text:#171A1F;
    --muted:#63625A;
    --line:rgba(16,30,51,0.14);
    --hairline:rgba(16,30,51,0.09);
  }
  :root:not([data-theme="light"]) {
    @media (prefers-color-scheme: dark){
      --bg:#0B1420;
      --bg-panel:#101C2C;
      --navy:#F3EEE1;
      --navy-2:#E3D9BE;
      --gold:#C9A968;
      --gold-2:#DFC183;
      --text:#EDE9DD;
      --muted:#A6A192;
      --line:rgba(243,238,225,0.14);
      --hairline:rgba(243,238,225,0.08);
    }
  }
  :root[data-theme="dark"]{
    --bg:#0B1420;
    --bg-panel:#101C2C;
    --navy:#F3EEE1;
    --navy-2:#E3D9BE;
    --gold:#C9A968;
    --gold-2:#DFC183;
    --text:#EDE9DD;
    --muted:#A6A192;
    --line:rgba(243,238,225,0.14);
    --hairline:rgba(243,238,225,0.08);
  }
  *{box-sizing:border-box;margin:0;padding:0;}
  html{scroll-behavior:smooth; scroll-padding-top:env(safe-area-inset-top,0px);}
  html,body{height:100%;}
  body{
    background:var(--bg);
    color:var(--text);
    font-family:'Inter',sans-serif;
    line-height:1.65;
    padding-top:env(safe-area-inset-top,0px);
    padding-bottom:env(safe-area-inset-bottom,0px);
    -webkit-font-smoothing:antialiased;
  }
  .wrap{max-width:1120px;margin:0 auto;padding:0 48px;}
  h1,h2,h3{font-family:'Cormorant',serif;font-weight:500;color:var(--navy);}
  .mono{font-family:'IBM Plex Mono',monospace;}
  a{color:inherit;text-decoration:none;}
  .eyebrow{
    font-size:0.78rem;
    letter-spacing:0.18em;
    text-transform:uppercase;
    color:var(--gold);
    font-weight:600;
    margin-bottom:20px;
  }
  .hairline{width:100%;height:1px;background:var(--hairline);}

  /* NAV */
  nav{
    position:sticky;top:0;z-index:30;
    background:color-mix(in srgb, var(--bg) 88%, transparent);
    backdrop-filter:blur(10px);
    border-bottom:1px solid var(--hairline);
    padding-top:env(safe-area-inset-top,0px);
  }
  nav .wrap{display:flex;justify-content:space-between;align-items:center;height:78px;}
  .wordmark{font-family:'Cormorant',serif;font-size:1.5rem;letter-spacing:0.06em;color:var(--navy);}
  .wordmark .leaf{color:var(--gold);}
  .navlinks{display:flex;gap:34px;font-size:0.76rem;letter-spacing:0.1em;text-transform:uppercase;color:var(--muted);}
  .navlinks a:hover{color:var(--gold);}

  /* HERO */
  .hero{padding:150px 0 130px;text-align:center;border-bottom:1px solid var(--hairline);}
  .crest{width:56px;height:56px;margin:0 auto 34px;opacity:0.9;}
  .hero h1{font-size:5.6rem;letter-spacing:0.02em;line-height:1;margin-bottom:22px;}
  .hero .tag{font-family:'Cormorant',serif;font-style:italic;font-size:1.5rem;color:var(--navy-2);max-width:560px;margin:0 auto 40px;}
  .founders{font-size:0.82rem;letter-spacing:0.08em;text-transform:uppercase;color:var(--muted);margin-bottom:46px;}
  .founders span{color:var(--navy);}
  .scroll-cta{display:inline-block;border:1px solid var(--gold);color:var(--navy);padding:15px 40px;font-size:0.78rem;letter-spacing:0.12em;text-transform:uppercase;transition:all .25s;}
  .scroll-cta:hover{background:var(--gold);color:var(--bg);}

  /* SECTION */
  section{padding:104px 0;border-bottom:1px solid var(--hairline);}
  .num-tag{font-family:'Cormorant',serif;font-style:italic;font-size:1.1rem;color:var(--gold);margin-bottom:6px;display:block;}
  .section-title{font-size:2.6rem;max-width:640px;margin-bottom:14px;line-height:1.15;}
  .section-kicker{max-width:600px;color:var(--muted);font-size:1.02rem;margin-bottom:56px;}

  .two-col{display:grid;grid-template-columns:0.85fr 1.15fr;gap:70px;align-items:start;}
  .lead-col p{color:var(--navy);font-size:1.5rem;font-family:'Cormorant',serif;font-style:italic;line-height:1.4;}
  .body-col p{color:var(--muted);margin-bottom:18px;max-width:520px;}
  .body-col strong{color:var(--text);font-weight:600;}

  .stat-row{display:grid;grid-template-columns:repeat(3,1fr);gap:0;border-top:1px solid var(--hairline);border-bottom:1px solid var(--hairline);margin:52px 0;}
  .stat{padding:30px 28px;border-right:1px solid var(--hairline);}
  .stat:last-child{border-right:none;}
  .stat .big{font-family:'Cormorant',serif;font-size:2.4rem;color:var(--navy);display:block;}
  .stat .cap{font-size:0.78rem;letter-spacing:0.06em;color:var(--muted);text-transform:uppercase;margin-top:6px;}

  .compare-grid{display:grid;grid-template-columns:1fr 1fr;gap:0;border:1px solid var(--hairline);}
  .compare-card{padding:38px 36px;border-right:1px solid var(--hairline);}
  .compare-card:last-child{border-right:none;}
  .compare-card h4{font-size:1.35rem;margin-bottom:14px;}
  .compare-card ul{list-style:none;}
  .compare-card li{color:var(--muted);font-size:0.92rem;padding:8px 0;border-top:1px solid var(--hairline);}
  .compare-card li:first-child{border-top:none;}
  .compare-card.us{background:var(--bg-panel);}
  .compare-card.us h4{color:var(--gold);}

  .flow{display:grid;grid-template-columns:repeat(4,1fr);border:1px solid var(--hairline);margin:52px 0;}
  .flow-step{padding:32px 26px;border-right:1px solid var(--hairline);}
  .flow-step:last-child{border-right:none;}
  .flow-step .rn{font-family:'Cormorant',serif;font-style:italic;color:var(--gold);font-size:1.7rem;display:block;margin-bottom:12px;}
  .flow-step h5{font-family:'Inter';font-weight:600;font-size:0.95rem;margin-bottom:6px;color:var(--text);}
  .flow-step p{color:var(--muted);font-size:0.85rem;}

  table{width:100%;border-collapse:collapse;font-size:0.92rem;}
  th{text-align:left;font-family:'IBM Plex Mono',monospace;font-size:0.74rem;letter-spacing:0.05em;text-transform:uppercase;color:var(--gold);padding:12px 0;border-bottom:1px solid var(--line);font-weight:500;}
  td{padding:14px 0;border-bottom:1px solid var(--hairline);color:var(--muted);font-family:'IBM Plex Mono',monospace;font-size:0.86rem;}
  td.label-col{color:var(--text);font-family:'Inter';}
  td.num,th.num{text-align:right;}
  tr.total td{color:var(--gold);font-weight:600;border-bottom:none;padding-top:18px;}

  /* CHART */
  .chart-box{border:1px solid var(--hairline);padding:48px 50px;margin-top:56px;}
  .chart-box h4{font-size:1.4rem;margin-bottom:6px;}
  .chart-box .sub{color:var(--muted);font-size:0.88rem;margin-bottom:30px;}
  .chart-svg{width:100%;height:auto;}

  /* TEAM */
  .team-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:0;border:1px solid var(--hairline);}
  .team-card{padding:42px 34px;border-right:1px solid var(--hairline);text-align:center;}
  .team-card:last-child{border-right:none;}
  .avatar{width:64px;height:64px;border-radius:50%;border:1px solid var(--gold);margin:0 auto 22px;display:flex;align-items:center;justify-content:center;font-family:'Cormorant',serif;font-size:1.4rem;color:var(--gold);}
  .team-card h4{font-size:1.25rem;margin-bottom:8px;line-height:1.3;}
  .team-card .role{font-size:0.76rem;letter-spacing:0.08em;text-transform:uppercase;color:var(--gold);margin-bottom:14px;}
  .team-card p{color:var(--muted);font-size:0.88rem;}

  /* INVESTMENT */
  .ask-box{background:var(--navy);color:var(--bg);padding:60px;text-align:center;border-radius:2px;}
  :root[data-theme="dark"] .ask-box, :root:not([data-theme="light"]) .ask-box{
    color:var(--bg);
  }
  .ask-box .amount{font-family:'Cormorant',serif;font-size:4rem;color:var(--gold-2);margin-bottom:10px;}
  .ask-box .desc{font-size:1rem;opacity:0.85;max-width:480px;margin:0 auto 34px;}
  .use-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:30px;max-width:600px;margin:0 auto;}
  .use-item .pct{font-family:'Cormorant',serif;font-size:1.8rem;color:var(--gold-2);}
  .use-item .lbl{font-size:0.76rem;letter-spacing:0.05em;text-transform:uppercase;opacity:0.75;margin-top:4px;}

  /* CLOSING */
  .closing{text-align:center;padding:150px 0;border-bottom:none;}
  .closing .eyebrow{justify-content:center;}
  .closing h2{font-size:3rem;max-width:760px;margin:0 auto 30px;line-height:1.25;}
  .closing p{max-width:520px;margin:0 auto;color:var(--muted);font-size:1.05rem;}

  footer{padding:50px 0 60px;text-align:center;}
  footer p{color:var(--muted);font-size:0.78rem;letter-spacing:0.04em;}

  @media (max-width:860px){
    .wrap{padding:0 26px;}
    .hero h1{font-size:3.2rem;}
    .two-col{grid-template-columns:1fr;gap:36px;}
    .stat-row{grid-template-columns:1fr;}
    .stat{border-right:none;border-bottom:1px solid var(--hairline);}
    .compare-grid{grid-template-columns:1fr;}
    .compare-card{border-right:none;border-bottom:1px solid var(--hairline);}
    .flow{grid-template-columns:1fr;}
    .flow-step{border-right:none;border-bottom:1px solid var(--hairline);}
    .team-grid{grid-template-columns:1fr;}
    .team-card{border-right:none;border-bottom:1px solid var(--hairline);}
    .use-grid{grid-template-columns:1fr;gap:20px;}
    .navlinks{display:none;}
    .ask-box{padding:40px 26px;}
  }
</style>
</head>
<body>

<nav>
  <div class="wrap">
    <div class="wordmark">TERRA<span class="leaf">.</span></div>
    <div class="navlinks">
      <a href="#mercado">Mercado</a>
      <a href="#negocio">Negocio</a>
      <a href="#finanzas">Finanzas</a>
      <a href="#equipo">Equipo</a>
      <a href="#inversion">Inversión</a>
    </div>
  </div>
</nav>

<section class="hero">
  <div class="wrap">
    <svg class="crest" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
      <circle cx="50" cy="50" r="38" stroke="currentColor" style="color:var(--gold)" stroke-width="1.2"/>
      <circle cx="50" cy="50" r="30" stroke="currentColor" style="color:var(--gold)" stroke-width="0.6"/>
      <line x1="50" y1="16" x2="50" y2="24" stroke="currentColor" style="color:var(--gold)" stroke-width="1.2"/>
      <line x1="50" y1="76" x2="50" y2="84" stroke="currentColor" style="color:var(--gold)" stroke-width="1.2"/>
      <line x1="50" y1="50" x2="50" y2="30" stroke="currentColor" style="color:var(--navy)" stroke-width="1.4"/>
      <line x1="50" y1="50" x2="64" y2="58" stroke="currentColor" style="color:var(--navy)" stroke-width="1.4"/>
    </svg>
    <div class="eyebrow" style="justify-content:center;display:flex;">Proyecto Shark Tank · Bachillerato</div>
    <h1>TERRA</h1>
    <p class="tag">El cuidado personal que tu piel y el planeta pueden confiar.</p>
    <p class="founders">Fundado por <span>José Arturo Cervantes Andrade</span> · <span>Fidel Nicolás Pablo León</span> · <span>Leonardo García Villalpando</span></p>
    <a href="#problema" class="scroll-cta">Ver el pitch completo</a>
  </div>
</section>

<section id="problema">
  <div class="wrap">
    <span class="num-tag">01</span>
    <h2 class="section-title">El problema</h2>
    <div class="two-col">
      <div class="lead-col">
        <p>"La mayoría de los desodorantes que usamos todos los días llevan aluminio, plásticos de un solo uso y químicos que nadie se detiene a leer."</p>
      </div>
      <div class="body-col">
        <p>El desodorante es uno de los productos de higiene personal más usados a diario — y también uno de los menos cuestionados. La mayoría de las fórmulas del mercado masivo contienen sales de aluminio y conservadores agresivos, y prácticamente todas se venden en envases plásticos de un solo uso.</p>
        <p>Al mismo tiempo, cada vez más consumidores —sobre todo jóvenes— buscan alternativas más saludables y sostenibles, pero se encuentran con opciones naturales que son importadas, costosas o difíciles de conseguir en México.</p>
      </div>
    </div>
  </div>
</section>

<section id="solucion">
  <div class="wrap">
    <span class="num-tag">02</span>
    <h2 class="section-title">La solución</h2>
    <div class="two-col">
      <div class="lead-col">
        <p>Un desodorante ecológico, formulado con ingredientes naturales y envasado de forma biodegradable — hecho en México.</p>
      </div>
      <div class="body-col">
        <p>TERRA neutraliza el olor sin bloquear la sudoración natural del cuerpo, usando una fórmula a base de aceite de coco, manteca de karité, bicarbonato de sodio y aceites esenciales. Cero aluminio, cero parabenos, cero crueldad animal.</p>
        <p>Se presenta en un tubo biodegradable de bajo impacto ambiental, con una versión en frasco de vidrio reutilizable para quienes buscan una experiencia más duradera.</p>
      </div>
    </div>
  </div>
</section>

<section id="mercado">
  <div class="wrap">
    <span class="num-tag">03</span>
    <h2 class="section-title">El mercado</h2>
    <p class="section-kicker">Un mercado pequeño y alcanzable para empezar, con espacio real para crecer poco a poco.</p>

    <div class="stat-row">
      <div class="stat">
        <span class="big">~800</span>
        <span class="cap">Personas en la comunidad escolar y el círculo cercano — mercado inicial alcanzable</span>
      </div>
      <div class="stat">
        <span class="big">~75</span>
        <span class="cap">Clientes meta para el primer año, comprando 1-2 veces</span>
      </div>
      <div class="stat">
        <span class="big">15–35</span>
        <span class="cap">Rango de edad del cliente ideal, activo y cercano al equipo</span>
      </div>
    </div>

    <div class="two-col">
      <div class="lead-col">
        <p>No necesitamos todo el mercado — necesitamos convencer a las primeras 75 personas de que esto funciona.</p>
      </div>
      <div class="body-col">
        <p><strong>Cliente ideal:</strong> compañeros de escuela, sus familias y contactos cercanos al equipo, con vida activa (deporte, escuela) y ya interesados en productos naturales o sostenibles.</p>
        <p><strong>Oportunidad:</strong> empezamos con un mercado pequeño y controlable — nuestra propia comunidad escolar — antes de pensar en vender fuera de ese círculo. Es una base realista para medir si el producto funciona antes de invertir en crecer.</p>
      </div>
    </div>
  </div>
</section>

<section id="competencia">
  <div class="wrap">
    <span class="num-tag">04</span>
    <h2 class="section-title">Competencia y diferenciación</h2>
    <p class="section-kicker">No competimos en el mismo terreno que las marcas masivas, ni en el mismo precio que las importadas.</p>
    <div class="compare-grid">
      <div class="compare-card">
        <h4>El mercado hoy</h4>
        <ul>
          <li>Rexona, Dove, Secret, Nivea — fórmula con aluminio, producción industrial</li>
          <li>NaturalDry, Immi, Zahal — naturales, ya presentes en México</li>
          <li>Tom's of Maine, Weleda — naturales, importadas, precio elevado</li>
        </ul>
      </div>
      <div class="compare-card us">
        <h4>TERRA</h4>
        <ul>
          <li>Producción artesanal en lotes pequeños, con trazabilidad total</li>
          <li>Fórmula pensada para después de la actividad física, no genérica</li>
          <li>Envase biodegradable desde la presentación de entrada</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="negocio">
  <div class="wrap">
    <span class="num-tag">05</span>
    <h2 class="section-title">Modelo de negocio</h2>
    <p class="section-kicker">Producción por lotes, venta directa e institucional, con márgenes saludables desde la primera unidad.</p>

    <div class="flow">
      <div class="flow-step"><span class="rn">I</span><h5>Producción por lote</h5><p>20 unidades cada tres semanas, elaboración manual con control de calidad, escalando conforme crece la demanda.</p></div>
      <div class="flow-step"><span class="rn">II</span><h5>Venta directa</h5><p>Redes sociales, ferias y pedidos personalizados — el mayor margen.</p></div>
      <div class="flow-step"><span class="rn">III</span><h5>Venta institucional</h5><p>Tiendas eco-conscientes y gimnasios, con precio de mayoreo.</p></div>
      <div class="flow-step"><span class="rn">IV</span><h5>Reinversión</h5><p>Parte del margen regresa a materia prima del siguiente lote.</p></div>
    </div>

    <table>
      <tr><th>Presentación</th><th class="num">Costo</th><th class="num">Precio</th><th class="num">Margen</th></tr>
      <tr><td class="label-col">Clásica (tubo biodegradable, lote piloto)</td><td class="num">$18</td><td class="num">$65</td><td class="num">≈72%</td></tr>
      <tr><td class="label-col">Mayoreo / eventos (mín. 10 pzas)</td><td class="num">$18</td><td class="num">$48</td><td class="num">≈63%</td></tr>
    </table>
  </div>
</section>

<section id="finanzas">
  <div class="wrap">
    <span class="num-tag">06</span>
    <h2 class="section-title">Proyecciones financieras</h2>
    <p class="section-kicker">Cifras conservadoras basadas en un crecimiento gradual de producción y canales de distribución.</p>

    <table>
      <tr><th>Horizonte</th><th class="num">Unidades / año</th><th class="num">Ingresos</th><th class="num">Utilidad estimada</th></tr>
      <tr><td class="label-col">Piloto actual (lote 1, 20 u.)</td><td class="num">20</td><td class="num">$1,300</td><td class="num">$940</td></tr>
      <tr><td class="label-col">Año 1 (ritmo ~12 u./mes)</td><td class="num">150</td><td class="num">$9,000</td><td class="num">$6,300</td></tr>
      <tr><td class="label-col">Año 3 (ritmo ~25 u./mes)</td><td class="num">300</td><td class="num">$17,400</td><td class="num">$12,000</td></tr>
      <tr class="total"><td>Año 5 (ritmo ~42 u./mes)</td><td class="num">500</td><td class="num">$27,500</td><td class="num">$18,500</td></tr>
    </table>

    <div class="chart-box">
      <h4>Crecimiento de ingresos proyectado</h4>
      <div class="sub">Cifras en miles de pesos mexicanos (MXN)</div>
      <svg class="chart-svg" viewBox="0 0 760 260" xmlns="http://www.w3.org/2000/svg">
        <line x1="60" y1="20" x2="60" y2="210" stroke="var(--hairline)" stroke-width="1"/>
        <line x1="60" y1="210" x2="720" y2="210" stroke="var(--hairline)" stroke-width="1"/>
        <line x1="60" y1="150" x2="720" y2="150" stroke="var(--hairline)" stroke-width="0.6" stroke-dasharray="2,4"/>
        <line x1="60" y1="90" x2="720" y2="90" stroke="var(--hairline)" stroke-width="0.6" stroke-dasharray="2,4"/>
        <line x1="60" y1="30" x2="720" y2="30" stroke="var(--hairline)" stroke-width="0.6" stroke-dasharray="2,4"/>

        <polyline points="120,153 400,100 680,36" fill="none" stroke="var(--gold)" stroke-width="1.6"/>
        <circle cx="120" cy="153" r="4" fill="var(--navy)"/>
        <circle cx="400" cy="100" r="4" fill="var(--navy)"/>
        <circle cx="680" cy="36" r="5" fill="var(--gold)"/>

        <text x="120" y="230" text-anchor="middle" font-family="IBM Plex Mono, monospace" font-size="12" fill="var(--muted)">Año 1</text>
        <text x="400" y="230" text-anchor="middle" font-family="IBM Plex Mono, monospace" font-size="12" fill="var(--muted)">Año 3</text>
        <text x="680" y="230" text-anchor="middle" font-family="IBM Plex Mono, monospace" font-size="12" fill="var(--muted)">Año 5</text>

        <text x="120" y="137" text-anchor="middle" font-family="Cormorant, serif" font-size="15" fill="var(--navy)">$9.0k</text>
        <text x="400" y="84" text-anchor="middle" font-family="Cormorant, serif" font-size="15" fill="var(--navy)">$17.4k</text>
        <text x="680" y="22" text-anchor="middle" font-family="Cormorant, serif" font-size="16" fill="var(--gold)">$27.5k</text>
      </svg>
    </div>

    <div class="stat-row" style="margin-top:56px;">
      <div class="stat">
        <span class="big">4 u/mes</span>
        <span class="cap">Punto de equilibrio estimado (costos fijos casi nulos)</span>
      </div>
      <div class="stat">
        <span class="big">Mes 1</span>
        <span class="cap">Momento en que se alcanza el punto de equilibrio</span>
      </div>
      <div class="stat">
        <span class="big">$715</span>
        <span class="cap">Inversión de arranque ya cubierta por el equipo</span>
      </div>
    </div>
  </div>
</section>

<section id="equipo">
  <div class="wrap">
    <span class="num-tag">07</span>
    <h2 class="section-title">Equipo</h2>
    <p class="section-kicker">Tres estudiantes, tres roles complementarios.</p>
    <div class="team-grid">
      <div class="team-card">
        <div class="avatar">JA</div>
        <h4>José Arturo Cervantes Andrade</h4>
        <div class="role">Dirección creativa y de marca</div>
        <p>Identidad de marca, diseño y presentación del producto.</p>
      </div>
      <div class="team-card">
        <div class="avatar">FN</div>
        <h4>Fidel Nicolás Pablo León</h4>
        <div class="role">Desarrollo de producto</div>
        <p>Formulación, materiales y control de calidad.</p>
      </div>
      <div class="team-card">
        <div class="avatar">LG</div>
        <h4>Leonardo García Villalpando</h4>
        <div class="role">Finanzas y estrategia comercial</div>
        <p>Costos, precios, canales de venta y proyecciones.</p>
      </div>
    </div>
  </div>
</section>

<section id="inversion">
  <div class="wrap">
    <span class="num-tag">08</span>
    <h2 class="section-title">La inversión</h2>
    <p class="section-kicker">Un monto pequeño para financiar los siguientes lotes, acorde a una operación que ya se sostiene sola.</p>
    <div class="ask-box">
      <div class="amount">$800 <span style="font-size:1.6rem;">MXN</span></div>
      <div class="desc">A cambio del 8% de la empresa, para producir los siguientes dos lotes sin depender del margen de ventas anteriores.</div>
      <div class="use-grid">
        <div class="use-item"><div class="pct">55%</div><div class="lbl">Materia prima</div></div>
        <div class="use-item"><div class="pct">30%</div><div class="lbl">Envase y etiqueta</div></div>
        <div class="use-item"><div class="pct">15%</div><div class="lbl">Imprevistos</div></div>
      </div>
    </div>
  </div>
</section>

<section class="closing">
  <div class="wrap">
    <div class="eyebrow">Cierre</div>
    <h2>Con tu inversión, TERRA puede pasar de un proyecto escolar a la alternativa ecológica de cuidado personal favorita de México — un frasco a la vez.</h2>
    <p>Problema real. Solución probada. Mercado en crecimiento. Equipo comprometido.</p>
  </div>
</section>

<footer>
  <div class="wrap">
    <p>TERRA — Proyecto Shark Tank · Bachillerato · 2026</p>
  </div>
</footer>

</body>
</html>
