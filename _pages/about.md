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
    --bg: #f6f7fb;
    --surface: rgba(255,255,255,0.82);
    --surface-strong: #ffffff;
    --surface-soft: #f8f9ff;
    --text: #1f2430;
    --muted: #5f6677;
    --line: rgba(107, 114, 128, 0.16);
    --primary: #5b5bd6;
    --primary-deep: #4038b8;
    --accent: #8b5cf6;
    --accent-soft: #efe9ff;
    --shadow: 0 12px 30px rgba(31, 36, 48, 0.08);
    --shadow-hover: 0 18px 36px rgba(31, 36, 48, 0.12);
    --radius-xl: 24px;
    --radius-lg: 18px;
    --radius-md: 14px;
    --max-width: 1120px;
  }

  body {
    font-family: "Inter", "Segoe UI", "Helvetica Neue", Arial, sans-serif;
    color: var(--text);
    background:
      radial-gradient(circle at top left, rgba(139, 92, 246, 0.10), transparent 28%),
      radial-gradient(circle at top right, rgba(91, 91, 214, 0.10), transparent 22%),
      linear-gradient(180deg, #fbfbfe 0%, #f5f7fb 100%);
    line-height: 1.78;
    letter-spacing: 0.01em;
  }

  .page__content {
    max-width: var(--max-width);
  }

  p, li, span {
    color: var(--text);
  }

  a {
    color: var(--primary-deep);
    text-decoration: none;
    transition: all 0.2s ease;
  }

  a:hover {
    color: var(--accent);
  }

  h3 {
    position: relative;
    margin: 3.2rem 0 1.2rem;
    padding-left: 0.9rem;
    font-size: 1.28rem;
    font-weight: 800;
    letter-spacing: 0.02em;
    color: #141927;
  }

  h3::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0.15em;
    width: 4px;
    height: 1.15em;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--primary), var(--accent));
  }

  hr {
    border: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, rgba(91, 91, 214, 0.25), transparent);
    margin: 3.2rem 0;
  }

  .hero-card,
  .glass-card,
  .news-box,
  .pie-card,
  .publication-container,
  .service-card,
  .award-card,
  .contact-card,
  .map-shell {
    background: var(--surface);
    backdrop-filter: blur(14px);
    -webkit-backdrop-filter: blur(14px);
    border: 1px solid rgba(255,255,255,0.65);
    box-shadow: var(--shadow);
  }

  .hero-card {
    position: relative;
    overflow: hidden;
    border-radius: 28px;
    padding: 28px 30px;
    margin-top: 0.4rem;
  }

  .hero-card::after {
    content: "";
    position: absolute;
    inset: auto -60px -60px auto;
    width: 180px;
    height: 180px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(139, 92, 246, 0.18), transparent 70%);
    pointer-events: none;
  }

  .hero-topline {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 6px 12px;
    margin-bottom: 14px;
    border-radius: 999px;
    font-size: 0.82rem;
    font-weight: 700;
    color: var(--primary-deep);
    background: var(--accent-soft);
    border: 1px solid rgba(91, 91, 214, 0.10);
  }

  .profile-wrapper {
    display: grid;
    grid-template-columns: minmax(0, 1.75fr) minmax(180px, 0.8fr);
    gap: 28px;
    align-items: center;
  }

  .profile-content {
    min-width: 0;
  }

  .profile-text {
    font-size: 1rem;
    line-height: 1.9;
    color: var(--muted);
    margin: 0;
    text-align: justify;
  }

  .profile-highlight {
    color: var(--primary-deep);
    font-weight: 700;
  }

  .profile-logos {
    display: grid;
    grid-template-columns: repeat(2, minmax(72px, 1fr));
    gap: 12px;
    align-items: center;
    justify-items: center;
  }

  .profile-logos a:nth-child(1) {
    grid-column: 1 / -1;
  }

  .logo-tile {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    min-height: 92px;
    padding: 10px;
    border-radius: 18px;
    background: rgba(255,255,255,0.85);
    border: 1px solid rgba(91, 91, 214, 0.08);
    transition: transform 0.22s ease, box-shadow 0.22s ease;
  }

  .logo-tile:hover {
    transform: translateY(-4px);
    box-shadow: 0 10px 20px rgba(91, 91, 214, 0.12);
  }

  .profile-logos img {
    max-width: 82px;
    max-height: 82px;
    object-fit: contain;
    display: block;
    box-shadow: none;
  }

  .section-intro {
    margin: -0.25rem 0 1.1rem;
    font-size: 0.96rem;
    color: var(--muted);
  }

  .news-box {
    border-radius: var(--radius-xl);
    padding: 16px;
    max-height: 360px;
    overflow-y: auto;
    background: linear-gradient(180deg, rgba(255,255,255,0.92), rgba(248,249,255,0.92));
  }

  .news-box::-webkit-scrollbar {
    width: 8px;
  }

  .news-box::-webkit-scrollbar-thumb {
    background: rgba(91, 91, 214, 0.22);
    border-radius: 999px;
  }

  .news-item {
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 12px;
    align-items: start;
    padding: 14px 14px;
    margin-bottom: 10px;
    border-radius: 16px;
    background: rgba(255,255,255,0.72);
    border: 1px solid rgba(91, 91, 214, 0.08);
    transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
  }

  .news-item:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 24px rgba(31, 36, 48, 0.08);
    background: #ffffff;
  }

  .news-emoji {
    font-size: 1.15rem;
    line-height: 1.2;
    margin-top: 1px;
  }

  .news-date {
    display: inline-block;
    min-width: 78px;
    margin-right: 8px;
    color: var(--primary-deep);
    font-weight: 800;
  }

  .inline-link {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    margin-left: 8px;
    font-weight: 700;
  }

  .pie-chart-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 22px;
    margin-top: 1.2rem;
  }

  .pie-card {
    border-radius: 22px;
    padding: 16px 16px 8px;
  }

  .stats-chart {
    width: 100%;
    height: 360px;
  }

  .list-title {
    margin: 0.2rem 0 0.8rem;
    padding-left: 0;
    list-style: none;
    font-size: 1rem;
    font-weight: 800;
    color: #171b28;
  }

  .publication-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 18px;
  }

  .publication-container {
    display: grid;
    grid-template-columns: minmax(180px, 240px) minmax(0, 1fr);
    gap: 20px;
    align-items: center;
    padding: 18px;
    border-radius: 22px;
    transition: transform 0.22s ease, box-shadow 0.22s ease;
  }

  .publication-container:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-hover);
  }

  .pub-img-wrapper {
    position: relative;
    width: 100%;
  }

  .publication-container img {
    width: 100%;
    max-width: 240px;
    max-height: 150px;
    border-radius: 16px;
    object-fit: cover;
    box-shadow: 0 10px 20px rgba(0,0,0,0.16);
  }

  .paper-badge {
    position: absolute;
    top: 10px;
    left: 10px;
    z-index: 2;
    padding: 5px 10px;
    border-radius: 999px;
    background: linear-gradient(135deg, #223a9a, #4f46e5);
    color: #fff;
    font-size: 0.76rem;
    font-weight: 800;
    box-shadow: 0 8px 20px rgba(34, 58, 154, 0.24);
  }

  .pub-meta {
    margin-bottom: 8px;
    font-size: 0.9rem;
    font-weight: 800;
    color: var(--primary-deep);
    letter-spacing: 0.02em;
  }

  .pub-title {
    font-size: 1rem;
    font-weight: 800;
    line-height: 1.65;
    color: #161b27;
  }

  .pub-authors {
    margin-top: 8px;
    color: var(--muted);
    font-size: 0.96rem;
  }

  .pub-authors strong {
    color: var(--primary-deep);
  }

  .service-grid,
  .award-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 18px;
  }

  .service-card,
  .award-card,
  .contact-card,
  .map-shell {
    border-radius: 22px;
    padding: 20px 22px;
  }

  .card-title {
    margin: 0 0 10px;
    font-size: 1rem;
    font-weight: 800;
    color: #171b28;
  }

  .clean-list,
  .nested-list {
    margin: 0;
    padding-left: 1.1rem;
  }

  .clean-list li,
  .nested-list li {
    margin-bottom: 0.55rem;
    color: var(--muted);
  }

  .contact-card {
    padding-bottom: 10px;
  }

  .contact-line {
    margin: 0;
    color: var(--muted);
    font-size: 0.97rem;
  }

  .map-shell {
    margin-top: 18px;
    text-align: center;
  }

  .map-box {
    width: 100%;
    max-width: 320px;
    margin: 0 auto;
    overflow: hidden;
    border-radius: 16px;
  }

  .greedy-nav button {
    display: none !important;
  }

  @media (max-width: 960px) {
    .profile-wrapper,
    .service-grid,
    .award-grid,
    .pie-chart-grid,
    .publication-container {
      grid-template-columns: 1fr;
    }

    .publication-container img {
      max-width: 100%;
      max-height: none;
    }

    .profile-logos {
      grid-template-columns: repeat(3, minmax(72px, 1fr));
    }

    .profile-logos a:nth-child(1) {
      grid-column: auto;
    }
  }

  @media (max-width: 768px) {
    .hero-card,
    .news-box,
    .pie-card,
    .publication-container,
    .service-card,
    .award-card,
    .contact-card,
    .map-shell {
      border-radius: 18px;
    }

    .hero-card {
      padding: 22px 18px;
    }

    .stats-chart {
      height: 300px;
    }

    .profile-text,
    .section-intro,
    .pub-authors,
    .contact-line,
    .clean-list li,
    .nested-list li {
      text-align: left;
    }
  }

  @media (max-width: 480px) {
    h3 {
      font-size: 1.12rem;
    }

    .hero-topline {
      font-size: 0.76rem;
    }

    .news-item {
      grid-template-columns: 1fr;
      gap: 6px;
    }

    .stats-chart {
      height: 260px;
    }
  }
