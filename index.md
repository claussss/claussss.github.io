---
layout: single
permalink: /
title: "Yurii Halychanskyi"
description: "Yurii Halychanskyi — UIUC PhD student researching generative audio, speech, and accent conversion."
excerpt: "Yurii Halychanskyi is a PhD student at UIUC focusing on generative audio models, speech technology, and accent conversion."
last_modified_at: 2024-05-26
author: "Yurii Halychanskyi"
keywords: ["Yurii Halychanskyi", "PhD student", "UIUC", "Generative Audio", "Speech Conversion", "Accent Conversion", "Machine Learning"]
---

<style>
  /* ============================================================
     Theme palette — one set of tokens, overridden for dark mode.
     Everything below is built on these so light/dark stay in sync.
     ============================================================ */
  :root {
    --bg:          #f3f4f1;
    --surface:     #ffffff;
    --surface-2:   #f4f7fb;
    --bubble:      #ffffff;
    --text:        #20242b;
    --heading:     #1a1e25;
    --muted:       #55606e;
    --accent:      #2f6f8f;
    --accent-soft: #e7f0f4;
    --border:      #e6e3da;
    --ring:        #a7b89a;
    --shadow:      0 6px 18px rgba(60, 50, 30, 0.10);
    --shadow-sm:   0 2px 6px rgba(60, 50, 30, 0.05);
  }
  html[data-theme="dark"] {
    --bg:          #252a34;
    --surface:     #2e3440;
    --surface-2:   #2b303b;
    --bubble:      #363d4a;
    --text:        #e7ebf2;
    --heading:     #f2f5fa;
    --muted:       #b7c0cd;
    --accent:      #8ec7e3;
    --accent-soft: #2b4a57;
    --border:      #3b4252;
    --ring:        #46506180;
    --shadow:      0 8px 22px rgba(0, 0, 0, 0.40);
    --shadow-sm:   none;
  }

  /* Page background + smooth cross-fade when the theme is toggled */
  body, .page, .page__content, #main {
    background-color: var(--bg) !important;
  }
  body, .page__content, .header, .header-content h1,
  .publication-card, .publication-authors, .presentations-chat, .chat-bubble,
  .chat-meta, .venue-badge, .email, .social-links a, .section-title,
  .institution-details .location, .institution-details .degree,
  .institution-details .date, a {
    transition: background-color .45s ease, color .45s ease,
                border-color .45s ease, box-shadow .45s ease;
  }

  /* ---------------- Header card ---------------- */
  .header {
    display: flex;
    gap: 2rem;
    margin-bottom: 2.5rem;
    padding: 2rem;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    box-shadow: var(--shadow);
    align-items: center;
  }

  /* Profile picture: day + night stacked, cross-faded by theme.
     Both images are pixel-aligned to the same framing, so only the
     lighting appears to change when switching modes. */
  .profile-frame {
    position: relative;
    width: 300px;
    height: 300px;
    flex-shrink: 0;
  }
  .profile-img {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center 40%;
    transform: scale(1.05);
    border-radius: 14px;
    border: 2px solid var(--ring);
    box-shadow: 0 6px 16px rgba(0, 0, 0, 0.18);
    transition: opacity .6s ease, border-color .45s ease;
  }
  .profile-night { opacity: 0; }
  html[data-theme="dark"] .profile-day   { opacity: 0; }
  html[data-theme="dark"] .profile-night { opacity: 1; }

  /* ---------------- Header text ---------------- */
  .header-content h1 {
    font-size: 2.3rem;
    margin: 0 0 0.35rem 0;
    color: var(--heading);
    font-weight: 700;
    letter-spacing: -0.015em;
    background: none;
    -webkit-text-fill-color: initial;
  }
  .social-links {
    display: flex;
    gap: 1.1rem;
    align-items: center;
    margin: 0.6rem 0;
  }
  .social-links a {
    color: var(--muted);
    text-decoration: none;
    display: inline-flex;
    transition: transform .2s ease, opacity .2s ease;
  }
  .social-links a:hover { transform: translateY(-3px); }
  .social-links a img {
    width: 30px !important;
    height: 30px !important;
    display: block;
  }
  /* Monochrome logos (GitHub, X) are near-black — lighten them in dark mode */
  html[data-theme="dark"] .social-links a img.icon-mono {
    filter: invert(1) brightness(1.9);
  }
  .email {
    color: var(--accent);
    text-decoration: none;
    font-size: 1.05rem;
    margin: 0.4rem 0 0 0;
    display: inline-block;
  }
  .email:hover { text-decoration: underline; }

  /* ---------------- Sections ---------------- */
  .section { margin-bottom: 2.5rem; }
  .section-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--heading);
    margin: 0 0 1.1rem 0;
    padding-bottom: 0.45rem;
    letter-spacing: -0.01em;
    border-bottom: 1px solid var(--border);
    position: relative;
  }
  .section-title::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: -1px;
    width: 46px;
    height: 2px;
    background: var(--accent);
    border-radius: 2px;
  }
  .about-item p { color: var(--text); line-height: 1.6; }

  /* ---------------- Publications ---------------- */
  .publication-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 1.1rem 1.35rem 1.2rem;
    margin-bottom: 1rem;
    box-shadow: var(--shadow-sm);
    transition: transform .2s ease, box-shadow .2s ease,
                background-color .45s ease, border-color .45s ease;
  }
  .publication-card:hover {
    transform: translateY(-3px);
    box-shadow: var(--shadow);
  }
  .publication-card h3 {
    margin: 0.1rem 0 0.4rem 0;
    font-size: 1.13rem;
    line-height: 1.35;
    color: var(--heading);
  }
  .publication-authors {
    margin: 0.2rem 0 0.6rem 0;
    font-size: 0.95rem;
    color: var(--muted);
  }
  .author-me { color: var(--accent); }
  .publication-links a {
    margin-right: 0.85rem;
    font-weight: 600;
    font-size: 0.92rem;
    color: var(--accent);
    text-decoration: none;
  }
  .publication-links a:hover { text-decoration: underline; }

  /* Venue badges */
  .venue-row { margin-bottom: 0.55rem; }
  .venue-badge {
    display: inline-block;
    padding: 0.16rem 0.65rem;
    border-radius: 999px;
    font-size: 0.76rem;
    font-weight: 700;
    letter-spacing: 0.01em;
    background: var(--accent-soft);
    color: var(--accent);
    border: 1px solid transparent;
    margin: 0 0.4rem 0.3rem 0;
  }
  .venue-badge.preprint { background: #eef0f2; color: #5b6470; }
  .venue-badge.oral     { background: #fbe9c7; color: #8a5a00; }
  .venue-badge.poster   { background: #e8efe3; color: #4f6a3f; }
  html[data-theme="dark"] .venue-badge.preprint { background: #3b4252; color: #c0c6d0; }
  html[data-theme="dark"] .venue-badge.oral     { background: #5a4416; color: #f0c873; }
  html[data-theme="dark"] .venue-badge.poster   { background: #3a4636; color: #b7d3a3; }

  /* ---------------- Experience & Education ---------------- */
  .institution-logo {
    width: 92px;
    height: 92px;
    object-fit: contain;
    border-radius: 6px;
    margin-right: 1.2rem;
    background: none;
    flex-shrink: 0;
    display: block;
  }
  .education-item, .employment-item {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    padding: 0.55rem 0;
    margin-bottom: 0.4rem;
  }
  .institution-details {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .institution-details h3 {
    margin: 0 0 0.2rem 0;
    line-height: 1.2;
    color: var(--heading);
  }
  .institution-details .location,
  .institution-details .degree,
  .institution-details .date {
    line-height: 1.35;
    color: var(--muted);
  }

  /* ---------------- Presentations "chat" ---------------- */
  .presentations-chat {
    margin-top: 1rem;
    padding: 1.2rem 1.4rem;
    background: var(--surface-2);
    border-radius: 16px;
    border: 1px solid var(--border);
    max-width: 760px;
  }
  .presentations-chat .chat-bubble {
    background: var(--bubble);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 0.8rem 1rem;
    margin-bottom: 0.7rem;
    box-shadow: var(--shadow-sm);
    line-height: 1.5;
    color: var(--text);
  }
  .presentations-chat .chat-bubble:last-child { margin-bottom: 0; }
  .presentations-chat .chat-meta {
    display: block;
    font-size: 0.85em;
    color: var(--muted);
    margin-top: 0.3rem;
  }

  /* ---------------- Equal-contribution note ---------------- */
  .equal-contrib {
    font-size: 0.95em;
    font-weight: 600;
    color: var(--accent);
    margin-left: 2px;
    margin-right: 6px;
    vertical-align: super;
  }
  .equal-contrib-note {
    font-size: 0.98em;
    color: var(--muted);
    margin: 0.2em 0 0.8em 0;
    font-style: italic;
  }

  /* ---------------- Theme toggle (top-right) ---------------- */
  #theme-toggle {
    position: fixed !important;
    top: 0.8rem;
    right: 1rem;
    z-index: 9999;
    background: transparent;
  }
  #theme-toggle a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: var(--surface);
    border: 1px solid var(--border);
    box-shadow: var(--shadow-sm);
    cursor: pointer;
    transition: background-color .45s ease, border-color .45s ease,
                transform .2s ease, box-shadow .2s ease;
  }
  #theme-toggle a:hover { transform: scale(1.08); box-shadow: var(--shadow); }
  #theme-icon {
    color: var(--accent);
    transition: transform .5s cubic-bezier(.4, 0, .2, 1);
  }
  html[data-theme="dark"] #theme-icon { transform: rotate(360deg); }

  /* Hide redundant name occurrences: top-nav site title link and page H1 */
  .masthead__menu-item--lg { display: none !important; }
  .page__title { display: none !important; }

  /* ---------------- Subtle entrance animations ---------------- */
  @media (prefers-reduced-motion: no-preference) {
    .header, .section {
      animation: fadeUp .55s cubic-bezier(.4, 0, .2, 1) both;
    }
    .header    { animation-delay: .02s; }
    .section:nth-of-type(1) { animation-delay: .10s; }
    .section:nth-of-type(2) { animation-delay: .16s; }
    .section:nth-of-type(3) { animation-delay: .22s; }
    .section:nth-of-type(4) { animation-delay: .28s; }
    .section:nth-of-type(5) { animation-delay: .34s; }
  }
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(14px); }
    to   { opacity: 1; transform: none; }
  }

  /* ---------------- Responsive ---------------- */
  @media (max-width: 768px) {
    .header {
      flex-direction: column;
      text-align: center;
      padding: 1.4rem;
    }
    .profile-frame { width: 240px; height: 240px; }
    .social-links { justify-content: center; }
    .header-content h1 { font-size: 2rem; }
  }
</style>

<header class="header">
  <div class="profile-frame">
    <img src="images/profile_new_close_fur.jpg" alt="Portrait of Yurii Halychanskyi" class="profile-img profile-day">
    <img src="images/profile_new_close_fur_night.jpg" alt="" aria-hidden="true" class="profile-img profile-night">
  </div>
  <div class="header-content">
    <h1>Yurii Halychanskyi</h1>
    <div class="social-links">
      <a target="_blank" href="https://scholar.google.com/citations?user=Rcx5Jn8AAAAJ&hl=en" title="Google Scholar">
        <img src="images/Google_Scholar_logo.svg" width="28" height="28" alt="Google Scholar">
      </a>
      <a target="_blank" href="https://github.com/claussss" title="Github">
        <img src="images/Octicons-mark-github.svg" width="28" height="28" alt="GitHub" class="icon-mono">
      </a>
      <a target="_blank" href="https://www.linkedin.com/in/yurii-halychanskyi-a57590169/" title="LinkedIn">
        <img src="images/LinkedIn_icon.svg" width="28" height="28" alt="LinkedIn">
      </a>
      <a target="_blank" href="https://x.com/Yurii46278911?t=hmwTabK4xqQGbvtJNva-bg&s=09" title="Twitter">
        <img src="images/X_logo_2023_original.svg" width="28" height="28" alt="Twitter" class="icon-mono">
      </a>
    </div>
    <p class="email">yuriih2 [AT] illinois [DOT] edu</p>
  </div>
</header>

<section class="section">
  <h2 class="section-title">About Me</h2>
  <div class="about-item">
    <p>
      I am a PhD student at the <strong>University of Illinois Urbana-Champaign (UIUC)</strong>, co-advised by Volodymyr Kindratenko and Mark Hasegawa-Johnson.
      My research focuses on <strong>generative audio modeling</strong> for <strong>cross-domain conversion</strong>, including tasks such as timbre and accent transfer in low-resource or unsupervised settings.
    </p>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Publications</h2>

  <!-- Few-Shot Synthetic Accented Speech for ASR Fine-Tuning -->
  <div class="publication-card">
    <div class="publication-content">
      <div class="venue-row">
        <span class="venue-badge">Learning to Listen: ICML 2026 Workshop on ML for Audio</span>
        <span class="venue-badge oral">Oral</span>
      </div>
      <h3>Few-Shot Synthetic Accented Speech for ASR Fine-Tuning: What Helps and When?</h3>
      <p class="publication-authors"><strong class="author-me">Yurii Halychanskyi</strong>, Nimet Beyza Bozdag, Mark Hasegawa-Johnson, Dilek Hakkani-Tür, Volodymyr Kindratenko.</p>
      <div class="publication-links">
        <a href="https://arxiv.org/pdf/2604.27273">[Paper]</a>
        <a href="https://claussss.github.io/few_shot_accent_synthesis_demo" target="_blank" rel="noopener">[Demo]</a>
      </div>
    </div>
  </div>

  <!-- Accent Conversion Survey -->
  <div class="publication-card">
    <div class="publication-content">
      <div class="venue-row">
        <span class="venue-badge preprint">Preprint</span>
      </div>
      <h3>Accent Conversion: A Problem-Driven Survey of Sociolinguistic and Technical Constraints</h3>
      <p class="publication-authors"><strong class="author-me">Yurii Halychanskyi</strong>, Jianfeng Steven Guo, Volodymyr Kindratenko.</p>
      <div class="publication-links">
        <a href="https://arxiv.org/pdf/2604.27281">[Paper]</a>
      </div>
    </div>
  </div>

  <!-- FAC-FACodec -->
  <div class="publication-card">
    <div class="publication-content">
      <div class="venue-row">
        <span class="venue-badge">ICASSP 2026</span>
        <span class="venue-badge poster">Poster</span>
      </div>
      <h3>FAC-FACodec: Controllable Zero‑Shot Foreign Accent Conversion with Factorized Speech Codec</h3>
      <p class="publication-authors"><strong class="author-me">Yurii Halychanskyi</strong>, Cameron Churchwell, Yutong Wen, Volodymyr Kindratenko.</p>
      <div class="publication-links">
        <a href="https://arxiv.org/pdf/2510.10785">[Paper]</a>
        <a href="https://claussss.github.io/accent_control_demo/" target="_blank" rel="noopener">[Demo]</a>
      </div>
    </div>
  </div>

  <!-- Latent Diffusion Bridges for Unsupervised Musical Audio Timbre Transfer -->
  <div class="publication-card">
    <div class="publication-content">
      <div class="venue-row">
        <span class="venue-badge">ICASSP 2025</span>
        <span class="venue-badge poster">Poster</span>
      </div>
      <h3>Latent diffusion bridges for unsupervised musical audio timbre transfer</h3>
      <p class="publication-authors">
        Michele Mancusi<span class="equal-contrib" title="Equal contribution">*</span>, <strong class="author-me">Yurii Halychanskyi</strong><span class="equal-contrib" title="Equal contribution">*</span>, Kin Wai Cheuk, Eloi Moliner, Chieh-Hsin Lai, Stefan Uhlich, Junghyun Koo, Marco A Martínez-Ramírez, Wei-Hsiang Liao, Giorgio Fabbro, Yuki Mitsufuji.
      </p>
      <p class="equal-contrib-note"><span class="equal-contrib">*</span> Equal contribution</p>
      <div class="publication-links">
        <a href="https://arxiv.org/pdf/2409.06096" target="_blank" rel="noopener">[Paper]</a>
        <a href="https://sony.github.io/diffusion-timbre-transfer/" target="_blank" rel="noopener">[Demo]</a>
      </div>
    </div>
  </div>

</section>

<section class="section">
  <h2 class="section-title">Research Experience</h2>

  <div class="employment-grid">

    <div class="employment-item">
      <img src="images/logo_meta.webp" alt="Meta Logo" class="institution-logo">
      <div class="institution-details">
        <h3>Meta</h3>
        <div class="location">London, United Kingdom</div>
        <div class="degree">Research Scientist Intern</div>
        <div class="date">Summer 2026</div>
      </div>
    </div>

    <div class="employment-item">
      <img src="images/logo_sonyai.png" alt="Sony AI Logo" class="institution-logo">
      <div class="institution-details">
        <h3>Sony AI</h3>
        <div class="location">Tokyo, Japan</div>
        <div class="degree">Research Scientist Intern</div>
        <div class="date">Summer 2024</div>
      </div>
    </div>

    <div class="employment-item">
      <img src="images/logo_ml4sci.png" alt="ML4SCI Logo" class="institution-logo">
      <div class="institution-details">
        <h3>Machine Learning for Science (ML4SCI)</h3>
        <div class="location">Remote</div>
        <div class="degree">Research Scientist Intern (Google Summer of Code)</div>
        <div class="date">Summer 2021, Summer 2022</div>
      </div>
    </div>

  </div>
</section>

<section class="section">
  <h2 class="section-title">Education</h2>
  <div class="education-grid">

    <div class="education-item">
      <img src="images/logo_uiuc.jpg" alt="UIUC Logo" class="institution-logo">
      <div class="institution-details">
        <h3>University of Illinois Urbana‑Champaign</h3>
        <div class="location">Urbana, IL</div>
        <div class="degree">PhD in Computer Science</div>
        <div class="date">Aug 2023 – May 2028 (Expected)</div>
      </div>
    </div>

    <div class="education-item">
      <img src="images/logo_uw.png" alt="University of Washington Logo" class="institution-logo">
      <div class="institution-details">
        <h3>University of Washington</h3>
        <div class="location">Seattle, WA</div>
        <div class="degree">B.S. in Computer Science</div>
        <div class="date">2021 – 2023</div>
      </div>
    </div>

  </div>
</section>


<section class="section">
  <h2 class="section-title">Presentations</h2>
  <div class="presentations-chat">
    <div class="chat-bubble">
      Will present <strong>Few-Shot Synthetic Accented Speech for ASR Fine-Tuning: What Helps and When?</strong> at the <a href="https://mlforaudioworkshop.github.io/" target="_blank" rel="noopener">Learning to Listen: ICML 2026 Workshop on Machine Learning for Audio</a> in Seoul, Korea.
      <span class="chat-meta">Upcoming · July 10, 2026</span>
    </div>
    <div class="chat-bubble">
      Presented <strong>FAC-FACodec: Controllable Zero‑Shot Foreign Accent Conversion with Factorized Speech Codec</strong> at <strong>ICASSP 2026</strong> — session <em>SLP-P6: Neural Vocoders and Codecs</em>.
      <span class="chat-meta">Tuesday, May 5, 2026 · 14:00–16:00</span>
    </div>
    <div class="chat-bubble">
      Presented <strong>FAC-FACodec: Controllable Zero‑Shot Foreign Accent Conversion with Factorized Speech Codec</strong> at the 4th Annual NCSA Student Research Conference.
      <span class="chat-meta">April 23, 2026</span>
    </div>
    <div class="chat-bubble">
      Presented <strong>FAC-FACodec: Controllable Zero‑Shot Foreign Accent Conversion with Factorized Speech Codec</strong> and <strong>Few-Shot Synthetic Accented Speech for ASR Fine-Tuning: What Helps and When?</strong> at <a href="https://nlp.cs.illinois.edu/msld.html" target="_blank" rel="noopener">Midwest Speech and Language Days (MSLD) 2026</a>.
      <span class="chat-meta">April 15, 2026</span>
    </div>
  </div>
</section>


<!--
  Note: For best results, add the referenced images (profile, logos, icons) to your images/ directory.
  You can further style this page by adding a custom CSS file or inline <style> block.
-->
