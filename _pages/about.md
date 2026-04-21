---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  :root {
    --bg: #f7f9fc;
    --panel: rgba(255, 255, 255, 0.9);
    --panel-strong: #ffffff;
    --text: #1f2937;
    --muted: #667085;
    --title: #0f172a;
    --line: #e6ebf2;
    --line-strong: #dbe5f0;
    --accent: #245b92;
    --accent-2: #5a89b6;
    --accent-3: #8fb2d1;
    --accent-soft: #eef5fb;
    --shadow-xs: 0 2px 8px rgba(15, 23, 42, 0.04);
    --shadow-sm: 0 8px 24px rgba(15, 23, 42, 0.06);
    --shadow: 0 14px 36px rgba(15, 23, 42, 0.08);
    --shadow-lg: 0 22px 52px rgba(15, 23, 42, 0.12);
    --radius: 22px;
    --radius-sm: 16px;
    --maxw: 1120px;
  }

  html {
    font-size: 15px;
    scroll-behavior: smooth;
  }

  body {
    font-family: "Inter", "Segoe UI", Arial, sans-serif;
    color: var(--text);
    background:
      radial-gradient(circle at top right, rgba(79, 134, 186, 0.10), transparent 20%),
      radial-gradient(circle at left top, rgba(36, 91, 146, 0.05), transparent 22%),
      linear-gradient(180deg, #fbfcfe 0%, #f7f9fc 100%);
    line-height: 1.78;
    letter-spacing: 0.01em;
    text-rendering: optimizeLegibility;
  }

  .page,
  .page__content,
  .archive {
    max-width: var(--maxw);
  }

  .page__content {
    padding-bottom: 2.4rem;
  }

  p, span, li, div {
    font-size: 0.97rem;
  }

  p {
    margin-bottom: 0.95rem;
  }

  a {
    color: var(--accent);
    text-decoration: none;
    transition: color 0.22s ease, border-color 0.22s ease, background 0.22s ease, box-shadow 0.22s ease, transform 0.22s ease;
  }

  a:hover {
    color: #173f67;
  }

  .page__content a:not(.pub-btn):not(.news-btn):not(.hero-chip) {
    border-bottom: 1px solid rgba(36, 91, 146, 0.16);
  }

  .page__content a:not(.pub-btn):not(.news-btn):not(.hero-chip):hover {
    border-bottom-color: rgba(36, 91, 146, 0.38);
  }

  .sidebar .author__avatar img,
  .author__avatar img {
    border-radius: 22px !important;
    box-shadow: var(--shadow-sm);
  }

  .sidebar .author__content,
  .author__content {
    padding: 0.15rem 0.1rem 0 !important;
  }

  .sidebar .author__name,
  .author__name {
    font-size: 1.18rem !important;
    line-height: 1.28 !important;
    font-weight: 800 !important;
    color: var(--title) !important;
    margin-top: 0.46rem !important;
    margin-bottom: 0.72rem !important;
    letter-spacing: -0.01em;
  }

  .sidebar .author__bio,
  .author__bio {
    font-size: 0.96rem !important;
    line-height: 1.72 !important;
    color: var(--text) !important;
    margin-bottom: 0.82rem !important;
  }

  .sidebar .author__pronouns,
  .author__pronouns {
    font-size: 0.92rem !important;
    line-height: 1.58 !important;
    color: var(--muted) !important;
    margin-bottom: 0.78rem !important;
  }

  .sidebar .author__urls-wrapper,
  .author__urls-wrapper {
    margin-top: 0.9rem !important;
  }

  .sidebar .author__urls,
  .author__urls {
    margin-top: 0.25rem !important;
    padding-top: 0.2rem !important;
  }

  .sidebar .author__urls li,
  .author__urls li {
    font-size: 0.93rem !important;
    line-height: 1.65 !important;
    margin-bottom: 0.52rem !important;
  }

  .sidebar .author__urls a,
  .author__urls a {
    font-size: 0.93rem !important;
    color: var(--text) !important;
    border-bottom: none !important;
  }

  .sidebar .author__urls a:hover,
  .author__urls a:hover {
    color: var(--accent) !important;
  }

  .sidebar .author__urls i,
  .author__urls i,
  .sidebar .author__urls svg,
  .author__urls svg {
    font-size: 0.94rem !important;
    width: 0.96rem !important;
    color: var(--accent) !important;
  }

  h3 {
    position: relative;
    margin: 3.35rem 0 1.2rem;
    padding: 0 0 0.95rem 1.05rem;
    font-size: 1.16rem;
    font-weight: 800;
    color: var(--title);
    letter-spacing: 0.01em;
    border-bottom: 1px solid var(--line);
    scroll-margin-top: 96px;
  }

  h3::before {
    content: '';
    position: absolute;
    left: 0;
    top: 0.22rem;
    width: 4px;
    height: 1.1rem;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--accent) 0%, var(--accent-2) 100%);
    box-shadow: 0 6px 14px rgba(36, 91, 146, 0.24);
  }

  strong {
    font-weight: 700;
  }

  .page-intro,
  .section-note {
    color: var(--muted);
    font-size: 0.91rem;
    line-height: 1.72;
    margin-top: -0.1rem;
    margin-bottom: 1.05rem;
    max-width: 860px;
  }

  .hero {
    position: relative;
    display: grid;
    grid-template-columns: minmax(0, 1fr) 230px;
    gap: 1.8rem;
    align-items: center;
    padding: 1.7rem 1.75rem;
    background:
      radial-gradient(circle at top right, rgba(79, 134, 186, 0.14), transparent 28%),
      linear-gradient(180deg, rgba(255,255,255,0.98) 0%, rgba(247,250,253,0.98) 100%);
    border: 1px solid rgba(36, 91, 146, 0.10);
    border-radius: 28px;
    box-shadow: var(--shadow);
    overflow: hidden;
    isolation: isolate;
  }

  .hero::before {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, rgba(255,255,255,0.42), transparent 42%);
    pointer-events: none;
    z-index: -1;
  }

  .hero::after {
    content: '';
    position: absolute;
    inset: auto 0 0 0;
    height: 3px;
    background: linear-gradient(90deg, rgba(36, 91, 146, 0.95), rgba(79, 134, 186, 0.38), rgba(255, 255, 255, 0));
  }

  .hero-text {
    min-width: 0;
  }

  .hero-text p {
    margin: 0;
    text-align: left;
    font-size: 1rem;
    line-height: 1.86;
  }

  .hero-links {
    margin-top: 1.1rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.68rem;
  }

  .hero-chip {
    display: inline-flex;
    align-items: center;
    padding: 0.42rem 0.86rem;
    border: 1px solid #d8e5f1;
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.94);
    color: var(--accent);
    font-size: 0.81rem;
    font-weight: 800;
    white-space: nowrap;
    box-shadow: var(--shadow-xs);
  }

  .hero-chip:hover {
    transform: translateY(-1px);
    box-shadow: var(--shadow-sm);
  }

  .logo-panel {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.95rem;
    align-items: stretch;
    justify-items: stretch;
    width: 100%;
    min-width: 0;
  }

  .logo-panel a {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 114px;
    width: 100%;
    min-width: 0;
    padding: 1rem 1.1rem;
    background: rgba(255, 255, 255, 0.92);
    border: 1px solid var(--line);
    border-radius: 18px;
    box-shadow: var(--shadow-xs);
    box-sizing: border-box;
    overflow: hidden;
  }

  .logo-panel a:first-child {
    grid-column: 1 / -1;
    min-height: 128px;
  }

  .logo-panel a:hover {
    transform: translateY(-2px);
    box-shadow: var(--shadow-sm);
    border-color: var(--line-strong);
  }

  .logo-panel img {
    display: block;
    width: auto;
    max-width: 100%;
    max-height: 76px;
    object-fit: contain;
    opacity: 0.97;
  }

  .logo-panel a:first-child img {
    max-height: 82px;
  }

  .news-box,
  .stats-card,
  .info-card,
  .contact-card,
  .pub-card,
  .stats-summary-card {
    backdrop-filter: blur(8px);
  }

  .news-box {
    border: 1px solid var(--line);
    border-radius: 24px;
    background: linear-gradient(180deg, rgba(255,255,255,0.98) 0%, rgba(251,253,255,0.98) 100%);
    overflow: hidden;
    box-shadow: var(--shadow-sm);
  }

  .news-list {
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .news-item {
    display: grid;
    grid-template-columns: 98px minmax(0, 1fr);
    gap: 1rem;
    padding: 1.08rem 1.14rem;
    border-bottom: 1px solid var(--line);
    align-items: start;
    transition: background 0.2s ease, transform 0.2s ease;
  }

  .news-item:hover {
    background: linear-gradient(180deg, #fbfdff 0%, #f7fbff 100%);
  }

  .news-list .news-item:last-child {
    border-bottom: none;
  }

  .news-date {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: fit-content;
    min-width: 78px;
    padding: 0.3rem 0.58rem;
    border-radius: 999px;
    background: linear-gradient(180deg, #f3f8fd 0%, #ebf3fa 100%);
    border: 1px solid #d8e5f1;
    font-size: 0.78rem;
    font-weight: 800;
    color: var(--accent);
    letter-spacing: 0.03em;
    box-shadow: inset 0 1px 0 rgba(255,255,255,0.7);
  }

  .news-content {
    color: var(--text);
    line-height: 1.76;
  }

  .news-links {
    display: inline-flex;
    flex-wrap: wrap;
    gap: 0.48rem;
    margin-left: 0.58rem;
    vertical-align: middle;
  }

  .news-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.32rem;
    padding: 0.3rem 0.66rem;
    border-radius: 999px;
    border: 1px solid #d7e3ef;
    background: #fff;
    color: var(--accent);
    font-size: 0.78rem;
    font-weight: 700;
    line-height: 1.2;
    text-decoration: none !important;
    box-shadow: var(--shadow-xs);
  }

  .news-btn:hover {
    background: var(--accent-soft);
    border-color: #bfd3e6;
    color: #163f64;
    text-decoration: none !important;
    transform: translateY(-1px);
  }

  .news-btn.secondary {
    color: #475467;
    border-color: #e4e7ec;
  }

  .news-btn.secondary:hover {
    background: #f8fafc;
    color: #344054;
  }

  .news-pagination {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 0.75rem;
    padding: 0.9rem 1rem;
    border-top: 1px solid var(--line);
    background: linear-gradient(180deg, #fcfdff 0%, #f7f9fc 100%);
  }

  .news-page-info {
    color: var(--muted);
    font-size: 0.86rem;
  }

  .news-pagination-buttons {
    display: inline-flex;
    gap: 0.5rem;
  }

  .news-page-btn {
    appearance: none;
    border: 1px solid var(--line);
    background: #fff;
    color: var(--text);
    border-radius: 12px;
    padding: 0.38rem 0.78rem;
    font-size: 0.84rem;
    font-weight: 700;
    line-height: 1.2;
    cursor: pointer;
    transition: background 0.18s ease, color 0.18s ease, border-color 0.18s ease, transform 0.18s ease;
  }

  .news-page-btn:hover:not(:disabled) {
    background: var(--accent-soft);
    border-color: #d6e2ef;
    transform: translateY(-1px);
  }

  .news-page-btn:disabled {
    opacity: 0.45;
    cursor: not-allowed;
  }

  .stats-wrap {
    display: grid;
    grid-template-columns: 1.05fr 0.95fr;
    gap: 1rem;
    align-items: stretch;
  }

  .stats-card {
    border: 1px solid var(--line);
    border-radius: 24px;
    background: linear-gradient(180deg, rgba(255,255,255,0.98) 0%, rgba(251,253,255,0.98) 100%);
    padding: 1.1rem 0.9rem;
    box-shadow: var(--shadow-sm);
    overflow: visible;
    position: relative;
  }

  .stats-card-head-top {
    text-align: center;
    margin-bottom: 0.2rem;
  }

  .stats-card-head-top .stats-card-title {
    font-size: 1rem;
    font-weight: 800;
    color: var(--title);
    line-height: 1.3;
  }

  .stats-card-head-top .stats-card-subtitle {
    margin-top: 0.22rem;
    font-size: 0.8rem;
    color: var(--muted);
    line-height: 1.4;
  }

  .stats-chart {
    width: min(100%, 420px);
    height: 340px;
    margin: 0.1rem auto 0;
    flex: 0 0 auto;
    overflow: visible;
  }

  .stats-summary-card {
    position: relative;
    padding: 1.15rem 1rem 1rem;
    overflow: hidden;
    border: 1px solid var(--line);
    border-radius: 24px;
    background: linear-gradient(180deg, rgba(255,255,255,0.98) 0%, rgba(251,253,255,0.98) 100%);
    box-shadow: var(--shadow-sm);
  }

  .stats-metric-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.72rem;
  }

  .stats-metric-item {
    padding: 0.9rem 0.9rem 0.82rem;
    border: 1px solid var(--line);
    border-radius: 18px;
    background: rgba(255,255,255,0.86);
    box-shadow: inset 0 1px 0 rgba(255,255,255,0.72);
    text-align: center;
  }

  .stats-metric-label {
    display: block;
    margin-bottom: 0.3rem;
    font-size: 0.74rem;
    font-weight: 700;
    color: var(--muted);
    letter-spacing: 0.03em;
    text-transform: uppercase;
  }

  .stats-metric-value {
    display: block;
    font-size: 1.14rem;
    font-weight: 800;
    color: var(--title);
    line-height: 1.1;
  }

  .subheading {
    margin: 1.65rem 0 0.95rem;
    font-size: 1rem;
    font-weight: 800;
    color: var(--title);
    display: flex;
    align-items: center;
    gap: 0.58rem;
  }

  .subheading::before {
    content: '';
    width: 4px;
    height: 1rem;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--accent) 0%, #7fa1c0 100%);
    box-shadow: 0 6px 12px rgba(36,91,146,0.18);
  }

  .pub-list {
    display: grid;
    gap: 1.08rem;
  }

  .pub-card {
    display: grid;
    grid-template-columns: 188px minmax(0, 1fr);
    gap: 1.08rem;
    padding: 1.08rem;
    background: linear-gradient(180deg, rgba(255,255,255,0.98) 0%, rgba(251,253,255,0.98) 100%);
    border: 1px solid var(--line);
    border-radius: 24px;
    align-items: start;
    box-shadow: var(--shadow-sm);
    transition: transform 0.22s ease, box-shadow 0.22s ease, border-color 0.22s ease;
  }

  .pub-card:hover {
    transform: translateY(-3px);
    border-color: var(--line-strong);
    box-shadow: var(--shadow);
  }

  .pub-thumb {
    position: relative;
    border-radius: 18px;
    overflow: hidden;
    background: linear-gradient(180deg, #fbfcfd 0%, #f5f8fb 100%);
    border: 1px solid var(--line);
    height: 138px;
    padding: 0.8rem;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .pub-thumb img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: contain;
    border-radius: 8px;
  }

  .paper-badge {
    position: absolute;
    top: 10px;
    left: 10px;
    padding: 0.2rem 0.52rem;
    border-radius: 999px;
    background: rgba(15, 23, 42, 0.84);
    color: #fff;
    font-size: 0.68rem;
    font-weight: 800;
    letter-spacing: 0.02em;
    box-shadow: 0 4px 10px rgba(15, 23, 42, 0.16);
  }

  .pub-meta {
    margin-bottom: 0.42rem;
    color: var(--accent);
    font-size: 0.82rem;
    font-weight: 800;
  }

  .pub-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-bottom: 0.6rem;
  }

  .pub-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.24rem 0.6rem;
    border-radius: 999px;
    background: var(--accent-soft);
    border: 1px solid #d8e4f0;
    color: var(--accent);
    font-size: 0.73rem;
    font-weight: 800;
    letter-spacing: 0.01em;
  }

  .pub-title {
    margin: 0 0 0.45rem;
    color: var(--title);
    font-size: 1.02rem;
    line-height: 1.48;
    font-weight: 800;
  }

  .pub-authors {
    color: var(--muted);
    line-height: 1.72;
    margin-bottom: 0.8rem;
  }

  .pub-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.52rem;
    margin-top: 0.12rem;
  }

  .pub-btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.28rem;
    min-width: 94px;
    padding: 0.36rem 0.74rem;
    border-radius: 999px;
    border: 1px solid #d7e3ef;
    background: #f8fbfe;
    color: var(--accent);
    font-size: 0.78rem;
    font-weight: 700;
    line-height: 1.15;
    text-decoration: none !important;
    box-shadow: var(--shadow-xs);
  }

  .pub-btn:hover {
    background: var(--accent-soft);
    border-color: #bfd3e6;
    color: #163f64;
    text-decoration: none !important;
    transform: translateY(-1px);
  }

  .pub-btn.secondary {
    background: #ffffff;
    color: #475467;
    border-color: #d9e1ea;
  }

  .pub-btn.secondary:hover {
    background: #f8fafc;
    color: #344054;
    border-color: #cfd8e3;
  }

  .two-col-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
  }

  .info-card,
  .contact-card {
    border: 1px solid var(--line);
    border-radius: var(--radius);
    background: linear-gradient(180deg, rgba(255,255,255,0.98) 0%, rgba(251,253,255,0.98) 100%);
    padding: 1.08rem 1.12rem;
    box-shadow: 0 6px 18px rgba(15, 23, 42, 0.045);
  }

  .info-card h4 {
    margin: 0 0 0.74rem;
    font-size: 0.93rem;
    color: var(--title);
  }

  .info-card ul {
    margin: 0;
    padding-left: 1.15rem;
  }

  .info-card li {
    margin-bottom: 0.52rem;
    color: var(--text);
  }

  .map-shell {
    margin: 1rem auto 0;
    border: 1px solid var(--line);
    border-radius: 16px;
    overflow: hidden;
    background: #fff;
    max-width: 320px;
    box-shadow: inset 0 1px 0 rgba(255,255,255,0.8);
  }

  .map-shell > div {
    max-height: 280px;
    overflow: hidden;
  }

  .compact-list {
    margin-top: 0.42rem;
  }

  .compact-list li {
    margin-bottom: 0.44rem;
  }

  .greedy-nav button {
    display: none !important;
  }

  @media (max-width: 900px) {
    .hero,
    .pub-card,
    .two-col-grid,
    .stats-wrap {
      grid-template-columns: 1fr;
    }

    .hero {
      padding: 1.28rem 1.22rem;
    }

    .logo-panel {
      justify-items: stretch;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 0.85rem;
    }

    .logo-panel a:first-child {
      grid-column: auto;
    }
  }

  @media (max-width: 640px) {
    html {
      font-size: 14px;
    }

    .page__content {
      padding-bottom: 1.4rem;
    }

    .sidebar .author__name,
    .author__name {
      font-size: 1.05rem !important;
    }

    .sidebar .author__bio,
    .author__bio,
    .sidebar .author__pronouns,
    .author__pronouns,
    .sidebar .author__urls li,
    .author__urls li,
    .sidebar .author__urls a,
    .author__urls a {
      font-size: 0.91rem !important;
    }

    h3 {
      margin-top: 2.5rem;
      padding-left: 0.88rem;
    }

    .hero,
    .stats-card,
    .stats-summary-card,
    .info-card,
    .contact-card,
    .pub-card {
      padding: 0.95rem;
    }

    .news-item {
      grid-template-columns: 1fr;
      gap: 0.48rem;
    }

    .news-links {
      margin-left: 0;
      margin-top: 0.48rem;
    }

    .pub-thumb {
      height: 154px;
      padding: 0.76rem;
    }

    .pub-thumb img {
      width: 100%;
      height: 100%;
      max-height: none;
      object-fit: contain;
    }

    .stats-chart {
      width: min(100%, 320px);
      height: 300px;
    }

    .stats-metric-grid {
      gap: 0.62rem;
    }

    .stats-metric-item {
      padding: 0.8rem 0.78rem 0.74rem;
    }

    .stats-metric-value {
      font-size: 1.02rem;
    }
  }