</style>

### 👨‍🎓 Profile

<div class="hero-card">
  <div class="hero-topline">Academic Homepage · Machine Learning · Long-Tailed Learning</div>

  <div class="profile-wrapper">
    <div class="profile-content">
      <p class="profile-text">
        I am currently a <span class="profile-highlight">Ph.D. student at Southeast University</span>, under the supervision of
        <a href="https://jyh-learning.github.io"><strong>Assoc. Prof. Yuheng Jia</strong></a>.
        I received my M.S. degree from Henan University in 2023, under the supervision of
        <a href="https://cs.henu.edu.cn/info/1273/5566.htm"><strong>Prof. Chongsheng Zhang</strong></a>.
        Before that, I obtained my B.S. degree in 2020 from Henan Institute of Engineering.
        My research interests lie in <span class="profile-highlight">machine learning</span>, with a particular focus on
        <span class="profile-highlight">long-tailed learning</span> and <span class="profile-highlight">weakly supervised learning</span>.
      </p>
    </div>

    <div class="profile-logos">
      <a class="logo-tile" href="https://www.seu.edu.cn" target="_blank">
        <img src="./images/SEU.svg" alt="Southeast University" title="Southeast University">
      </a>
      <a class="logo-tile" href="https://cse.seu.edu.cn" target="_blank">
        <img src="./images/CS.png" alt="School of Computer Science and Engineering" title="School of Computer Science and Engineering">
      </a>
      <a class="logo-tile" href="https://www.palmlab.cn" target="_blank">
        <img src="./images/PALM.png" alt="Pattern Learning and Mining Lab" title="Pattern Learning and Mining Lab">
      </a>
    </div>
  </div>
