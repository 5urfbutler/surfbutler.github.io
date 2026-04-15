<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>TreCastr - hyperlocal information viewer</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f5f2ec;
      --ink: #1a1a18;
      --muted: #6b6860;
      --accent: #2d5a3d;
      --accent-light: #e8f0eb;
      --border: #d8d4cc;
      --card: #ffffff;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      background: var(--bg);
      color: var(--ink);
      font-family: 'DM Sans', sans-serif;
      font-weight: 300;
      line-height: 1.7;
      min-height: 100vh;
    }

    /* Subtle grain overlay */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 0;
    }

    .wrap {
      position: relative;
      z-index: 1;
      max-width: 720px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    /* ── Header ── */
    header {
      padding: 4rem 0 3rem;
      border-bottom: 1px solid var(--border);
    }

    .wordmark {
      font-family: 'DM Serif Display', serif;
      font-size: clamp(2.4rem, 6vw, 3.6rem);
      letter-spacing: -0.02em;
      color: var(--ink);
      line-height: 1;
    }

    .wordmark em {
      font-style: italic;
      color: var(--accent);
    }

    .tagline {
      margin-top: 0.75rem;
      font-size: 1rem;
      color: var(--muted);
      font-weight: 400;
      letter-spacing: 0.01em;
    }

    /* ── Nav pills ── */
    nav {
      margin-top: 1.5rem;
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
    }

    nav a {
      display: inline-block;
      padding: 0.35rem 1rem;
      border: 1px solid var(--border);
      border-radius: 999px;
      font-size: 0.85rem;
      font-weight: 500;
      color: var(--muted);
      text-decoration: none;
      transition: border-color 0.2s, color 0.2s, background 0.2s;
    }

    nav a:hover {
      border-color: var(--accent);
      color: var(--accent);
      background: var(--accent-light);
    }

    /* ── Sections ── */
    section {
      padding: 3.5rem 0;
      border-bottom: 1px solid var(--border);
    }

    section:last-of-type { border-bottom: none; }

    .section-label {
      font-size: 0.7rem;
      font-weight: 500;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 1.25rem;
    }

    h2 {
      font-family: 'DM Serif Display', serif;
      font-size: clamp(1.5rem, 4vw, 2rem);
      font-weight: 400;
      letter-spacing: -0.01em;
      line-height: 1.2;
      margin-bottom: 1.25rem;
    }

    p { color: var(--muted); margin-bottom: 1rem; }
    p:last-child { margin-bottom: 0; }

    /* ── Info card ── */
    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 1.5rem 1.75rem;
      margin-top: 1.5rem;
    }

    .card-row {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      gap: 1rem;
      padding: 0.6rem 0;
      border-bottom: 1px solid var(--border);
      font-size: 0.9rem;
    }

    .card-row:last-child { border-bottom: none; }

    .card-row .label { color: var(--muted); font-weight: 400; }
    .card-row .value { color: var(--ink); font-weight: 500; text-align: right; }

    /* ── Policy list ── */
    .policy-item {
      display: flex;
      gap: 1rem;
      padding: 1rem 0;
      border-bottom: 1px solid var(--border);
      align-items: flex-start;
    }

    .policy-item:last-child { border-bottom: none; }

    .policy-dot {
      flex-shrink: 0;
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: var(--accent);
      margin-top: 0.55rem;
    }

    .policy-text { font-size: 0.92rem; color: var(--muted); }
    .policy-text strong { color: var(--ink); font-weight: 500; }

    /* ── Support button ── */
    .support-link {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      margin-top: 1.5rem;
      padding: 0.75rem 1.5rem;
      background: var(--accent);
      color: #fff;
      border-radius: 8px;
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 500;
      transition: opacity 0.2s;
    }

    .support-link:hover { opacity: 0.85; }

    /* ── Footer ── */
    footer {
      padding: 2.5rem 0;
      font-size: 0.8rem;
      color: var(--muted);
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    /* ── Fade-in animation ── */
    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(18px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    header, section {
      animation: fadeUp 0.5s ease both;
    }

    section:nth-of-type(1) { animation-delay: 0.1s; }
    section:nth-of-type(2) { animation-delay: 0.2s; }
    section:nth-of-type(3) { animation-delay: 0.3s; }
  </style>
</head>
<body>
  <div class="wrap">

    <header>
      <div class="wordmark">TreCast<em>r</em></div>
      <p class="tagline">A hyperlocal information viewer app for iOS, iPadOS and macOS.</p>
      <nav>
        <a href="#support">Support</a>
        <a href="#privacy">Privacy Policy</a>
      </nav>
    </header>

    <!-- Support -->
    <section id="support">
      <div class="section-label">Get help</div>
      <h2>Support</h2>
      <p>If you have a question, found a bug, or need assistance with TreCast<em>r</em>, get in touch and we'll do our best to help.</p>
      <a class="support-link" href="mailto:shard.veggie.2v@icloud.com">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><polyline points="2,4 12,13 22,4"/></svg>
        Email Support
      </a>
    </section>

    <!-- Privacy Policy -->
    <section id="privacy">
      <div class="section-label">Legal</div>
      <h2>Privacy Policy</h2>
      <p>Last updated: <span id="date"></span></p>
      <p>This policy describes how TreCast<em>r</em> handles information when you use the application.</p>

      <div class="card">
        <div class="policy-item">
          <div class="policy-dot"></div>
          <div class="policy-text"><strong>No personal data collected.</strong> TreCast<em>r</em> does not collect, store, or transmit any personally identifiable information.</div>
        </div>
        <div class="policy-item">
          <div class="policy-dot"></div>
          <div class="policy-text"><strong>Crash reports and diagnostics.</strong> The app may collect anonymised crash reports and diagnostic information to help identify and fix bugs. This data does not include any personally identifiable information and is used solely to improve the stability of the application.</div>
        </div>
        <div class="policy-item">
          <div class="policy-dot"></div>
          <div class="policy-text"><strong>No third-party sharing.</strong> We do not sell, trade, or share any data with third parties.</div>
        </div>
        <div class="policy-item">
          <div class="policy-dot"></div>
          <div class="policy-text"><strong>No tracking.</strong> TreCast<em>r</em> does not track your behaviour across other apps or websites.</div>
        </div>
        <!-- <div class="policy-item">
          <div class="policy-dot"></div>
          <div class="policy-text"><strong>Local data stays local.</strong> Any data generated or used by the application remains on your device and is not uploaded to external servers.</div>
        </div> -->
      </div>

      <p style="margin-top:1.5rem; font-size:0.85rem;">Questions about this policy? Contact us at <a href="mailto:shard.veggie.2v@icloud.com" style="color:var(--accent);">shard.veggie.2v@icloud.com</a>.</p>
    </section>

    <footer>
      <span>© <span id="year"></span> Jon Starling</span>
      <span>Designed and built in Cornwall, UK</span>
    </footer>

  </div>

  <script>
    const now = new Date();
    document.getElementById('year').textContent = now.getFullYear();
    document.getElementById('date').textContent = now.toLocaleDateString('en-GB', { day: 'numeric', month: 'long', year: 'numeric' });
  </script>
</body>
</html>