</style>

### 👨‍🎓 Profile

<div class="hero">
  <div class="hero-text">
    <p>
      I am currently a Ph.D. student at Southeast University, under the supervision of
      <a href="https://jyh-learning.github.io"><strong>Prof. Yuheng Jia</strong></a>.
      I received my M.S. degree from Henan University in 2023, under the supervision of
      <a href="https://cs.henu.edu.cn/info/1273/5566.htm"><strong>Prof. Chongsheng Zhang</strong></a>.
      Before that, I obtained my B.S. degree in 2020 from Henan Institute of Engineering.
      My research interests lie in machine learning, with a focus on long-tailed learning and weakly supervised learning.
    </p>
    <div class="hero-links">
      <span class="hero-chip">Machine Learning</span>
      <span class="hero-chip">Long-Tailed Learning</span>
      <span class="hero-chip">Weakly Supervised Learning</span>
    </div>
  </div>

  <div class="logo-panel">
    <a href="https://www.seu.edu.cn" target="_blank">
      <img src="./images/SEU.svg" alt="Southeast University" title="Southeast University">
    </a>
    <a href="https://cse.seu.edu.cn" target="_blank">
      <img src="./images/CS.png" alt="School of Computer Science and Engineering" title="School of Computer Science and Engineering">
    </a>
    <a href="https://www.palmlab.cn" target="_blank">
      <img src="./images/PALM.png" alt="Pattern Learning and Mining Lab" title="Pattern Learning and Mining Lab">
    </a>
  </div>