</div>

### 🔥 News

<div class="section-intro">Recent highlights, awards, and paper acceptances.</div>

<div class="news-box">
  <div class="news-item">
    <div class="news-emoji">🎉</div>
    <div>
      <span class="news-date">[2026.01]</span>
      Our work <strong>“Samples Are Not Equal: A Sample Selection Approach for Deep Clustering”</strong> is accepted by <strong>ICLR 2026</strong>!
      <a class="inline-link" href="https://iclr.cc/virtual/2026/poster/10009380">Paper</a>
      <a class="inline-link" href="https://github.com/notoaudrey/Samples-Are-Not-Equal">Code</a>
    </div>
  </div>

  <div class="news-item">
    <div class="news-emoji">🎉</div>
    <div>
      <span class="news-date">[2025.11]</span>
      Our work <strong>“DiCaP: Distribution-Calibrated Pseudo-labeling for Semi-Supervised Multi-Label Learning”</strong> is accepted by <strong>AAAI 2026</strong>!
      <a class="inline-link" href="https://ojs.aaai.org/index.php/AAAI/article/view/39302">Paper</a>
      <a class="inline-link" href="https://github.com/hb-studying/DiCaP">Code</a>
    </div>
  </div>

  <div class="news-item">
    <div class="news-emoji">🏆</div>
    <div>
      <span class="news-date">[2025.10]</span>
      Won the <strong>National Scholarship for Ph.D. Students</strong>.
    </div>
  </div>

  <div class="news-item">
    <div class="news-emoji">🎉</div>
    <div>
      <span class="news-date">[2025.09]</span>
      Our work <strong>“Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning”</strong> is accepted by <strong>NeurIPS 2025</strong>!
      <a class="inline-link" href="https://neurips.cc/virtual/2025/loc/san-diego/poster/116160">Paper</a>
      <a class="inline-link" href="https://github.com/YaxinHou/CPG">Code</a>
    </div>
  </div>

  <div class="news-item" style="margin-bottom:0;">
    <div class="news-emoji">🎉</div>
    <div>
      <span class="news-date">[2025.05]</span>
      Our work <strong>“A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning”</strong> is accepted by <strong>ICML 2025</strong>!
      <a class="inline-link" href="https://icml.cc/virtual/2025/poster/44441">Paper</a>
      <a class="inline-link" href="https://github.com/YaxinHou/Meta-Expert">Code</a>
    </div>
  </div>
