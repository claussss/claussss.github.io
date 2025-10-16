---
layout: single
permalink: /
title: "Yurii Halychanskyi"
description: "Yurii Halychanskyi — UIUC PhD student researching generative audio, speech, and accent conversion."
excerpt: "Yurii Halychanskyi is a PhD student at UIUC focusing on generative audio models, speech technology, and accent conversion."
last_modified_at: 2024-05-26
author: "Yurii Halychanskyi"
---

<style>
  .header {
    display: flex;
    gap: 2rem;
    margin-bottom: 2rem;
    padding: 2rem;
    background: white;
    border-radius: 12px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
    align-items: center;
  }
  .profile-img {
    width: 220px; /* Change this value to adjust profile pic size */
    height: 220px; /* Change this value to adjust profile pic size */
    object-fit: cover;
    object-position: center top; /* Shift the crop up to show more of the top part */
    border-radius: 12px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    margin-bottom: 0;
  }
  .header-content h1 {
    font-size: 2.2rem;
    margin-bottom: 0.5rem;
    color: #222;
    background: none;
    -webkit-background-clip: initial;
    -webkit-text-fill-color: initial;
    font-weight: 700;
  }
  .social-links {
    display: flex;
    gap: 1.2rem;
    margin-top: 0.7rem;
    margin-bottom: 0.7rem;
  }
  .social-links a {
    color: #666;
    text-decoration: none;
    font-size: 1.2rem;
    transition: color 0.2s;
  }
  .social-links a:hover {
    color: #2563eb;
  }
  .email {
    color: #2563eb;
    text-decoration: none;
    font-size: 1.1rem;
    margin-top: 0.5rem;
  }
  @media (max-width: 768px) {
    .header {
      flex-direction: column;
      padding: 1.2rem;
    }
    .profile-img {
      width: 120px;
      height: 120px;
    }
  }
  /* Hide day/night toggle if present */
  .dark-toggle, .js-dark-toggle, .color-mode-toggle, .color-mode, .site-header .site-nav .page-link[title*="Dark"], .site-header .site-nav .page-link[title*="Night"], .site-header .site-nav .page-link[title*="Light"] {
    display: none !important;
    visibility: hidden !important;
    pointer-events: none !important;
    height: 0 !important;
    width: 0 !important;
    min-width: 0 !important;
    min-height: 0 !important;
    max-width: 0 !important;
    max-height: 0 !important;
    overflow: hidden !important;
  }
  .equal-contrib {
    font-size: 0.95em;
    font-weight: 600;
    color: #2563eb;
    margin-left: 2px;
    margin-right: 6px;
    vertical-align: super;
  }
  .institution-logo {
    width: 60px;
    height: 60px;
    object-fit: contain;
    border-radius: 5px;
    margin-right: 1.2rem;
    margin-bottom: 0;
    background: none;
    flex-shrink: 0;
    display: block;
  }
  .education-item, .employment-item {
    display: flex;
    align-items: center;
    gap: 1.2rem;
    padding: 0.5rem 0 0.5rem 0;
    background: none;
    border-radius: 0;
    margin-bottom: 0.5rem;
    box-shadow: none;
  }
  .institution-details {
    flex: 1;
  }
  .equal-contrib-note {
    font-size: 0.98em;
    color: var(--text-normal, #444);
    margin: 0.2em 0 0.8em 0;
    font-style: italic;
    transition: color 0.2s;
  }
</style>

<header class="header">
  <img src="images/profile_final.jpg" alt="Portrait of Yurii Halychanskyi" class="profile-img">
  <div class="header-content">
    <h1>Yurii Halychanskyi</h1>
    <div class="social-links">
      <a target="_blank" href="https://scholar.google.com/citations?user=Rcx5Jn8AAAAJ&hl=en" title="Google Scholar">
        <img src="images/Google_Scholar_logo.svg" width="28" height="28" alt="Google Scholar">
      </a>
      <a target="_blank" href="https://github.com/claussss" title="Github">
        <img src="images/Octicons-mark-github.svg" width="28" height="28" alt="GitHub">
      </a>
      <a target="_blank" href="https://www.linkedin.com/in/yurii-halychanskyi-a57590169/" title="LinkedIn">
        <img src="images/LinkedIn_icon.svg" width="28" height="28" alt="LinkedIn">
      </a>
      <a target="_blank" href="https://x.com/Yurii46278911?t=hmwTabK4xqQGbvtJNva-bg&s=09" title="Twitter">
        <img src="images/X_logo_2023_original.svg" width="28" height="28" alt="Twitter">
      </a>
    </div>
    <p class="email">yuriih2 [AT] illinois [DOT] edu</p>
  </div>
</header>

<section class="section">
  <h2 class="section-title">About Me</h2>
  <div class="about-item">
    <p>
      I am a PhD student at the <strong>University of Illinois Urbana-Champaign (UIUC)</strong>, advised by Volodymyr Kindratenko.
      My research focuses on <strong>generative audio modeling</strong> for <strong>cross-domain conversion</strong>, including tasks such as timbre and accent transfer in low-resource or unsupervised settings.
    </p>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Publications</h2>

  <!-- FAC-FACodec -->
  <div class="publication-card">
    <div class="publication-content">
      <h3>FAC-FACodec: Controllable Zero‑Shot Foreign Accent Conversion with Factorized Speech Codec</h3>
      <p class="publication-authors"><strong class="author-me">Yurii Halychanskyi</strong>, Cameron Churchwell, Yutong Wen, Volodymyr Kindratenko.</p>
      <div class="publication-links">
        <a href="https://arxiv.org/abs/2510.10785">[Abstract]</a>
        <a href="https://arxiv.org/pdf/2510.10785">[Paper]</a>
      </div>
    </div>
  </div>

  <!-- Latent Diffusion Bridges for Unsupervised Musical Audio Timbre Transfer -->
  <div class="publication-card">
    <div class="publication-content">
      <h3>Latent diffusion bridges for unsupervised musical audio timbre transfer</h3>
      <p class="publication-authors">
        Michele Mancusi<span class="equal-contrib" title="Equal contribution">*</span>, <strong class="author-me">Yurii Halychanskyi</strong><span class="equal-contrib" title="Equal contribution">*</span>, Kin Wai Cheuk, Eloi Moliner, Chieh-Hsin Lai, Stefan Uhlich, Junghyun Koo, Marco A Martínez-Ramírez, Wei-Hsiang Liao, Giorgio Fabbro, Yuki Mitsufuji.
      </p>
      <p class="equal-contrib-note"><span class="equal-contrib">*</span> Equal contribution</p>
      <p class="publication-venue">IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2025.</p>
      <div class="publication-links">
        <a href="https://arxiv.org/abs/2409.06096">[Abstract]</a>
        <a href="https://arxiv.org/pdf/2409.06096" target="_blank" rel="noopener">[Paper]</a>
      </div>
    </div>
  </div>

</section>

<section class="section">
  <h2 class="section-title">Research Experience</h2>

  <div class="employment-grid">

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


<!--
  Note: For best results, add the referenced images (profile, logos, icons) to your images/ directory.
  You can further style this page by adding a custom CSS file or inline <style> block.
-->