</div>

### 🔥 News

<div class="news-box">
  <ul class="news-list" id="news-list">
    <li class="news-item">
      <div class="news-date">2026.01</div>
      <div class="news-content">🎉 Our work “Samples Are Not Equal: A Sample Selection Approach for Deep Clustering” is accepted by ICLR 2026.<span class="news-links"><a class="news-btn" href="https://iclr.cc/virtual/2026/poster/10009380" target="_blank">📄 Paper</a><a class="news-btn secondary" href="https://github.com/notoaudrey/Samples-Are-Not-Equal" target="_blank">💻 Code</a></span></div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.11</div>
      <div class="news-content">🎉 Our work “DiCaP: Distribution-Calibrated Pseudo-labeling for Semi-Supervised Multi-Label Learning” is accepted by AAAI 2026.<span class="news-links"><a class="news-btn" href="https://ojs.aaai.org/index.php/AAAI/article/view/39302" target="_blank">📄 Paper</a><a class="news-btn secondary" href="https://github.com/hb-studying/DiCaP" target="_blank">💻 Code</a></span></div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.10</div>
      <div class="news-content">🎉 Received the National Scholarship for Ph.D. students.</div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.09</div>
      <div class="news-content">🎉 Our work “Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning” is accepted by NeurIPS 2025.<span class="news-links"><a class="news-btn" href="https://neurips.cc/virtual/2025/loc/san-diego/poster/116160" target="_blank">📄 Paper</a><a class="news-btn secondary" href="https://github.com/YaxinHou/CPG" target="_blank">💻 Code</a></span></div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.05</div>
      <div class="news-content">🎉 Our work “A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning” is accepted by ICML 2025.<span class="news-links"><a class="news-btn" href="https://icml.cc/virtual/2025/poster/44441" target="_blank">📄 Paper</a><a class="news-btn secondary" href="https://github.com/YaxinHou/Meta-Expert" target="_blank">💻 Code</a></span></div>
    </li>
  </ul>

  <div class="news-pagination">
    <div class="news-page-info" id="news-page-info"></div>
    <div class="news-pagination-buttons">
      <button class="news-page-btn" id="news-prev" type="button">Prev</button>
      <button class="news-page-btn" id="news-next" type="button">Next</button>
    </div>
  </div>
