<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Privacy Policy - Rebound Arena</title>
  <meta name="description"
    content="Privacy Policy for Rebound Arena. Learn how your data is handled with respect to advertisements, in-app purchases, and device identifiers." />

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap"
    rel="stylesheet" />

  <style>
    :root {
      --bg-primary: #0b0f17;
      --bg-surface: #111827;
      --bg-surface-elevated: #1a2234;
      --bg-card: rgba(26, 34, 52, 0.7);
      --border-color: rgba(255, 255, 255, 0.08);
      --border-accent: rgba(99, 102, 241, 0.3);

      --text-primary: #f8fafc;
      --text-secondary: #94a3b8;
      --text-muted: #64748b;

      --primary: #6366f1;
      --primary-hover: #4f46e5;
      --primary-glow: rgba(99, 102, 241, 0.25);
      --accent-cyan: #06b6d4;
      --accent-emerald: #10b981;
      --accent-amber: #f59e0b;

      --radius-sm: 8px;
      --radius-md: 14px;
      --radius-lg: 20px;
      --shadow-subtle: 0 10px 30px -10px rgba(0, 0, 0, 0.5);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      background-color: var(--bg-primary);
      color: var(--text-primary);
      line-height: 1.7;
      -webkit-font-smoothing: antialiased;
      scroll-behavior: smooth;
    }

    /* Background aesthetic glow */
    .ambient-glow {
      position: fixed;
      top: -200px;
      right: -100px;
      width: 600px;
      height: 600px;
      background: radial-gradient(circle, rgba(99, 102, 241, 0.15) 0%, rgba(6, 182, 212, 0.05) 45%, transparent 70%);
      pointer-events: none;
      z-index: 0;
    }

    .ambient-glow-2 {
      position: fixed;
      bottom: -150px;
      left: -100px;
      width: 500px;
      height: 500px;
      background: radial-gradient(circle, rgba(16, 185, 129, 0.08) 0%, transparent 60%);
      pointer-events: none;
      z-index: 0;
    }

    /* Navigation Bar */
    header {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      background: rgba(11, 15, 23, 0.85);
      border-bottom: 1px solid var(--border-color);
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 16px 24px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .brand-box {
      display: flex;
      align-items: center;
      gap: 12px;
      text-decoration: none;
      color: var(--text-primary);
    }

    .brand-icon {
      width: 40px;
      height: 40px;
      border-radius: 12px;
      background: linear-gradient(135deg, #6366f1 0%, #06b6d4 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Outfit', sans-serif;
      font-weight: 800;
      font-size: 20px;
      color: white;
      box-shadow: 0 4px 14px var(--primary-glow);
    }

    .brand-title {
      font-family: 'Outfit', sans-serif;
      font-weight: 700;
      font-size: 1.25rem;
      letter-spacing: -0.02em;
    }

    .header-meta {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      padding: 6px 14px;
      border-radius: 9999px;
      font-size: 0.82rem;
      font-weight: 600;
      background: rgba(99, 102, 241, 0.12);
      border: 1px solid rgba(99, 102, 241, 0.25);
      color: #a5b4fc;
    }

    .badge-dot {
      width: 7px;
      height: 7px;
      border-radius: 50%;
      background-color: var(--accent-emerald);
      box-shadow: 0 0 8px var(--accent-emerald);
    }

    /* Main Container Layout */
    .page-wrapper {
      position: relative;
      z-index: 1;
      max-width: 1200px;
      margin: 0 auto;
      padding: 48px 24px 80px;
    }

    .hero-section {
      text-align: center;
      max-width: 800px;
      margin: 0 auto 56px;
    }

    .hero-tag {
      font-family: 'Outfit', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      font-size: 0.82rem;
      font-weight: 700;
      color: var(--accent-cyan);
      margin-bottom: 12px;
      display: inline-block;
    }

    .hero-title {
      font-family: 'Outfit', sans-serif;
      font-size: clamp(2.4rem, 5vw, 3.5rem);
      font-weight: 800;
      line-height: 1.15;
      letter-spacing: -0.03em;
      margin-bottom: 20px;
      background: linear-gradient(to right, #ffffff, #cbd5e1);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .hero-desc {
      font-size: 1.1rem;
      color: var(--text-secondary);
      max-width: 660px;
      margin: 0 auto;
    }

    /* Privacy Summary Cards */
    .summary-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-bottom: 56px;
    }

    .summary-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      padding: 24px;
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      transition: transform 0.2s ease, border-color 0.2s ease;
    }

    .summary-card:hover {
      transform: translateY(-3px);
      border-color: var(--border-accent);
    }

    .card-icon {
      width: 44px;
      height: 44px;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 20px;
      margin-bottom: 16px;
    }

    .icon-safe {
      background: rgba(16, 185, 129, 0.15);
      color: var(--accent-emerald);
    }

    .icon-ads {
      background: rgba(6, 182, 212, 0.15);
      color: var(--accent-cyan);
    }

    .icon-iap {
      background: rgba(99, 102, 241, 0.15);
      color: #a5b4fc;
    }

    .icon-child {
      background: rgba(245, 158, 11, 0.15);
      color: var(--accent-amber);
    }

    .summary-card h3 {
      font-family: 'Outfit', sans-serif;
      font-size: 1.1rem;
      font-weight: 700;
      margin-bottom: 8px;
      color: var(--text-primary);
    }

    .summary-card p {
      font-size: 0.92rem;
      color: var(--text-secondary);
      line-height: 1.55;
    }

    /* Document Structure (TOC + Content) */
    .content-layout {
      display: grid;
      grid-template-columns: 280px 1fr;
      gap: 48px;
      align-items: start;
    }

    /* Sidebar Navigation */
    .sidebar {
      position: sticky;
      top: 100px;
      background: var(--bg-surface);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      padding: 24px;
    }

    .sidebar-title {
      font-family: 'Outfit', sans-serif;
      font-size: 0.85rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--text-muted);
      margin-bottom: 16px;
    }

    .toc-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .toc-link {
      display: block;
      padding: 8px 12px;
      border-radius: var(--radius-sm);
      color: var(--text-secondary);
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 500;
      transition: all 0.2s ease;
    }

    .toc-link:hover,
    .toc-link.active {
      color: #ffffff;
      background: rgba(99, 102, 241, 0.15);
      padding-left: 16px;
    }

    /* Policy Content */
    .policy-content {
      background: var(--bg-surface);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      padding: 44px;
      box-shadow: var(--shadow-subtle);
    }

    .policy-section {
      margin-bottom: 44px;
      scroll-margin-top: 110px;
    }

    .policy-section:last-child {
      margin-bottom: 0;
    }

    .policy-section h2 {
      font-family: 'Outfit', sans-serif;
      font-size: 1.65rem;
      font-weight: 700;
      color: var(--text-primary);
      margin-bottom: 18px;
      display: flex;
      align-items: center;
      gap: 12px;
      letter-spacing: -0.02em;
      border-bottom: 1px solid rgba(255, 255, 255, 0.06);
      padding-bottom: 12px;
    }

    .policy-section h2 .sec-num {
      color: var(--accent-cyan);
      font-size: 1.15rem;
      font-weight: 800;
    }

    .policy-section p {
      color: #cbd5e1;
      margin-bottom: 16px;
      font-size: 1rem;
    }

    .policy-section ul {
      list-style-type: none;
      margin-bottom: 20px;
      padding-left: 0;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .policy-section ul li {
      position: relative;
      padding-left: 28px;
      color: #cbd5e1;
    }

    .policy-section ul li::before {
      content: "•";
      position: absolute;
      left: 10px;
      top: -2px;
      color: var(--primary);
      font-size: 1.5rem;
    }

    /* Highlight Callout Box */
    .callout-box {
      background: rgba(99, 102, 241, 0.08);
      border-left: 4px solid var(--primary);
      border-radius: 0 var(--radius-sm) var(--radius-sm) 0;
      padding: 18px 22px;
      margin: 22px 0;
    }

    .callout-box.safe {
      background: rgba(16, 185, 129, 0.08);
      border-left-color: var(--accent-emerald);
    }

    .callout-title {
      font-family: 'Outfit', sans-serif;
      font-weight: 700;
      font-size: 1rem;
      color: #ffffff;
      margin-bottom: 6px;
    }

    .callout-box p {
      margin-bottom: 0;
      font-size: 0.95rem;
      color: #e2e8f0;
    }

    /* Partner Grid / Third Party Links */
    .provider-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 16px;
      margin: 22px 0;
    }

    .provider-card {
      background: var(--bg-surface-elevated);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-sm);
      padding: 16px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      transition: all 0.2s ease;
    }

    .provider-card:hover {
      border-color: var(--border-accent);
      transform: translateY(-2px);
    }

    .provider-name {
      font-weight: 700;
      color: #ffffff;
      font-size: 0.98rem;
      margin-bottom: 4px;
    }

    .provider-role {
      font-size: 0.82rem;
      color: var(--text-muted);
      margin-bottom: 12px;
    }

    .provider-link {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      color: var(--accent-cyan);
      font-size: 0.85rem;
      font-weight: 600;
      text-decoration: none;
    }

    .provider-link:hover {
      text-decoration: underline;
    }

    /* Contact Box */
    .contact-card {
      background: linear-gradient(135deg, rgba(99, 102, 241, 0.1) 0%, rgba(6, 182, 212, 0.1) 100%);
      border: 1px solid var(--border-accent);
      border-radius: var(--radius-md);
      padding: 28px;
      margin-top: 24px;
    }

    .contact-info-list {
      margin-top: 14px;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .contact-item {
      display: flex;
      align-items: center;
      gap: 12px;
      color: #e2e8f0;
      font-size: 0.98rem;
    }

    .contact-item a {
      color: var(--accent-cyan);
      text-decoration: none;
      font-weight: 600;
    }

    .contact-item a:hover {
      text-decoration: underline;
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--border-color);
      padding: 36px 24px;
      text-align: center;
      color: var(--text-muted);
      font-size: 0.88rem;
      margin-top: 60px;
    }

    .footer-content {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 12px;
    }

    /* Action Buttons */
    .action-bar {
      display: flex;
      gap: 12px;
      margin-top: 24px;
      justify-content: flex-end;
    }

    .btn-action {
      background: var(--bg-surface-elevated);
      border: 1px solid var(--border-color);
      color: var(--text-secondary);
      padding: 8px 16px;
      border-radius: var(--radius-sm);
      font-size: 0.85rem;
      font-weight: 600;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      transition: all 0.2s ease;
    }

    .btn-action:hover {
      color: #ffffff;
      border-color: var(--border-accent);
    }

    /* Responsive */
    @media (max-width: 900px) {
      .content-layout {
        grid-template-columns: 1fr;
      }

      .sidebar {
        display: none;
      }

      .policy-content {
        padding: 28px 20px;
      }

      .action-bar {
        justify-content: center;
      }
    }

    @media print {
      body {
        background: #ffffff;
        color: #000000;
      }

      .ambient-glow,
      .ambient-glow-2,
      header,
      .sidebar,
      .action-bar,
      footer {
        display: none !important;
      }

      .policy-content {
        border: none;
        box-shadow: none;
        padding: 0;
      }

      .policy-section h2 {
        color: #000000;
      }

      .policy-section p,
      .policy-section ul li {
        color: #333333;
      }

      .callout-box {
        background: #f1f5f9;
        border-left-color: #333333;
      }

      .provider-card {
        background: #f8fafc;
        border: 1px solid #e2e8f0;
      }
    }
  </style>