</div>

### 📊 Publication Statistics

<div class="section-intro">
  A concise overview of publications by venue, including accepted and published papers listed on this homepage.
</div>

<div class="pie-chart-grid">
  <div class="pie-card">
    <div id="conference-chart" class="stats-chart"></div>
  </div>
  <div class="pie-card">
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

  const conferenceTotal = conferenceData.reduce((sum, item) => sum + item.value, 0);
  const journalTotal = journalData.reduce((sum, item) => sum + item.value, 0);

  const mutedColorsConference = ['#5B5BD6', '#7C73F2', '#A08CFF', '#CDC4FF'];
  const mutedColorsJournal = ['#6E7BC7', '#A9B6E8', '#CAD4F6', '#E3E9FF'];

  function buildPieOption(titleText, total, data, colors) {
    const isMobile = window.innerWidth <= 768;
    const isTiny = window.innerWidth <= 480;

    return {
      tooltip: {
        trigger: 'item',
        formatter: '{b}: {c} ({d}%)',
        backgroundColor: 'rgba(255,255,255,0.98)',
        borderColor: '#ececf4',
        borderWidth: 1,
        textStyle: {
          color: '#1f2430',
          fontFamily: 'Inter, Arial, sans-serif'
        }
      },
      legend: {
        top: 10,
        left: 'center',
        orient: 'horizontal',
        icon: 'circle',
        itemWidth: isMobile ? 10 : 12,
        itemHeight: isMobile ? 10 : 12,
        textStyle: {
          color: '#5f6677',
          fontSize: isTiny ? 10 : (isMobile ? 11 : 12),
          fontFamily: 'Inter, Arial, sans-serif'
        }
      },
      graphic: [
        {
          type: 'text',
          left: 'center',
          top: isMobile ? '46.5%' : '50%',
          style: {
            text: titleText,
            textAlign: 'center',
            fill: '#6a7285',
            fontSize: isTiny ? 11 : (isMobile ? 12 : 14),
            fontWeight: 700,
            fontFamily: 'Inter, Arial, sans-serif'
          }
        },
        {
          type: 'text',
          left: 'center',
          top: isMobile ? '54%' : '57%',
          style: {
            text: String(total),
            textAlign: 'center',
            fill: '#1f2430',
            fontSize: isTiny ? 18 : (isMobile ? 20 : 26),
            fontWeight: 800,
            fontFamily: 'Inter, Arial, sans-serif'
          }
        }
      ],
      series: [
        {
          type: 'pie',
          radius: isTiny ? ['38%', '56%'] : (isMobile ? ['42%', '60%'] : ['48%', '67%']),
          center: isTiny ? ['50%', '62%'] : (isMobile ? ['50%', '60%'] : ['50%', '58%']),
          avoidLabelOverlap: true,
          minShowLabelAngle: 10,
          itemStyle: {
            borderColor: '#ffffff',
            borderWidth: 3
          },
          label: {
            show: true,
            position: 'outside',
            formatter: isMobile ? '{b}\n{c}' : '{b}: {c}',
            color: '#4f5668',
            fontSize: isTiny ? 9 : (isMobile ? 10 : 12),
            fontWeight: 700,
            fontFamily: 'Inter, Arial, sans-serif'
          },
          labelLine: {
            show: true,
            length: isTiny ? 4 : (isMobile ? 6 : 8),
            length2: isTiny ? 3 : (isMobile ? 4 : 6),
            lineStyle: {
              color: '#c4c9d9'
            }
          },
          emphasis: {
            scale: true,
            scaleSize: 5
          },
          color: colors,
          data: data
        }
      ]
    };
  }

  function renderCharts() {
    conferenceChart.setOption(buildPieOption('Conference', conferenceTotal, conferenceData, mutedColorsConference), true);
    journalChart.setOption(buildPieOption('Journal', journalTotal, journalData, mutedColorsJournal), true);
    conferenceChart.resize();
    journalChart.resize();
  }

  renderCharts();

  let resizeTimer = null;
  window.addEventListener('resize', function () {
    clearTimeout(resizeTimer);
    resizeTimer = setTimeout(renderCharts, 150);
  });
</script>

### 📝 Publications

<div class="section-intro">
  Papers are listed in descending order by year of submission before publication, or by year of publication. For a complete list, please visit my
  <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=-0IuShsAAAAJ">Google Scholar</a> page.