</div>

<script>
  (function () {
    const list = document.getElementById('news-list');
    const prevBtn = document.getElementById('news-prev');
    const nextBtn = document.getElementById('news-next');
    const pageInfo = document.getElementById('news-page-info');
    if (!list || !prevBtn || !nextBtn || !pageInfo) return;

    const items = Array.from(list.querySelectorAll('.news-item'));
    const perPage = 3;
    const totalPages = Math.max(1, Math.ceil(items.length / perPage));
    let currentPage = 1;

    function renderNewsPage(page) {
      currentPage = Math.min(Math.max(page, 1), totalPages);
      const start = (currentPage - 1) * perPage;
      const end = start + perPage;

      items.forEach((item, index) => {
        item.style.display = index >= start && index < end ? 'grid' : 'none';
      });

      pageInfo.textContent = `Page ${currentPage} / ${totalPages}`;
      prevBtn.disabled = currentPage === 1;
      nextBtn.disabled = currentPage === totalPages;
    }

    prevBtn.addEventListener('click', function () {
      renderNewsPage(currentPage - 1);
    });

    nextBtn.addEventListener('click', function () {
      renderNewsPage(currentPage + 1);
    });

    renderNewsPage(1);
  })();
</script>

### 📊 Publication Statistics

<div class="stats-wrap">
  <div class="stats-card">
    <div class="stats-card-head stats-card-head-top">
      <div class="stats-card-title">Papers</div>
      <div class="stats-card-subtitle">By venue</div>
    </div>
    <div id="all-papers-chart" class="stats-chart"></div>
  </div>

  <div class="stats-summary-card">
    <div class="stats-card-head stats-card-head-top">
      <div class="stats-card-title">Statistics</div>
      <div class="stats-card-subtitle">Publication overview</div>
    </div>

    <div class="stats-metric-grid">
      <div class="stats-metric-item">
        <span class="stats-metric-label">CCF A</span>
        <span class="stats-metric-value">5</span>
      </div>
      <div class="stats-metric-item">
        <span class="stats-metric-label">CCF B</span>
        <span class="stats-metric-value">1</span>
      </div>
      <div class="stats-metric-item">
        <span class="stats-metric-label">Conference</span>
        <span class="stats-metric-value">5</span>
      </div>
      <div class="stats-metric-item">
        <span class="stats-metric-label">Journal</span>
        <span class="stats-metric-value">1</span>
      </div>
    </div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/echarts@5/dist/echarts.min.js"></script>
