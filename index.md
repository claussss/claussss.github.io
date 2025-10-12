---
layout: single
# Remove the title so it doesn't show above the profile card
permalink: /
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
    width: 200px; /* Change this value to adjust profile pic size */
    height: 200px; /* Change this value to adjust profile pic size */
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
</style>

<header class="header">
  <img src="images/profile.jpg" alt="Profile" class="profile-img">
  <div class="header-content">
    <h1>Yurii Halychanskyi</h1>
    <div class="social-links">
      <a target="_blank" href="https://scholar.google.com/citations?user=Rcx5Jn8AAAAJ&hl=en" title="Google Scholar">
        <img src="images/Google_Scholar_logo.svg" width="28" height="28" alt="Google Scholar">
      </a>
      <a target="_blank" href="https://github.com/Claussss" title="Github">
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
    <span class="about-emoji" aria-hidden="true">🎓</span>
    <p>
      I am a PhD student at the <strong>University of Illinois Urbana-Champaign (UIUC)</strong>, working on speech, accent conversion, and generative audio.
    </p>
  </div>
  <div class="about-item">
    <span class="about-emoji" aria-hidden="true">📚</span>
    <p>
      My research focuses on generative models for audio, speech processing, and accent conversion.
    </p>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Selected Publications</h2>
  <!-- Example publication card, add more as needed -->
  <div class="publication-card">
    <div class="publication-content">
      <h3>Title of Your Paper</h3>
      <p class="publication-authors"><strong class="author-me">Yurii Halychanskyi</strong>, Coauthor 1, Coauthor 2.</p>
      <p class="publication-venue">Conference/Journal, Year.</p>
      <div class="publication-links">
        <a href="#">[Abstract]</a>
        <a href="#">[Paper]</a>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Research Experience</h2>
  <div class="employment-grid">
    <div class="employment-item">
      <img src="images/logo_uiuc.jpg" alt="UIUC Logo" class="institution-logo">
      <div class="institution-details">
        <h3>University of Illinois Urbana-Champaign</h3>
        <div class="location">Urbana, IL</div>
        <div class="degree">PhD Student</div>
        <div class="date">2022 - Present</div>
      </div>
    </div>
    <!-- Add more employment items as needed -->
  </div>
</section>

<section class="section">
  <h2 class="section-title">Education</h2>
  <div class="education-grid">
    <div class="education-item">
      <img src="images/logo_uiuc.jpg" alt="UIUC Logo" class="institution-logo">
      <div class="institution-details">
        <h3>University of Illinois Urbana-Champaign</h3>
        <div class="location">Urbana, IL</div>
        <div class="degree">PhD in Computer Science</div>
        <div class="date">2022 - Present</div>
      </div>
    </div>
    <div class="education-item">
      <img src="images/logo_ntua.png" alt="NTUA Logo" class="institution-logo">
      <div class="institution-details">
        <h3>National Technical University of Athens</h3>
        <div class="location">Athens, Greece</div>
        <div class="degree">Diploma in Electrical and Computer Engineering</div>
        <div class="date">2016 - 2022</div>
      </div>
    </div>
  </div>
</section>

<footer>
  <p>Last updated in Oct. 2025.</p>
</footer>

<!--
  Note: For best results, add the referenced images (profile, logos, icons) to your images/ directory.
  You can further style this page by adding a custom CSS file or inline <style> block.
-->