</head>

<body>

  <div class="ambient-glow"></div>
  <div class="ambient-glow-2"></div>

  <!-- Header Navigation -->
  <header>
    <div class="nav-container">
      <a href="#" class="brand-box">
        <div class="brand-icon">R</div>
        <span class="brand-title">Rebound Arena</span>
      </a>
      <div class="header-meta">
        <span class="badge">
          <span class="badge-dot"></span>
          Effective: September 2026
        </span>
      </div>
    </div>
  </header>

  <!-- Main Container -->
  <main class="page-wrapper">

    <!-- Hero Title -->
    <section class="hero-section">
      <span class="hero-tag">Transparency & Trust</span>
      <h1 class="hero-title">Privacy Policy</h1>
      <p class="hero-desc">
        We respect your privacy. <strong>Rebound Arena</strong> does not collect or sell your personal details. Learn
        how game features, advertisements, and store purchases operate below.
      </p>
      <div class="action-bar">
        <button class="btn-action" onclick="window.print()">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"
            stroke-linecap="round" stroke-linejoin="round">
            <polyline points="6 9 6 2 18 2 18 9"></polyline>
            <path d="M6 18H4a2 2 0 0 1-2-2v-5a2 2 0 0 1 2-2h16a2 2 0 0 1 2 2v5a2 2 0 0 1-2 2h-2"></path>
            <rect x="6" y="14" width="12" height="8"></rect>
          </svg>
          Print / Save PDF
        </button>
      </div>
    </section>

    <!-- Quick Summary Cards -->
    <div class="summary-grid">
      <div class="summary-card">
        <div class="card-icon icon-safe">🛡️</div>
        <h3>No Personal Data</h3>
        <p>We do not collect or store sensitive personal information like your name, email, physical address, or phone
          number.</p>
      </div>

      <div class="summary-card">
        <div class="card-icon icon-ads">📢</div>
        <h3>Third-Party Ads</h3>
        <p>The game serves ads via trusted networks which may process anonymous device identifiers to show relevant
          advertisements.</p>
      </div>

      <div class="summary-card">
        <div class="card-icon icon-iap">💳</div>
        <h3>Secure Purchases</h3>
        <p>In-app purchases are securely processed by Apple or Google. We never see or store your payment details or
          card numbers.</p>
      </div>

      <div class="summary-card">
        <div class="card-icon icon-child">👶</div>
        <h3>Child Privacy</h3>
        <p>We care deeply about safety and comply with COPPA, GDPR-K, and mobile store family requirements.</p>
      </div>
    </div>

    <!-- Content Layout with Sticky Sidebar -->
    <div class="content-layout">
      <!-- Sidebar Navigation -->
      <aside class="sidebar">
        <div class="sidebar-title">Table of Contents</div>
        <ul class="toc-list" id="toc-list">
          <li><a href="#introduction" class="toc-link">1. Introduction</a></li>
          <li><a href="#no-data" class="toc-link">2. Data We Do Not Collect</a></li>
          <li><a href="#third-parties" class="toc-link">3. Third-Party Services</a></li>
          <li><a href="#in-app-purchases" class="toc-link">4. In-App Purchases</a></li>
          <li><a href="#advertising" class="toc-link">5. Advertising & Device IDs</a></li>
          <li><a href="#children" class="toc-link">6. Children's Privacy</a></li>
          <li><a href="#security" class="toc-link">7. Data Storage & Security</a></li>
          <li><a href="#user-rights" class="toc-link">8. Your Privacy Rights</a></li>
          <li><a href="#changes" class="toc-link">9. Policy Changes</a></li>
          <li><a href="#contact" class="toc-link">10. Contact Us</a></li>
        </ul>
      </aside>

      <!-- Main Policy Content -->
      <article class="policy-content">

        <!-- Section 1 -->
        <section id="introduction" class="policy-section">
          <h2><span class="sec-num">01.</span> Introduction</h2>
          <p>
            Welcome to <strong>Rebound Arena</strong> (the "Game", "App", "we", "us", or "our"). This Privacy Policy
            explains our practices regarding your information when you install, play, or interact with Rebound Arena on
            iOS and Android devices.
          </p>
          <p>
            By downloading or playing Rebound Arena, you acknowledge and agree to the terms described in this Privacy
            Policy. If you do not agree with this policy, please do not use the Game.
          </p>
        </section>

        <!-- Section 2 -->
        <section id="no-data" class="policy-section">
          <h2><span class="sec-num">02.</span> Information We Do Not Collect</h2>
          <p>
            Rebound Arena is built primarily as an offline-friendly entertainment experience. <strong>We do not maintain
              our own user accounts, registration databases, or backend servers that harvest personal data.</strong>
          </p>
          <div class="callout-box safe">
            <div class="callout-title">Direct Developer Collection: None</div>
            <p>We do NOT collect, store, share, or sell any of the following directly:</p>
          </div>
          <ul>
            <li>Full legal names, usernames, or physical home addresses</li>
            <li>Email addresses or phone numbers</li>
            <li>Contacts, microphone, camera, or photo library files</li>
            <li>Precise real-time GPS location coordinates</li>
            <li>Biometric or health data</li>
          </ul>
          <p>
            Game progress, local high scores, and unlocked items are stored locally on your device (or synchronized via
            your platform's native cloud save system, such as Apple iCloud or Google Play Games, according to your
            device configuration).
          </p>
        </section>

        <!-- Section 3 -->
        <section id="third-parties" class="policy-section">
          <h2><span class="sec-num">03.</span> Third-Party Services & SDKs</h2>
          <p>
            While we do not collect personal data ourselves, Rebound Arena integrates standard third-party software
            development kits (SDKs) to provide in-game advertisements, support in-app purchases, and ensure game
            stability.
          </p>
          <p>
            These third parties may automatically collect non-personal device information (such as operating system
            version, device model, language settings, approximate IP-based geographic region, and advertising
            identifiers) in compliance with their own independent privacy policies:
          </p>

          <div class="provider-grid">
            <div class="provider-card">
              <div>
                <div class="provider-name">Unity Ads / Engine</div>
                <div class="provider-role">Game Engine & Ad Delivery</div>
              </div>
              <a class="provider-link" href="https://unity.com/legal/privacy-policy" target="_blank"
                rel="noopener noreferrer">
                View Privacy Policy &rarr;
              </a>
            </div>

            <div class="provider-card">
              <div>
                <div class="provider-name">Google AdMob</div>
                <div class="provider-role">Advertising Network</div>
              </div>
              <a class="provider-link" href="https://policies.google.com/privacy" target="_blank"
                rel="noopener noreferrer">
                View Privacy Policy &rarr;
              </a>
            </div>

            <div class="provider-card">
              <div>
                <div class="provider-name">Google Play Services</div>
                <div class="provider-role">Billing & Store Distribution</div>
              </div>
              <a class="provider-link" href="https://policies.google.com/privacy" target="_blank"
                rel="noopener noreferrer">
                View Privacy Policy &rarr;
              </a>
            </div>

            <div class="provider-card">
              <div>
                <div class="provider-name">Apple App Store</div>
                <div class="provider-role">In-App Purchases & Distribution</div>
              </div>
              <a class="provider-link" href="https://www.apple.com/legal/privacy/" target="_blank"
                rel="noopener noreferrer">
                View Privacy Policy &rarr;
              </a>
            </div>
          </div>
        </section>

        <!-- Section 4 -->
        <section id="in-app-purchases" class="policy-section">
          <h2><span class="sec-num">04.</span> In-App Purchases (IAP)</h2>
          <p>
            Rebound Arena offers optional virtual goods or ad-removal through in-app purchases.
          </p>
          <ul>
            <li><strong>No Financial Access:</strong> All transactions are executed through Apple App Store (In-App
              Purchase) or Google Play (Google Play Billing). We never receive, process, or store your credit card
              numbers, billing addresses, or financial credentials.</li>
            <li><strong>Receipt Validation:</strong> The game receives an encrypted digital token from the store
              platform confirming whether an item was successfully purchased or restored, enabling the purchased feature
              inside the game.</li>
          </ul>
        </section>

        <!-- Section 5 -->
        <section id="advertising" class="policy-section">
          <h2><span class="sec-num">05.</span> Advertising & Device Identifiers</h2>
          <p>
            Rebound Arena may display advertisements (such as rewarded video ads or banner ads) to support ongoing game
            development.
          </p>
          <p>
            Advertising networks use device identifiers (such as Apple's Identifier for Advertisers —
            <strong>IDFA</strong> on iOS, or Google's Advertising ID — <strong>GAID</strong> on Android) to:
          </p>
          <ul>
            <li>Measure ad performance and view counts</li>
            <li>Prevent fraud and repetitive ad displays</li>
            <li>Deliver relevant advertisements (subject to your consent preferences)</li>
          </ul>

          <div class="callout-box">
            <div class="callout-title">How to Opt-Out or Reset Ad Tracking:</div>
            <p><strong>On iOS:</strong> Go to <em>Settings &gt; Privacy &amp; Security &gt; Tracking</em>, where you can
              disable tracking requests or revoke permissions for Rebound Arena.</p>
            <p style="margin-top: 6px;"><strong>On Android:</strong> Go to <em>Settings &gt; Google &gt; Ads</em> (or
              <em>Privacy &gt; Ads</em>) and choose to "Delete Advertising ID" or "Reset Advertising ID".</p>
          </div>
        </section>

        <!-- Section 6 -->
        <section id="children" class="policy-section">
          <h2><span class="sec-num">06.</span> Children's Privacy (COPPA & GDPR-K)</h2>
          <p>
            Protecting the privacy of children is of paramount importance to us. Rebound Arena is designed for general
            audiences and does not knowingly collect personally identifiable information from children under the age of
            13 (or 16 in the European Union).
          </p>
          <p>
            If ad providers serve ads in the game, we request that ad networks operate in accordance with COPPA, showing
            non-personalized or contextual advertising where appropriate. If you believe a child has provided personal
            information to us without parental consent, please contact us immediately, and we will take swift action to
            verify and erase any such information.
          </p>
        </section>

        <!-- Section 7 -->
        <section id="security" class="policy-section">
          <h2><span class="sec-num">07.</span> Data Storage, Retention & Security</h2>
          <p>
            Because we do not store personal data on remote developer servers, your gameplay data remains primarily on
            your physical device. If you uninstall the Game or clear its application storage, any locally held game
            progression data will be deleted unless backed up by your device's native cloud mechanism.
          </p>
          <p>
            We implement standard best practices and use encrypted communication protocols (HTTPS) whenever the Game
            communicates with third-party verification or ad endpoints.
          </p>
        </section>

        <!-- Section 8 -->
        <section id="user-rights" class="policy-section">
          <h2><span class="sec-num">08.</span> Your Privacy Rights (GDPR & CCPA)</h2>
          <p>
            Depending on your jurisdiction (such as the European Economic Area, the United Kingdom, California, or other
            US states), you may have specific legal rights regarding your data:
          </p>
          <ul>
            <li><strong>Right to Know / Access:</strong> You may request information on what categories of data
              third-party networks collect.</li>
            <li><strong>Right to Deletion:</strong> You can delete all local data at any time by uninstalling the
              application. For third-party ad identifiers, you can reset or delete them through your operating system
              settings.</li>
            <li><strong>Right to Opt-Out of "Sale" or "Sharing":</strong> We do not sell your personal data. You can
              limit personalized ad tracking via your device settings as detailed in Section 5.</li>
            <li><strong>Non-Discrimination:</strong> Exercising your privacy rights will never result in degraded game
              mechanics or denial of game services.</li>
          </ul>
        </section>

        <!-- Section 9 -->
        <section id="changes" class="policy-section">
          <h2><span class="sec-num">09.</span> Changes to This Privacy Policy</h2>
          <p>
            We may occasionally update this Privacy Policy to reflect changes in our practices, new game updates, or
            evolving legal and regulatory obligations.
          </p>
          <p>
            When changes are made, we will update the "Effective Date" at the top of this document. We encourage players
            to periodically review this page to stay informed about our commitment to user privacy.
          </p>
        </section>

        <!-- Section 10 -->
        <section id="contact" class="policy-section">
          <h2><span class="sec-num">10.</span> Contact Information</h2>
          <p>
            If you have questions, feedback, or concerns regarding this Privacy Policy or Rebound Arena, please feel
            free to reach out to us:
          </p>

          <div class="contact-card">
            <div class="callout-title" style="font-size: 1.15rem; margin-bottom: 8px;">Rebound Arena Support</div>
            <p>We are available to answer any questions or clarify any privacy concerns.</p>
            <div class="contact-info-list">
              <div class="contact-item">
                <span>📧 <strong>Developer Email:</strong></span>
                <a href="mailto:support@reboundarena.com">support@reboundarena.com</a>
                <span style="color: var(--text-muted); font-size: 0.85rem;">(replace with your email)</span>
              </div>
              <div class="contact-item">
                <span>🌐 <strong>Project Repository:</strong></span>
                <a href="https://github.com" target="_blank" rel="noopener noreferrer">GitHub Project Page</a>
              </div>
            </div>
          </div>
        </section>

      </article>
    </div>
  </main>

  <!-- Footer -->
  <footer>
    <div class="footer-content">
      <p>&copy; 2026 Rebound Arena. All rights reserved.</p>
      <p style="font-size: 0.8rem; color: var(--text-muted);">
        This policy is hosted publicly for Google Play Store and Apple App Store compliance.
      </p>
    </div>
  </footer>

  <!-- Table of Contents Active Link Highlight Script -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const sections = document.querySelectorAll('.policy-section');
      const tocLinks = document.querySelectorAll('.toc-link');

      const observerOptions = {
        root: null,
        rootMargin: '-20% 0px -70% 0px',
        threshold: 0
      };

      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            const id = entry.target.getAttribute('id');
            tocLinks.forEach(link => {
              if (link.getAttribute('href') === `#${id}`) {
                link.classList.add('active');
              } else {
                link.classList.remove('active');
              }
            });
          }
        });
      }, observerOptions);

      sections.forEach(section => observer.observe(section));
    });
  </script>
</body>

</html>