<script>
  const allPapersChart = echarts.init(
    document.getElementById('all-papers-chart'),
    null,
    { renderer: 'svg' }
  );

  const allPapersData = [
    { value: 1, name: 'ICLR' },
    { value: 1, name: 'NeurIPS' },
    { value: 1, name: 'ICML' },
    { value: 2, name: 'AAAI' },
    { value: 1, name: 'Inf. Sci.' }
  ];

  function buildPieOption() {
    const isMobile = window.innerWidth <= 768;

    return {
      tooltip: {
        trigger: 'item',
        formatter: '{b}: {c} ({d}%)',
        backgroundColor: 'rgba(255,255,255,0.98)',
        borderColor: '#e7ebf0',
        borderWidth: 1,
        textStyle: {
          color: '#1f2328',
          fontFamily: 'Inter, Arial, sans-serif'
        }
      },
      color: ['#2f5f8f', '#4f7aa6', '#7b9bbb', '#b7c8d9', '#d7e2ec'],
      legend: {
        bottom: 4,
        left: 'center',
        icon: 'circle',
        itemWidth: 9,
        itemHeight: 9,
        itemGap: isMobile ? 12 : 16,
        textStyle: {
          color: '#4b5563',
          fontSize: isMobile ? 11 : 12,
          fontFamily: 'Inter, Arial, sans-serif'
        }
      },
      graphic: [
        {
          type: 'text',
          left: 'center',
          top: '54%',
          style: {
            text: '6',
            textAlign: 'center',
            textVerticalAlign: 'middle',
            fill: '#0f172a',
            fontSize: isMobile ? 28 : 34,
            fontWeight: 800,
            fontFamily: 'Inter, Arial, sans-serif'
          }
        }
      ],
      series: [
        {
          type: 'pie',
          radius: isMobile ? ['50%', '72%'] : ['58%', '82%'],
          center: ['50%', '54%'],
          minAngle: 8,
          avoidLabelOverlap: true,
          itemStyle: {
            borderColor: '#ffffff',
            borderWidth: 3,
            shadowBlur: 8,
            shadowColor: 'rgba(15, 23, 42, 0.05)'
          },
          label: {
            color: '#475467',
            fontSize: isMobile ? 10 : 11,
            fontWeight: 600,
            formatter: isMobile ? '{b}\n{c}' : '{b}: {c}',
            width: isMobile ? 52 : 76,
            overflow: 'break'
          },
          labelLine: {
            length: isMobile ? 6 : 8,
            length2: isMobile ? 6 : 9,
            maxSurfaceAngle: 80,
            lineStyle: {
              color: '#cbd5e1'
            }
          },
          emphasis: {
            scale: true,
            scaleSize: 4
          },
          data: allPapersData
        }
      ]
    };
  }

  function renderCharts() {
    allPapersChart.setOption(buildPieOption(), true);
    allPapersChart.resize();
  }

  renderCharts();

  if (typeof ResizeObserver !== 'undefined') {
    const resizeObserver = new ResizeObserver(function () {
      allPapersChart.resize();
    });

    const chartEl = document.getElementById('all-papers-chart');
    if (chartEl) resizeObserver.observe(chartEl);
  } else {
    let resizeTimer = null;
    window.addEventListener('resize', function () {
      clearTimeout(resizeTimer);
      resizeTimer = setTimeout(function () {
        allPapersChart.resize();
      }, 120);
    });
  }