</div>

<div class="list-title">Conference Papers</div>

<div class="publication-grid">
  <div class="publication-container">
    <div class="pub-img-wrapper">
      <div class="paper-badge">CCF A</div>
      <img src="./images/CPG.png" alt="CPG publication image">
    </div>
    <div>
      <div class="pub-meta">NeurIPS 2025</div>
      <div class="pub-title">Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning.</div>
      <div class="pub-authors"><strong>Yaxin Hou</strong>, Bo Han, Yuheng Jia, Hui Liu, Junhui Hou.</div>
    </div>
  </div>

  <div class="publication-container">
    <div class="pub-img-wrapper">
      <div class="paper-badge">CCF A</div>
      <img src="./images/Meta-Expert.png" alt="Meta-Expert publication image">
    </div>
    <div>
      <div class="pub-meta">ICML 2025</div>
      <div class="pub-title">A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning.</div>
      <div class="pub-authors"><strong>Yaxin Hou</strong>, Yuheng Jia.</div>
    </div>
  </div>

  <div class="publication-container">
    <div class="pub-img-wrapper">
      <div class="paper-badge">CCF A</div>
      <img src="./images/QAST.png" alt="QAST publication image">
    </div>
    <div>
      <div class="pub-meta">AAAI 2023</div>
      <div class="pub-title">Quality-Aware Self-Training on Differentiable Synthesis of Rare Relational Data.</div>
      <div class="pub-authors">Chongsheng Zhang, <strong>Yaxin Hou</strong>, Ke Chen, Shuang Cao, Gaojuan Fan, Ji Liu.</div>
    </div>
  </div>
</div>

<div class="list-title" style="margin-top: 1.4rem;">Journal Papers</div>

<div class="publication-grid">
  <div class="publication-container">
    <div class="pub-img-wrapper">
      <div class="paper-badge">CCF B</div>
      <img src="./images/imFTP.png" alt="imFTP publication image">
    </div>
    <div>
      <div class="pub-meta">Information Sciences 2024</div>
      <div class="pub-title">imFTP: Deep imbalance learning via fuzzy transition and prototypical learning.</div>
      <div class="pub-authors"><strong>Yaxin Hou</strong>, Weiping Ding, Chongsheng Zhang.</div>
    </div>
  </div>
</div>

### 👨‍💻 Professional Services

<div class="service-grid">
  <div class="service-card">
    <div class="card-title">Conference Reviewer / Program Committee Member</div>
    <ul class="clean-list">
      <li>The International Conference on Machine Learning (ICML), 2026.</li>
      <li>The European Conference on Computer Vision (ECCV), 2026.</li>
      <li>The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026.</li>
      <li>The Annual Conference on Neural Information Processing Systems (NeurIPS), 2025.</li>
      <li>The IEEE International Symposium on Machine Learning and Media Computing (MLMC), 2025–2026.</li>
    </ul>
  </div>

  <div class="service-card">
    <div class="card-title">Journal Reviewer</div>
    <ul class="clean-list">
      <li>International Journal of Machine Learning and Cybernetics (IJMLC).</li>
      <li>Transactions on Machine Learning Research (TMLR).</li>
      <li>Pattern Recognition (PR).</li>
    </ul>
  </div>
</div>

### 🏆 Honors & Awards

<div class="award-grid">
  <div class="award-card">
    <div class="card-title">Scholarships</div>
    <ul class="clean-list">
      <li>National Scholarship (2025, The Chinese Ministry of Education).</li>
      <li>Master's Academic Scholarship (2020, The Henan Department of Education).</li>
      <li>National Encouragement Scholarship (2019, The Henan Department of Education).</li>
      <li>National Encouragement Scholarship (2017, The Henan Department of Education).</li>
    </ul>
  </div>

  <div class="award-card">
    <div class="card-title">Honors</div>
    <ul class="clean-list">
      <li>Merit Graduate Student (2025, Southeast University).</li>
      <li>Outstanding Graduate Student (2023, Henan University).</li>
      <li>Outstanding Graduate (2020, The Henan Department of Education).</li>
      <li>Merit Student (2020, The Henan Department of Education).</li>
    </ul>
  </div>
</div>

### 📧 Contact

<div class="contact-card">
  <p class="contact-line">Room 1009, Liberal Arts Building, School of Computer Science and Engineering.</p>

  <div class="map-shell">
    <div class="map-box">
      <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=4D0h1VqEfuXzDioG4SfurpFAjXyS5BKdHFuIwYdKIHE&cl=ffffff&w=a"></script>
    </div>
  </div>
</div>
