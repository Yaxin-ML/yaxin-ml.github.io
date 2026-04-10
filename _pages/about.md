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
    --text: #1f2328;
    --muted: #5f6b7a;
    --line: #e7ebf0;
    --soft: #f7f9fb;
    --soft-2: #fbfcfd;
    --accent: #1f4e79;
    --accent-soft: #eef4fa;
    --title: #111827;
    --shadow: 0 8px 24px rgba(15, 23, 42, 0.04);
    --radius: 14px;
  }

  html {
    font-size: 15px;
    scroll-behavior: smooth;
  }

  body {
    font-family: "Inter", "Segoe UI", Arial, sans-serif;
    color: var(--text);
    background: #ffffff;
    line-height: 1.72;
    letter-spacing: 0.01em;
    text-rendering: optimizeLegibility;
  }

  p, span, li, div {
    font-size: 0.94rem;
  }

  a {
    color: var(--accent);
    text-decoration: none;
    transition: color 0.18s ease, border-color 0.18s ease;
  }

  a:hover {
    color: #153b5d;
  }

  .sidebar .author__name,
  .author__name {
    font-size: 1.07rem !important;
    line-height: 1.28 !important;
    font-weight: 700 !important;
    color: var(--title) !important;
    margin-top: 0.36rem !important;
    margin-bottom: 0.76rem !important;
  }

  .sidebar .author__bio,
  .author__bio {
    font-size: 0.95rem !important;
    line-height: 1.64 !important;
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
    margin-top: 0.8rem !important;
  }

  .sidebar .author__urls,
  .author__urls {
    margin-top: 0.15rem !important;
  }

  .sidebar .author__urls li,
  .author__urls li {
    font-size: 0.95rem !important;
    line-height: 1.6 !important;
    margin-bottom: 0.44rem !important;
  }

  .sidebar .author__urls a,
  .author__urls a {
    font-size: 0.95rem !important;
    color: var(--text) !important;
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
    margin: 2.6rem 0 1rem;
    font-size: 1.02rem;
    font-weight: 700;
    color: var(--title);
    letter-spacing: 0.01em;
    padding-bottom: 0.55rem;
    border-bottom: 1px solid var(--line);
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
    display: grid;
    grid-template-columns: minmax(0, 1fr) 170px;
    gap: 1.5rem;
    align-items: center;
    padding: 1.25rem 1.35rem;
    background: linear-gradient(180deg, var(--soft-2) 0%, #ffffff 100%);
    border: 1px solid var(--line);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
  }

  .hero-text {
    min-width: 0;
  }

  .hero-text p {
    margin: 0;
    text-align: left;
  }

  .hero-links {
    margin-top: 0.8rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
  }

  .hero-chip {
    display: inline-flex;
    align-items: center;
    padding: 0.28rem 0.68rem;
    border: 1px solid var(--line);
    border-radius: 999px;
    background: #fff;
    color: var(--muted);
    font-size: 0.82rem;
    white-space: nowrap;
  }

  .logo-panel {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    align-items: center;
    justify-items: center;
  }

  .logo-panel a:first-child {
    grid-column: 1 / -1;
  }

  .logo-panel img {
    display: block;
    width: auto;
    max-width: 110px;
    max-height: 83px;
    object-fit: contain;
    filter: grayscale(8%);
    opacity: 0.95;
  }

  .news-box {
    border: 1px solid var(--line);
    border-radius: var(--radius);
    background: #fff;
    overflow: hidden;
  }

  .news-list {
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .news-item {
    display: grid;
    grid-template-columns: 92px minmax(0, 1fr);
    gap: 1rem;
    padding: 0.9rem 1rem;
    border-bottom: 1px solid var(--line);
    align-items: start;
  }

  .news-list .news-item:last-child {
    border-bottom: none;
  }

  .news-date {
    font-size: 0.82rem;
    font-weight: 700;
    color: var(--accent);
    letter-spacing: 0.02em;
  }

  .news-content {
    color: var(--text);
  }

  .news-pagination {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 0.75rem;
    padding: 0.8rem 1rem;
    border-top: 1px solid var(--line);
    background: var(--soft-2);
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
    padding: 0.34rem 0.72rem;
    font-size: 0.84rem;
    line-height: 1.2;
    cursor: pointer;
    transition: background 0.18s ease, color 0.18s ease, border-color 0.18s ease;
  }

  .news-page-btn:hover:not(:disabled) {
    background: var(--accent-soft);
    border-color: #d6e2ef;
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
    border-radius: var(--radius);
    background: #fff;
    padding: 1rem 1.1rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .stats-chart {
    width: min(100%, 300px);
    height: 300px;
    margin: 0 auto;
    flex: 0 0 auto;
  }

  .subheading {
    margin: 1.2rem 0 0.75rem;
    font-size: 0.95rem;
    font-weight: 700;
    color: var(--title);
  }

  .pub-list {
    display: grid;
    gap: 0.9rem;
  }

  .pub-card {
    display: grid;
    grid-template-columns: 210px minmax(0, 1fr);
    gap: 1rem;
    padding: 0.95rem;
    background: #fff;
    border: 1px solid var(--line);
    border-radius: var(--radius);
    align-items: start;
  }

  .pub-thumb {
    position: relative;
    border-radius: 12px;
    overflow: hidden;
    background: var(--soft);
    border: 1px solid var(--line);
  }

  .pub-thumb img {
    display: block;
    width: 100%;
    height: 132px;
    object-fit: cover;
  }

  .paper-badge {
    position: absolute;
    top: 10px;
    left: 10px;
    padding: 0.18rem 0.45rem;
    border-radius: 999px;
    background: rgba(17, 24, 39, 0.82);
    color: #fff;
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.02em;
  }

  .pub-meta {
    margin-bottom: 0.35rem;
    color: var(--accent);
    font-size: 0.82rem;
    font-weight: 700;
  }

  .pub-title {
    margin: 0 0 0.35rem;
    color: var(--title);
    font-size: 0.98rem;
    line-height: 1.45;
    font-weight: 650;
  }

  .pub-authors {
    color: var(--muted);
    line-height: 1.65;
  }

  .two-col-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
  }

  .info-card {
    border: 1px solid var(--line);
    border-radius: var(--radius);
    background: #fff;
    padding: 1rem 1.05rem;
  }

  .info-card h4 {
    margin: 0 0 0.7rem;
    font-size: 0.92rem;
    color: var(--title);
  }

  .info-card ul {
    margin: 0;
    padding-left: 1.05rem;
  }

  .info-card li {
    margin-bottom: 0.46rem;
    color: var(--text);
  }

  .contact-card {
    border: 1px solid var(--line);
    border-radius: var(--radius);
    background: linear-gradient(180deg, #ffffff 0%, var(--soft-2) 100%);
    padding: 1rem 1.05rem;
  }

  .map-shell {
    margin: 1rem auto 0;
    border: 1px solid var(--line);
    border-radius: 12px;
    overflow: hidden;
    background: #fff;
    max-width: 320px;
  }

  .map-shell > div {
    max-height: 280px;
    overflow: hidden;
  }

  .compact-list {
    margin-top: 0.4rem;
  }

  .compact-list li {
    margin-bottom: 0.4rem;
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
      justify-items: start;
      grid-template-columns: repeat(3, auto);
      gap: 1.45rem;
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
      font-size: 1.02rem !important;
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
      margin-top: 2.2rem;
    }

    .hero,
    .stats-card,
    .info-card,
    .contact-card,
    .pub-card {
      padding: 0.9rem;
    }

    .news-item {
      grid-template-columns: 1fr;
      gap: 0.25rem;
    }

    .pub-thumb img {
      height: auto;
      max-height: 180px;
    }

    .stats-chart {
      width: min(100%, 255px);
      height: 255px;
    }
  }
</style>

### 👨‍🎓 Profile

<div class="hero">
  <div class="hero-text">
    <p>
      I am currently a Ph.D. student at Southeast University, under the supervision of
      <a href="https://jyh-learning.github.io"><strong>Assoc. Prof. Yuheng Jia</strong></a>.
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
      <div class="news-content">🎉 Our work “Samples Are Not Equal: A Sample Selection Approach for Deep Clustering” is accepted by ICLR 2026. <a href="https://iclr.cc/virtual/2026/poster/10009380">Paper</a> · <a href="https://github.com/notoaudrey/Samples-Are-Not-Equal">Code</a></div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.11</div>
      <div class="news-content">🎉 Our work “DiCaP: Distribution-Calibrated Pseudo-labeling for Semi-Supervised Multi-Label Learning” is accepted by AAAI 2026. <a href="https://ojs.aaai.org/index.php/AAAI/article/view/39302">Paper</a> · <a href="https://github.com/hb-studying/DiCaP">Code</a></div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.10</div>
      <div class="news-content">🎉 Received the National Scholarship for Ph.D. students.</div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.09</div>
      <div class="news-content">🎉 Our work “Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning” is accepted by NeurIPS 2025. <a href="https://neurips.cc/virtual/2025/loc/san-diego/poster/116160">Paper</a> · <a href="https://github.com/YaxinHou/CPG">Code</a></div>
    </li>
    <li class="news-item">
      <div class="news-date">2025.05</div>
      <div class="news-content">🎉 Our work “A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning” is accepted by ICML 2025. <a href="https://icml.cc/virtual/2025/poster/44441">Paper</a> · <a href="https://github.com/YaxinHou/Meta-Expert">Code</a></div>
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
          radius: isMobile ? ['40%', '58%'] : ['45%', '64%'],
          center: ['50%', '58%'],
          minShowLabelAngle: 8,
          itemStyle: {
            borderColor: '#ffffff',
            borderWidth: 2
          },
          label: {
            color: '#4b5563',
            fontSize: isMobile ? 9 : 10,
            formatter: isMobile ? '{b}\n{c}' : '{b}: {c}'
          },
          labelLine: {
            length: isMobile ? 5 : 7,
            length2: isMobile ? 4 : 6,
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
      <div class="pub-meta">Annual Conference on Neural Information Processing Systems (NeurIPS), 2025</div>
      <div class="pub-title">Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning.</div>
      <div class="pub-authors"><strong style="color:#111827;">Yaxin Hou</strong>, Bo Han, Yuheng Jia, Hui Liu, Junhui Hou.</div>
    </div>
  </div>

  <div class="pub-card">
    <div class="pub-thumb">
      <div class="paper-badge">CCF A</div>
      <img src="./images/Meta-Expert.png" alt="Publication Image">
    </div>
    <div>
      <div class="pub-meta">International Conference on Machine Learning (ICML), 2025</div>
      <div class="pub-title">A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning.</div>
      <div class="pub-authors"><strong style="color:#111827;">Yaxin Hou</strong>, Yuheng Jia.</div>
    </div>
  </div>

  <div class="pub-card">
    <div class="pub-thumb">
      <div class="paper-badge">CCF A</div>
      <img src="./images/QAST.png" alt="Publication Image">
    </div>
    <div>
      <div class="pub-meta">AAAI Conference on Artificial Intelligence (AAAI), 2023</div>
      <div class="pub-title">Quality-Aware Self-Training on Differentiable Synthesis of Rare Relational Data.</div>
      <div class="pub-authors">Chongsheng Zhang, <strong style="color:#111827;">Yaxin Hou</strong>, Ke Chen, Shuang Cao, Gaojuan Fan, Ji Liu.</div>
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
      <div class="pub-meta">Information Sciences (Inf. Sci.), 2024</div>
      <div class="pub-title">imFTP: Deep imbalance learning via fuzzy transition and prototypical learning.</div>
      <div class="pub-authors"><strong style="color:#111827;">Yaxin Hou</strong>, Weiping Ding, Chongsheng Zhang.</div>
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

<div class="two-col-grid">
  <div class="info-card">
    <h4>Scholarships</h4>
    <ul class="compact-list">
      <li>National Scholarship (2025, The Chinese Ministry of Education).</li>
      <li>Master's Academic Scholarship (2020, The Henan Department of Education).</li>
      <li>National Encouragement Scholarship (2019, The Henan Department of Education).</li>
      <li>National Encouragement Scholarship (2017, The Henan Department of Education).</li>
    </ul>
  </div>

  <div class="info-card">
    <h4>Honors</h4>
    <ul class="compact-list">
      <li>Merit Graduate Student (2025, Southeast University).</li>
      <li>Outstanding Graduate Student (2023, Henan University).</li>
      <li>Outstanding Graduate (2020, The Henan Department of Education).</li>
      <li>Merit Student (2020, The Henan Department of Education).</li>
    </ul>
  </div>
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