</script>

### 📝 Publications

<div class="section-note">
  Papers are listed in descending order by year of publication. For a full list, please visit my <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=-0IuShsAAAAJ">Google Scholar</a> page.
</div>

<div class="subheading">Conference Papers</div>
<div class="pub-list">
  <div class="pub-card">
    <div class="pub-thumb">
      <div class="paper-badge">CCF A</div>
      <img src="./images/CPG.png" alt="Publication Image">
    </div>
    <div>
      <div class="pub-tags"><span class="pub-tag">Conference</span><span class="pub-tag">CCF A</span><span class="pub-tag">2025</span></div>
      <div class="pub-meta">Annual Conference on Neural Information Processing Systems (NeurIPS), 2025.</div>
      <div class="pub-title">Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning.</div>
      <div class="pub-authors"><strong style="color:#111827;">Yaxin Hou</strong>, Bo Han, Yuheng Jia, Hui Liu, Junhui Hou.</div>
      <div class="pub-links">
        <a class="pub-btn" href="https://neurips.cc/virtual/2025/loc/san-diego/poster/116160" target="_blank">📄 Paper</a>
        <a class="pub-btn secondary" href="https://github.com/YaxinHou/CPG" target="_blank">💻 Code</a>
      </div>
    </div>
  </div>

  <div class="pub-card">
    <div class="pub-thumb">
      <div class="paper-badge">CCF A</div>
      <img src="./images/Meta-Expert.png" alt="Publication Image">
    </div>
    <div>
      <div class="pub-tags"><span class="pub-tag">Conference</span><span class="pub-tag">CCF A</span><span class="pub-tag">2025</span></div>
      <div class="pub-meta">International Conference on Machine Learning (ICML), 2025.</div>
      <div class="pub-title">A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning.</div>
      <div class="pub-authors"><strong style="color:#111827;">Yaxin Hou</strong>, Yuheng Jia.</div>
      <div class="pub-links">
        <a class="pub-btn" href="https://icml.cc/virtual/2025/poster/44441" target="_blank">📄 Paper</a>
        <a class="pub-btn secondary" href="https://github.com/YaxinHou/Meta-Expert" target="_blank">💻 Code</a>
      </div>
    </div>
  </div>

  <div class="pub-card">
    <div class="pub-thumb">
      <div class="paper-badge">CCF A</div>
      <img src="./images/QAST.png" alt="Publication Image">
    </div>
    <div>
      <div class="pub-tags"><span class="pub-tag">Conference</span><span class="pub-tag">CCF A</span><span class="pub-tag">2023</span></div>
      <div class="pub-meta">AAAI Conference on Artificial Intelligence (AAAI), 2023.</div>
      <div class="pub-title">Quality-Aware Self-Training on Differentiable Synthesis of Rare Relational Data.</div>
      <div class="pub-authors">Chongsheng Zhang, <strong style="color:#111827;">Yaxin Hou</strong>, Ke Chen, Shuang Cao, Gaojuan Fan, Ji Liu.</div>
      <div class="pub-links">
        <a class="pub-btn" href="https://ojs.aaai.org/index.php/AAAI/article/view/25811" target="_blank">📄 Paper</a>
        <a class="pub-btn secondary" href="https://github.com/yaxinhou/QAST" target="_blank">💻 Code</a>
      </div>
    </div>
  </div>
