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
    --text: #1f2937;
    --muted: #667085;
    --line: #e6ebf2;
    --soft: #f7f9fc;
    --soft-2: #fbfcfe;
    --accent: #245b92;
    --accent-2: #4f86ba;
    --accent-soft: #eef5fb;
    --title: #0f172a;
    --shadow-sm: 0 6px 18px rgba(15, 23, 42, 0.05);
    --shadow: 0 12px 34px rgba(15, 23, 42, 0.07);
    --shadow-lg: 0 18px 40px rgba(15, 23, 42, 0.1);
    --radius: 18px;
    --radius-sm: 14px;
    --maxw: 1080px;
  }

  html {
    font-size: 15px;
    scroll-behavior: smooth;
  }

  body {
    font-family: "Inter", "Segoe UI", Arial, sans-serif;
    color: var(--text);
    background:
      radial-gradient(circle at top right, rgba(79, 134, 186, 0.07), transparent 22%),
      linear-gradient(180deg, #fcfdff 0%, #ffffff 24%);
    line-height: 1.75;
    letter-spacing: 0.01em;
    text-rendering: optimizeLegibility;
  }

  .page,
  .page__content,
  .archive {
    max-width: var(--maxw);
  }

  p, span, li, div {
    font-size: 0.95rem;
  }

  p {
    margin-bottom: 0.9rem;
  }

  a {
    color: var(--accent);
    text-decoration: none;
    transition: color 0.2s ease, border-color 0.2s ease, background 0.2s ease, box-shadow 0.2s ease, transform 0.2s ease;
  }

  a:hover {
    color: #173f67;
  }

  .sidebar .author__name,
  .author__name {
    font-size: 1.1rem !important;
    line-height: 1.3 !important;
    font-weight: 800 !important;
    color: var(--title) !important;
    margin-top: 0.36rem !important;
    margin-bottom: 0.76rem !important;
  }

  .sidebar .author__bio,
  .author__bio {
    font-size: 0.95rem !important;
    line-height: 1.66 !important;
    color: var(--text) !important;
    margin-bottom: 0.76rem !important;
  }

  .sidebar .author__pronouns,
  .author__pronouns {
    font-size: 0.93rem !important;
    line-height: 1.58 !important;
    color: var(--muted) !important;
    margin-bottom: 0.76rem !important;
  }

  .sidebar .author__urls-wrapper,
  .author__urls-wrapper {
    margin-top: 0.82rem !important;
  }

  .sidebar .author__urls,
  .author__urls {
    margin-top: 0.18rem !important;
  }

  .sidebar .author__urls li,
  .author__urls li {
    font-size: 0.94rem !important;
    line-height: 1.62 !important;
    margin-bottom: 0.48rem !important;
  }

  .sidebar .author__urls a,
  .author__urls a {
    font-size: 0.94rem !important;
    color: var(--text) !important;
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
    color: var(--text) !important;
  }

  h3 {
    position: relative;
    margin: 3rem 0 1.15rem;
    padding: 0 0 0.8rem 0.95rem;
    font-size: 1.08rem;
    font-weight: 800;
    color: var(--title);
    letter-spacing: 0.01em;
    border-bottom: 1px solid var(--line);
  }

  h3::before {
    content: '';
    position: absolute;
    left: 0;
    top: 0.18rem;
    width: 4px;
    height: 1.05rem;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--accent) 0%, var(--accent-2) 100%);
    box-shadow: 0 4px 10px rgba(36, 91, 146, 0.25);
  }

  strong {
    font-weight: 700;
  }

  .page-intro,
  .section-note {
    color: var(--muted);
    font-size: 0.9rem;
    margin-top: -0.1rem;
    margin-bottom: 1rem;
  }

  .hero {
    position: relative;
    display: grid;
    grid-template-columns: minmax(0, 1fr) 185px;
    gap: 1.6rem;
    align-items: center;
    padding: 1.45rem 1.5rem;
    background:
      radial-gradient(circle at top right, rgba(79, 134, 186, 0.11), transparent 28%),
      linear-gradient(180deg, #ffffff 0%, #f8fbff 100%);
    border: 1px solid rgba(36, 91, 146, 0.11);
    border-radius: 22px;
    box-shadow: var(--shadow);
    overflow: hidden;
  }

  .hero::after {
    content: '';
    position: absolute;
    inset: auto 0 0 0;
    height: 3px;
    background: linear-gradient(90deg, rgba(36, 91, 146, 0.9), rgba(79, 134, 186, 0.35), rgba(255, 255, 255, 0));
  }

  .hero-text {
    min-width: 0;
  }

  .hero-text p {
    margin: 0;
    text-align: left;
  }

  .hero-links {
    margin-top: 0.95rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
  }

  .hero-chip {
    display: inline-flex;
    align-items: center;
    padding: 0.34rem 0.76rem;
    border: 1px solid #d8e5f1;
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.92);
    color: var(--accent);
    font-size: 0.82rem;
    font-weight: 700;
    white-space: nowrap;
    box-shadow: 0 2px 8px rgba(15, 23, 42, 0.04);
  }

  .logo-panel {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    align-items: start;
    justify-items: stretch;
    width: 100%;
    min-width: 0;
  }

  .logo-panel a {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 112px;
    width: 100%;
    min-width: 0;
    padding: 1rem 1.15rem;
    background: rgba(255, 255, 255, 0.92);
    border: 1px solid var(--line);
    border-radius: 18px;
    box-shadow: 0 4px 14px rgba(15, 23, 42, 0.04);
    box-sizing: border-box;
    overflow: hidden;
  }

  .logo-panel a:first-child {
    grid-column: 1 / -1;
    min-height: 128px;
  }

  .logo-panel a:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 22px rgba(15, 23, 42, 0.08);
    border-color: #d8e5f1;
  }

  .logo-panel img {
    display: block;
    width: auto;
    max-width: 100%;
    max-height: 76px;
    object-fit: contain;
    filter: grayscale(6%);
    opacity: 0.96;
  }

  .logo-panel a:first-child img {
    max-height: 80px;
  }

  .news-box,
  .stats-card,
  .info-card,
  .contact-card,
  .pub-card {
    backdrop-filter: blur(3px);
  }

  .news-box {
    border: 1px solid var(--line);
    border-radius: 20px;
    background: linear-gradient(180deg, #ffffff 0%, #fcfdff 100%);
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
    grid-template-columns: 96px minmax(0, 1fr);
    gap: 1rem;
    padding: 1rem 1.1rem;
    border-bottom: 1px solid var(--line);
    align-items: start;
    transition: background 0.2s ease, transform 0.2s ease;
  }

  .news-item:hover {
    background: #f9fbff;
  }

  .news-list .news-item:last-child {
    border-bottom: none;
  }

  .news-date {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: fit-content;
    min-width: 76px;
    padding: 0.28rem 0.55rem;
    border-radius: 999px;
    background: var(--accent-soft);
    border: 1px solid #d8e5f1;
    font-size: 0.8rem;
    font-weight: 800;
    color: var(--accent);
    letter-spacing: 0.02em;
  }

  .news-content {
    color: var(--text);
  }

  .news-links {
    display: inline-flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-left: 0.55rem;
    vertical-align: middle;
  }

  .news-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.32rem;
    padding: 0.26rem 0.62rem;
    border-radius: 999px;
    border: 1px solid #d7e3ef;
    background: #fff;
    color: var(--accent);
    font-size: 0.78rem;
    font-weight: 700;
    line-height: 1.2;
    text-decoration: none !important;
    box-shadow: 0 2px 8px rgba(15, 23, 42, 0.03);
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
    padding: 0.85rem 1rem;
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
    border-radius: 10px;
    padding: 0.36rem 0.74rem;
    font-size: 0.84rem;
    font-weight: 600;
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
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
  }

  .stats-card {
    border: 1px solid var(--line);
    border-radius: 20px;
    background: linear-gradient(180deg, #ffffff 0%, #fcfdff 100%);
    padding: 1rem 0.8rem;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: visible;
    box-shadow: var(--shadow-sm);
  }

  .stats-chart {
    width: min(100%, 336px);
    height: 336px;
    margin: 0 auto;
    flex: 0 0 auto;
    overflow: visible;
  }

  .subheading {
    margin: 1.55rem 0 0.9rem;
    font-size: 1rem;
    font-weight: 800;
    color: var(--title);
    display: flex;
    align-items: center;
    gap: 0.55rem;
  }

  .subheading::before {
    content: '';
    width: 4px;
    height: 0.98rem;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--accent) 0%, #7fa1c0 100%);
  }

  .pub-list {
    display: grid;
    gap: 1rem;
  }

  .pub-card {
    display: grid;
    grid-template-columns: 188px minmax(0, 1fr);
    gap: 1.05rem;
    padding: 1rem;
    background: linear-gradient(180deg, #ffffff 0%, #fcfdff 100%);
    border: 1px solid var(--line);
    border-radius: 20px;
    align-items: start;
    box-shadow: var(--shadow-sm);
    transition: transform 0.22s ease, box-shadow 0.22s ease, border-color 0.22s ease;
  }

  .pub-card:hover {
    transform: translateY(-3px);
    border-color: #d9e4ef;
    box-shadow: var(--shadow);
  }

  .pub-thumb {
    position: relative;
    border-radius: 16px;
    overflow: hidden;
    background: linear-gradient(180deg, #fbfcfd 0%, #f6f8fa 100%);
    border: 1px solid var(--line);
    height: 132px;
    padding: 0.75rem;
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
    padding: 0.18rem 0.5rem;
    border-radius: 999px;
    background: rgba(15, 23, 42, 0.82);
    color: #fff;
    font-size: 0.68rem;
    font-weight: 800;
    letter-spacing: 0.02em;
    box-shadow: 0 4px 10px rgba(15, 23, 42, 0.16);
  }

  .pub-meta {
    margin-bottom: 0.4rem;
    color: var(--accent);
    font-size: 0.82rem;
    font-weight: 800;
  }

  .pub-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-bottom: 0.58rem;
  }

  .pub-tag {
    display: inline-flex;
    align-items: center;
    padding: 0.22rem 0.58rem;
    border-radius: 999px;
    background: var(--accent-soft);
    border: 1px solid #d8e4f0;
    color: var(--accent);
    font-size: 0.74rem;
    font-weight: 800;
    letter-spacing: 0.01em;
  }

  .pub-title {
    margin: 0 0 0.42rem;
    color: var(--title);
    font-size: 1rem;
    line-height: 1.46;
    font-weight: 800;
  }

  .pub-authors {
    color: var(--muted);
    line-height: 1.68;
    margin-bottom: 0.78rem;
  }

  .pub-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.14rem;
  }

  .pub-btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.28rem;
    min-width: 92px;
    padding: 0.34rem 0.72rem;
    border-radius: 999px;
    border: 1px solid #d7e3ef;
    background: #f8fbfe;
    color: var(--accent);
    font-size: 0.78rem;
    font-weight: 700;
    line-height: 1.15;
    text-decoration: none !important;
    box-shadow: 0 2px 8px rgba(15, 23, 42, 0.03);
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
    box-shadow: 0 2px 8px rgba(15, 23, 42, 0.03);
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

  .info-card {
    border: 1px solid var(--line);
    border-radius: var(--radius);
    background: linear-gradient(180deg, #ffffff 0%, #fcfdff 100%);
    padding: 1rem 1.08rem;
    box-shadow: 0 5px 16px rgba(15, 23, 42, 0.04);
  }

  .info-card h4 {
    margin: 0 0 0.7rem;
    font-size: 0.92rem;
    color: var(--title);
  }

  .info-card ul {
    margin: 0;
    padding-left: 1.1rem;
  }

  .info-card li {
    margin-bottom: 0.5rem;
    color: var(--text);
  }

  .contact-card {
    border: 1px solid var(--line);
    border-radius: 20px;
    background: linear-gradient(180deg, #ffffff 0%, var(--soft-2) 100%);
    padding: 1rem 1.08rem;
    box-shadow: 0 5px 16px rgba(15, 23, 42, 0.04);
  }

  .map-shell {
    margin: 1rem auto 0;
    border: 1px solid var(--line);
    border-radius: 14px;
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
    margin-top: 0.4rem;
  }

  .compact-list li {
    margin-bottom: 0.42rem;
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

    .sidebar .author__name,
    .author__name {
      font-size: 1.03rem !important;
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
      margin-top: 2.35rem;
      padding-left: 0.82rem;
    }

    .hero,
    .stats-card,
    .info-card,
    .contact-card,
    .pub-card {
      padding: 0.92rem;
    }

    .news-item {
      grid-template-columns: 1fr;
      gap: 0.45rem;
    }

    .news-links {
      margin-left: 0;
      margin-top: 0.48rem;
    }

    .pub-thumb {
      height: 150px;
      padding: 0.76rem;
    }

    .pub-thumb img {
      width: 100%;
      height: 100%;
      max-height: none;
      object-fit: contain;
    }

    .stats-chart {
      width: min(100%, 286px);
      height: 286px;
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

### 📊 Publication Statistics

<div class="section-note">
  A brief overview of publications by venue, including accepted and published papers listed on this homepage.
</div>

<div class="stats-wrap">
  <div class="stats-card">
    <div id="conference-chart" class="stats-chart"></div>
  </div>
  <div class="stats-card">
    <div id="journal-chart" class="stats-chart"></div>
  </div>
</div>

<div class="section-note" style="margin-top:0.85rem;">
  Currently listed on this homepage: <strong>6 papers</strong>, including <strong>5 conference papers</strong> and <strong>1 journal paper</strong>.
</div>

<script src="https://cdn.jsdelivr.net/npm/echarts@5/dist/echarts.min.js"></script>
<script>
  const conferenceChart = echarts.init(document.getElementById('conference-chart'), null, { renderer: 'svg' });
  const journalChart = echarts.init(document.getElementById('journal-chart'), null, { renderer: 'svg' });

  const conferenceData = [
    { value: 1, name: 'ICLR' },
    { value: 1, name: 'NeurIPS' },
    { value: 1, name: 'ICML' },
    { value: 2, name: 'AAAI' }
  ];

  const journalData = [
    { value: 1, name: 'Inf. Sci.' }
  ];

  function buildPieOption(title, total, data, colors) {
    const isMobile = window.innerWidth <= 768;
    return {
      tooltip: {
        trigger: 'item',
        formatter: '{b}: {c} ({d}%)',
        backgroundColor: 'rgba(255,255,255,0.98)',
        borderColor: '#e7ebf0',
        borderWidth: 1,
        textStyle: { color: '#1f2328', fontFamily: 'Inter, Arial, sans-serif' }
      },
      color: colors,
      legend: {
        top: 6,
        left: 'center',
        icon: 'circle',
        itemWidth: 10,
        itemHeight: 10,
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
          top: '46%',
          style: {
            text: title,
            textAlign: 'center',
            fill: '#6b7280',
            fontSize: isMobile ? 11 : 12,
            fontWeight: 600,
            fontFamily: 'Inter, Arial, sans-serif'
          }
        },
        {
          type: 'text',
          left: 'center',
          top: '54%',
          style: {
            text: String(total),
            textAlign: 'center',
            fill: '#111827',
            fontSize: isMobile ? 20 : 22,
            fontWeight: 700,
            fontFamily: 'Inter, Arial, sans-serif'
          }
        }
      ],
      series: [
        {
          type: 'pie',
          left: isMobile ? 10 : 18,
          right: isMobile ? 10 : 18,
          top: isMobile ? 18 : 20,
          bottom: isMobile ? 18 : 20,
          radius: isMobile ? ['39%', '57%'] : ['44%', '61%'],
          center: isMobile ? ['50%', '56%'] : ['50%', '57%'],
          minShowLabelAngle: 8,
          avoidLabelOverlap: true,
          itemStyle: {
            borderColor: '#ffffff',
            borderWidth: 2
          },
          label: {
            color: '#4b5563',
            fontSize: isMobile ? 9 : 11,
            formatter: isMobile ? '{b}\n{c}' : '{b}: {c}',
            width: isMobile ? 44 : 64,
            overflow: 'break'
          },
          labelLine: {
            length: isMobile ? 6 : 9,
            length2: isMobile ? 6 : 10,
            maxSurfaceAngle: 80,
            lineStyle: { color: '#c7d0db' }
          },
          emphasis: { scale: false },
          data: data
        }
      ]
    };
  }

  function renderCharts() {
    conferenceChart.setOption(buildPieOption('Conference', 5, conferenceData, ['#365d84', '#5f7fa1', '#89a3bd', '#b4c6d8']), true);
    journalChart.setOption(buildPieOption('Journal', 1, journalData, ['#4d6f8f']), true);
    conferenceChart.resize();
    journalChart.resize();
  }

  renderCharts();

  if (typeof ResizeObserver !== 'undefined') {
    const chartContainers = [
      document.getElementById('conference-chart'),
      document.getElementById('journal-chart')
    ].filter(Boolean);

    const resizeObserver = new ResizeObserver(function () {
      conferenceChart.resize();
      journalChart.resize();
    });

    chartContainers.forEach(function (el) {
      resizeObserver.observe(el);
    });
  } else {
    let resizeTimer = null;
    window.addEventListener('resize', function () {
      clearTimeout(resizeTimer);
      resizeTimer = setTimeout(function () {
        conferenceChart.resize();
        journalChart.resize();
      }, 120);
    });
  }
</script>

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

### 📝 Publications

<div class="section-note">
  Papers are listed in descending order by year of submission before publication, or by year of publication. For a full list, please visit my <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=-0IuShsAAAAJ">Google Scholar</a> page.
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
