<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Trofeos de Golf | Catálogo</title>

  <meta name="description" content="Catálogo de trofeos de golf: copas, placas y medallas. Personalización con grabado y logo." />
  <meta name="robots" content="index,follow" />
  <meta name="theme-color" content="#0b1220" />

  <!-- Open Graph (para compartir) -->
  <meta property="og:title" content="Trofeos de Golf | Catálogo" />
  <meta property="og:description" content="Copas, placas y medallas para torneos. Grabado y personalización." />
  <meta property="og:type" content="website" />

  <link rel="stylesheet" href="css/styles.css" />
</head>

<body>
  <a class="skip" href="#catalogo">Saltar al catálogo</a>

  <header class="shell topbar" id="inicio">
    <a class="brand" href="#inicio" aria-label="Inicio">
      <span class="logo" aria-hidden="true">
        <svg width="22" height="22" viewBox="0 0 24 24" fill="none">
          <path d="M7 21h10" stroke="rgba(0,0,0,.55)" stroke-width="2" stroke-linecap="round"/>
          <path d="M8 3h8v4a4 4 0 0 1-4 4h0a4 4 0 0 1-4-4V3Z" fill="rgba(0,0,0,.55)"/>
          <path d="M6 7h2a4 4 0 0 0 4 4 4 4 0 0 0 4-4h2" stroke="rgba(0,0,0,.55)" stroke-width="2" stroke-linecap="round"/>
          <path d="M12 11v6" stroke="rgba(0,0,0,.55)" stroke-width="2" stroke-linecap="round"/>
        </svg>
      </span>
      <span class="brandText">
        <strong>Trofeos de Golf</strong>
        <span>Copas · Placas · Medallas · Grabado</span>
      </span>
    </a>

    <nav class="nav" aria-label="Navegación">
      <a class="chip" href="#catalogo">Catálogo</a>
      <a class="chip" href="#personalizacion">Personalización</a>
      <a class="chip" href="#contacto">Contacto</a>
    </nav>
  </header>

  <main class="shell">
    <section class="hero" aria-label="Presentación">
      <div class="heroMain">
        <p class="badge">Entrega 48–72h* · Grabado láser · Logo del club</p>
        <h1>Premios que elevan tu torneo.</h1>
        <p class="lead">
          Filtra por categoría, material y grabado. Pide presupuesto por email o WhatsApp en segundos.
        </p>
        <div class="ctaRow">
          <a class="btn primary" href="#catalogo">Ver catálogo</a>
          <a class="btn" href="#contacto">Pedir presupuesto</a>
          <button class="btn ghost" id="btnResetTop" type="button">Limpiar filtros</button>
        </div>
        <p class="fine">*Texto demo: ajusta plazos, precios y condiciones a tu negocio.</p>
      </div>

      <aside class="heroCard" aria-label="Resumen">
        <div class="kpis">
          <div class="kpi">
            <div class="num" id="kpiTotal">—</div>
            <div class="lbl">Modelos</div>
          </div>
          <div class="kpi">
            <div class="num">Grabado</div>
            <div class="lbl">Texto + logo</div>
          </div>
          <div class="kpi">
            <div class="num">Premium</div>
            <div class="lbl">Cristal / metal</div>
          </div>
          <div class="kpi">
            <div class="num">Packs</div>
            <div class="lbl">Por torneo</div>
          </div>
        </div>

        <div class="panel">
          <div class="row"><span>Eventos</span><b>Club · Empresa · Liga</b></div>
          <div class="row"><span>Formatos</span><b>Scramble · Stableford</b></div>
          <div class="row"><span>Opciones</span><b>Estuche / caja</b></div>
        </div>
      </aside>
    </section>

    <section id="catalogo" class="section" aria-label="Catálogo de productos">
      <header class="sectionHead">
        <h2>Catálogo</h2>
        <p>Busca y filtra. Pulsa “Ver detalle” para referencias y CTA.</p>
      </header>

      <div class="filters" role="region" aria-label="Filtros">
        <div class="field">
          <label for="q">Buscar</label>
          <input id="q" type="search" placeholder="Ej.: copa, placa, medalla, cristal..." autocomplete="off" />
        </div>

        <div class="field">
          <label for="cat">Categoría</label>
          <select id="cat">
            <option value="all">Todas</option>
            <option value="copa">Copa</option>
            <option value="placa">Placa</option>
            <option value="medalla">Medalla</option>
          </select>
        </div>

        <div class="field">
          <label for="mat">Material</label>
          <select id="mat">
            <option value="all">Todos</option>
            <option value="metal">Metal</option>
            <option value="cristal">Cristal</option>
            <option value="madera">Madera</option>
          </select>
        </div>

        <div class="field">
          <label for="grab">Grabado</label>
          <select id="grab">
            <option value="all">Indiferente</option>
            <option value="si">Con grabado</option>
            <option value="no">Sin grabado</option>
          </select>
        </div>

        <div class="field">
          <label for="sort">Orden</label>
          <select id="sort">
            <option value="recomendado">Recomendado</option>
            <option value="precioAsc">Precio: menor a mayor</option>
            <option value="precioDesc">Precio: mayor a menor</option>
            <option value="nombre">Nombre</option>
          </select>
        </div>

        <div class="field actions">
          <button class="btn danger" id="btnReset" type="button">Reset</button>
        </div>
      </div>

      <div class="resultsBar">
        <div id="resultInfo">—</div>
        <div class="hint">Tip: al pedir presupuesto, incluye cantidad y fecha.</div>
      </div>

      <div class="grid" id="grid" aria-live="polite"></div>
    </section>

    <section id="personalizacion" class="section">
      <header class="sectionHead">
        <h2>Personalización</h2>
        <p>Bloque listo para condiciones reales: mínimos, plazos, tipos de grabado y packaging.</p>
      </header>

      <div class="kpis four">
        <div class="kpi">
          <div class="num">Grabado</div>
          <div class="lbl">Nombre · fecha · categoría</div>
        </div>
        <div class="kpi">
          <div class="num">Logo</div>
          <div class="lbl">SVG recomendado</div>
        </div>
        <div class="kpi">
          <div class="num">Mockup</div>
          <div class="lbl">Antes de producir</div>
        </div>
        <div class="kpi">
          <div class="num">Packaging</div>
          <div class="lbl">Estuche / caja</div>
        </div>
      </div>
    </section>

    <section id="contacto" class="section">
      <header class="sectionHead">
        <h2>Contacto</h2>
        <p>Demo (sin backend). Conéctalo a tu email/CRM o un endpoint.</p>
      </header>

      <form id="contactForm" class="contact">
        <div class="field">
          <label for="name">Nombre</label>
          <input id="name" required placeholder="Tu nombre" />
        </div>

        <div class="field">
          <label for="email">Email</label>
          <input id="email" type="email" required placeholder="tu@email.com" />
        </div>

        <div class="field full">
          <label for="msg">Mensaje</label>
          <input id="msg" required placeholder="Ej.: 60 jugadores, 3 categorías, logo del club..." />
        </div>

        <div class="field full contactActions">
          <button class="btn primary" type="submit">Enviar</button>
          <a class="btn" id="mailtoBtn" href="#">Enviar por email</a>
          <a class="btn ghost" id="waBtn" href="#" rel="noopener">WhatsApp</a>
        </div>

        <p class="toast" id="toast" role="status" aria-live="polite"></p>
      </form>
    </section>

    <footer class="footer">
      <span>© <span id="year"></span> Trofeos de Golf · Demo</span>
      <span class="mono">HTML + CSS + JS (sin librerías)</span>
    </footer>
  </main>

  <!-- Modal -->
  <div class="modalBackdrop" id="modalBackdrop" role="dialog" aria-modal="true" aria-labelledby="modalTitle" hidden>
    <div class="modal" role="document">
      <header class="modalHeader">
        <strong id="modalTitle">Detalle</strong>
        <button class="iconBtn" id="closeModal" type="button" aria-label="Cerrar">✕</button>
      </header>

      <div class="modalBody">
        <div class="modalImg" aria-hidden="true">
          <svg width="84" height="84" viewBox="0 0 24 24" fill="none">
            <path d="M7 21h10" stroke="rgba(255,255,255,.85)" stroke-width="2" stroke-linecap="round"/>
            <path d="M8 3h8v4a4 4 0 0 1-4 4h0a4 4 0 0 1-4-4V3Z" fill="rgba(255,255,255,.85)"/>
            <path d="M6 7h2a4 4 0 0 0 4 4 4 4 0 0 0 4-4h2" stroke="rgba(255,255,255,.85)" stroke-width="2" stroke-linecap="round"/>
            <path d="M12 11v6" stroke="rgba(255,255,255,.85)" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </div>

        <div class="modalInfo">
          <p class="badge" id="modalBadge">—</p>

          <div class="panel">
            <div class="row"><span>Precio desde</span><b id="modalPrice">—</b></div>
            <div class="row"><span>Categoría</span><b id="modalCat">—</b></div>
            <div class="row"><span>Material</span><b id="modalMat">—</b></div>
            <div class="row"><span>Grabado</span><b id="modalGrab">—</b></div>
          </div>

          <p class="muted" id="modalDesc"></p>

          <div class="modalActions">
            <a class="btn primary" id="modalCta" href="#contacto">Solicitar presupuesto</a>
            <button class="btn ghost" id="copyRef" type="button">Copiar referencia</button>
            <a class="btn" id="modalWa" href="#" rel="noopener">WhatsApp</a>
          </div>

          <p class="toast" id="copyToast" role="status" aria-live="polite"></p>
        </div>
      </div>
    </div>
  </div>

  <script type="module" src="js/app.js"></script>
</body>
</html>