</div>

<div class="subheading">Journal Papers</div>
<div class="pub-list">
  <div class="pub-card">
    <div class="pub-thumb">
      <div class="paper-badge">CCF B</div>
      <img src="./images/imFTP.png" alt="Publication Image">
    </div>
    <div>
      <div class="pub-tags"><span class="pub-tag">Journal</span><span class="pub-tag">CCF B</span><span class="pub-tag">2024</span></div>
      <div class="pub-meta">Information Sciences (Inf. Sci.), 2024.</div>
      <div class="pub-title">imFTP: Deep imbalance learning via fuzzy transition and prototypical learning.</div>
      <div class="pub-authors"><strong style="color:#111827;">Yaxin Hou</strong>, Weiping Ding, Chongsheng Zhang.</div>
      <div class="pub-links">
        <a class="pub-btn" href="https://www.sciencedirect.com/science/article/pii/S002002552400985X" target="_blank">📄 Paper</a>
        <a class="pub-btn secondary" href="https://github.com/yaxinhou/imFTP" target="_blank">💻 Code</a>
      </div>
    </div>
  </div>
</div>

### 👨‍💻 Professional Services

<div class="subheading">Conference Reviewer / Program Committee Member</div>
<div class="info-card">
  <ul class="compact-list">
    <li>The International Conference on Machine Learning (ICML), 2026.</li>
    <li>The European Conference on Computer Vision (ECCV), 2026.</li>
    <li>The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026.</li>
    <li>The Annual Conference on Neural Information Processing Systems (NeurIPS), 2025.</li>
    <li>The IEEE International Symposium on Machine Learning and Media Computing (MLMC), 2025–2026.</li>
  </ul>
</div>

<div class="subheading">Journal Reviewer</div>
<div class="info-card">
  <ul class="compact-list">
    <li>International Journal of Machine Learning and Cybernetics (IJMLC).</li>
    <li>Transactions on Machine Learning Research (TMLR).</li>
    <li>Pattern Recognition (PR).</li>
  </ul>
</div>

### 🏆 Honors & Awards

<div class="subheading">Scholarships</div>
<div class="info-card">
  <ul class="compact-list">
    <li>National Scholarship (2025, The Chinese Ministry of Education).</li>
    <li>Master's Academic Scholarship (2020, The Henan Department of Education).</li>
    <li>National Encouragement Scholarship (2019, The Henan Department of Education).</li>
    <li>National Encouragement Scholarship (2017, The Henan Department of Education).</li>
  </ul>
</div>

<div class="subheading">Honors</div>
<div class="info-card">
  <ul class="compact-list">
    <li>Merit Graduate Student (2025, Southeast University).</li>
    <li>Outstanding Graduate Student (2023, Henan University).</li>
    <li>Outstanding Graduate (2020, The Henan Department of Education).</li>
    <li>Merit Student (2020, The Henan Department of Education).</li>
  </ul>
</div>

### 📧 Contact

<div class="contact-card">
  <div>Room 1009, Liberal Arts Building, School of Computer Science and Engineering.</div>
  <div class="map-shell">
    <div>
      <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=4D0h1VqEfuXzDioG4SfurpFAjXyS5BKdHFuIwYdKIHE&cl=ffffff&w=a"></script>
    </div>
  </div>
</div>
