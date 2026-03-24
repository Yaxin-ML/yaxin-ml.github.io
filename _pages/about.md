---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  body {
    font-family: "Segoe UI", Arial, sans-serif;
    background: #ffffff;
    color: #222;
    line-height: 1.6em;
  }

  h3 {
    color: #000000;
    font-weight: 800;
    margin-top: 2.3em;
    letter-spacing: 0.3px;
  }

  hr {
    clear: both;
    border: none;
    border-top: 2px dashed #c5c5c5;
    margin: 3em 0;
  }

  .card {
    border-radius: 12px;
    padding: 18px 22px;
    background: #fafafa;
    box-shadow: 0 3px 8px rgba(0,0,0,0.08);
  }

  .profile-text {
    font-size: 0.95em;
    text-align: justify;
    line-height: 1.65em;
    display: block;
    margin-top: 8px;
  }

  .news-box {
    max-height: 300px;
    overflow-y: auto;
    border-left: 4px solid #f0eaff;
    padding: 16px 20px;
    border-radius: 12px;
    background: #f9f9fc;
    box-shadow: inset 0 0 6px rgba(0,0,0,0.05);
  }

  .news-item {
    padding: 3px 12px;
    margin-bottom: 2px;
    border-radius: 8px;
    transition: background 0.25s;
  }

  .news-item:hover {
    background: #f0eaff;
  }

  .publication-container {
    display: flex;
    gap: 18px;
    margin-bottom: 2.3em;
    font-size: 0.8em;
    padding: 12px;
    background: #fafafa;
    border-radius: 12px;
    transition: 0.25s ease;
    align-items: flex-start;
    border: 1px solid #eee;
    clear: both;
  }

  .publication-container:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 18px rgba(0,0,0,0.12);
  }

  .publication-container img {
    max-width: 240px;
    max-height: 150px;
    border-radius: 10px;
    object-fit: cover;
    box-shadow: 0 3px 10px rgba(0,0,0,0.18);
    flex-shrink: 0;
  }

  .paper-badge {
    position: absolute;
    top: 6px;
    left: 6px;
    background: #00308B;
    color: #fff;
    padding: 2.5px 6px;
    font-size: 0.8em;
    font-weight: bold;
    line-height: 1.0;
    border-radius: 4px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.15);
  }

  .pub-img-wrapper {
    position: relative;
    display: inline-block;
  }

  ul {
    margin-top: 0.5em;
    margin-bottom: 0.5em;
    line-height: 1.5em;
  }

  li {
    margin-bottom: 4px;
  }

  .map-container {
    display: flex; 
    justify-content: center; 
    margin: 25px 0;
  }

  .map-box {
    width: 100%; 
    max-width: 320px; 
    text-align: center;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0,0,0,0.12);
  }

  .profile-wrapper {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 20px;
  }

  .profile-content {
    flex: 3;
    width: 75%;
  }

  .profile-logos {
    flex: 1;
    display: grid; 
    grid-template-columns: 1fr 1fr;
    gap: 2px;
    align-items: center; 
    justify-items: center;
  }

  .profile-logos a:nth-child(1) {
    grid-column: 1 / -1;
    margin-bottom: 1px;
  }

  .profile-logos img {
    max-width: 75px;
    max-height: 75px;
    width: auto;
    object-fit: contain;
    transition: transform 0.2s;
    display: block;
    box-shadow: none;
  }

  .profile-logos img:hover {
    transform: scale(1.1);
  }

  .greedy-nav button {
    display: none !important;
  }

  .pie-chart-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    margin-top: 1em;
  }

  .pie-card {
    background: #fafafa;
    border: 1px solid #eeeeee;
    border-radius: 14px;
    padding: 12px 14px;
    box-shadow: 0 3px 8px rgba(0,0,0,0.06);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .pie-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(0,0,0,0.10);
  }

  .stats-chart {
    width: 100%;
    height: 360px;
  }

  @media (max-width: 1024px) {
    .stats-chart {
      height: 320px;
    }
  }

  @media (max-width: 768px) {
    .pie-chart-grid {
      grid-template-columns: 1fr;
    }

    .stats-chart {
      height: 300px;
    }

    .profile-wrapper {
      flex-direction: column;
      align-items: flex-start;
    }

    .profile-content {
      width: 100%;
    }

    .profile-logos {
      width: 100%;
      justify-items: start;
      grid-template-columns: repeat(3, auto);
      gap: 10px;
    }

    .profile-logos a:nth-child(1) {
      grid-column: auto;
      margin-bottom: 0;
    }

    .publication-container {
      flex-direction: column;
    }

    .publication-container img {
      max-width: 100%;
      height: auto;
    }
  }

  @media (max-width: 480px) {
    .stats-chart {
      height: 260px;
    }
  }
</style>


### 👨‍🎓Profile

<div class="profile-wrapper">
  <div class="profile-content">
    <span style="font-family:Arial; font-size:0.8em; text-align:justify;">
      I am currently a Ph.D. student at Southeast University, under the supervision of 
      <a href="https://jyh-learning.github.io" style="color:#4B0082;"><strong>Assoc. Prof. Yuheng Jia</strong></a>. 
      I received my M.S. degree from Henan University in 2023, under the supervision of 
      <a href="https://cs.henu.edu.cn/info/1273/5566.htm" style="color:#4B0082;"><strong>Prof. Chongsheng Zhang</strong></a>. 
      Before that, I obtained my B.S. degree in 2020 from Henan Institute of Engineering. 
      My research interests lie in machine learning, with a focus on long-tailed learning and weakly supervised learning.
    </span>
  </div>

  <div class="profile-logos">
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


### 🔥News

<div class="news-box">
  <span style="font-family:Arial; font-size:0.8em;">
    <div class="news-item">🎉 <span style="color:#4B0082;"><strong>[2026.01]</strong></span> Our work "Samples Are Not Equal: A Sample Selection Approach for Deep Clustering" is accepted by ICLR 2026! <a href="https://iclr.cc/virtual/2026/poster/10009380" style="color:#00308B;">Paper</a> <a href="https://github.com/notoaudrey/Samples-Are-Not-Equal">Codes</a><br></div>
    <div class="news-item">🎉 <span style="color:#4B0082;"><strong>[2025.11]</strong></span> Our work "DiCaP: Distribution-Calibrated Pseudo-labeling for Semi-Supervised Multi-Label Learning" is accepted by AAAI 2026! <a href="https://ojs.aaai.org/index.php/AAAI/article/view/39302" style="color:#00308B;">Paper</a> <a href="https://github.com/hb-studying/DiCaP">Codes</a><br></div>
    <div class="news-item">🎉 <span style="color:#4B0082;"><strong>[2025.10]</strong></span> Win National Scholarship for Ph.D. Student!<br></div>
    <div class="news-item">🎉 <span style="color:#4B0082;"><strong>[2025.09]</strong></span> Our work "Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning" is accepted by NeurIPS 2025! <a href="https://neurips.cc/virtual/2025/loc/san-diego/poster/116160" style="color:#00308B;">Paper</a> <a href="https://github.com/YaxinHou/CPG">Codes</a><br></div>
    <div class="news-item">🎉 <span style="color:#4B0082;"><strong>[2025.05]</strong></span> Our work "A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning" is accepted by ICML 2025! <a href="https://icml.cc/virtual/2025/poster/44441" style="color:#00308B;">Paper</a> <a href="https://github.com/YaxinHou/Meta-Expert">Codes</a><br></div>
  </span>
</div>


### 📊 Publication Statistics

<span style="font-family:Arial; font-size:0.8em; text-align:justify;">
A brief overview of my publications by venue, including accepted and published papers listed on this homepage.
</span>

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
  const conferenceChart = echarts.init(
    document.getElementById('conference-chart'),
    null,
    { renderer: 'svg' }
  );

  const journalChart = echarts.init(
    document.getElementById('journal-chart'),
    null,
    { renderer: 'svg' }
  );

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

  const mutedColorsConference = ['#6E6AA7', '#8B86C9', '#A7A3D8', '#C3C0E8'];
  const mutedColorsJournal = ['#7D84B2', '#A9B4C2', '#C7D3DD', '#DCE2EA'];

  function buildPieOption(titleText, total, data, colors) {
    const isMobile = window.innerWidth <= 768;
    const isTinyScreen = window.innerWidth <= 480;

    return {
      tooltip: {
        trigger: 'item',
        formatter: '{b}: {c} ({d}%)',
        backgroundColor: 'rgba(255,255,255,0.97)',
        borderColor: '#e5e5e5',
        borderWidth: 1,
        textStyle: {
          color: '#222',
          fontFamily: 'Arial, sans-serif'
        }
      },

      legend: {
        top: 10,
        left: 'center',
        orient: 'horizontal',
        itemWidth: isMobile ? 10 : 12,
        itemHeight: isMobile ? 10 : 12,
        icon: 'circle',
        textStyle: {
          color: '#444',
          fontSize: isTinyScreen ? 10 : (isMobile ? 11 : 12),
          fontFamily: 'Arial, sans-serif'
        }
      },

      graphic: [
        {
          type: 'text',
          left: 'center',
          top: isMobile ? '47%' : '50%',
          style: {
            text: titleText,
            textAlign: 'center',
            fill: '#6b6b78',
            fontSize: isTinyScreen ? 11 : (isMobile ? 12 : 14),
            fontWeight: 600,
            fontFamily: 'Arial, sans-serif'
          }
        },
        {
          type: 'text',
          left: 'center',
          top: isMobile ? '54%' : '57%',
          style: {
            text: String(total),
            textAlign: 'center',
            fill: '#2f2f3a',
            fontSize: isTinyScreen ? 18 : (isMobile ? 20 : 24),
            fontWeight: 700,
            fontFamily: 'Arial, sans-serif'
          }
        }
      ],

      series: [
        {
          name: titleText + ' Papers',
          type: 'pie',
          radius: isTinyScreen ? ['38%', '54%'] : (isMobile ? ['42%', '60%'] : ['48%', '67%']),
          center: isTinyScreen ? ['50%', '62%'] : (isMobile ? ['50%', '60%'] : ['50%', '58%']),
          avoidLabelOverlap: true,
          minShowLabelAngle: 10,
          itemStyle: {
            borderColor: '#fafafa',
            borderWidth: 3
          },
          label: {
            show: true,
            position: 'outside',
            formatter: isMobile ? '{b}\n{c}' : '{b}: {c}',
            color: '#555',
            fontSize: isTinyScreen ? 9 : (isMobile ? 10 : 12),
            fontWeight: 600,
            fontFamily: 'Arial, sans-serif'
          },
          labelLine: {
            show: true,
            length: isTinyScreen ? 4 : (isMobile ? 6 : 8),
            length2: isTinyScreen ? 3 : (isMobile ? 4 : 6),
            lineStyle: {
              color: '#b8b8c6'
            }
          },
          emphasis: {
            scale: true,
            scaleSize: 4
          },
          data: data,
          color: colors
        }
      ]
    };
  }

  function renderCharts() {
    conferenceChart.setOption(
      buildPieOption('Conference', conferenceTotal, conferenceData, mutedColorsConference),
      true
    );

    journalChart.setOption(
      buildPieOption('Journal', journalTotal, journalData, mutedColorsJournal),
      true
    );

    conferenceChart.resize();
    journalChart.resize();
  }

  renderCharts();

  let resizeTimer = null;
  window.addEventListener('resize', function () {
    clearTimeout(resizeTimer);
    resizeTimer = setTimeout(() => {
      renderCharts();
    }, 150);
  });
</script>


### 📝Publications

<span style="font-family:Arial; font-size:0.8em; text-align:justify;">
  Papers are listed below, in descending order by year of submission before they are published, or year of publication. Generally, the codes of all the papers will be available. For the full list, please refer to my 
  <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=-0IuShsAAAAJ" style="color:#00308B;">Google Scholar</a> page.
</span>

<ul style="margin-top: 0.1em; margin-bottom: 0.1em; font-family:Arial; font-size:0.9em;">
  <li><strong>Conference Papers</strong></li>
</ul>

<div class="publication-container">
  <div class="pub-img-wrapper">
    <div class="paper-badge">CCF A</div>
    <img src="./images/CPG.png" alt="Publication Image">
  </div>
  <div>
    <span style="color: #00308B; font-weight: bold">[NeurIPS 2025]</span> Keep It on a Leash: Controllable Pseudo-label Generation Towards Realistic Long-Tailed Semi-Supervised Learning.
    <br>
    <strong style="color:#4B0082;">Yaxin Hou</strong>, Bo Han, Yuheng Jia, Hui Liu, Junhui Hou.
  </div>
</div>

<div class="publication-container">
  <div class="pub-img-wrapper">
    <div class="paper-badge">CCF A</div>
    <img src="./images/Meta-Expert.png" alt="Publication Image">
  </div>
  <div>
    <span style="color: #00308B; font-weight: bold">[ICML 2025]</span> A Square Peg in a Square Hole: Meta-Expert for Long-Tailed Semi-Supervised Learning.
    <br>
    <strong style="color:#4B0082;">Yaxin Hou</strong>, Yuheng Jia.
  </div>
</div>

<div class="publication-container">
  <div class="pub-img-wrapper">
    <div class="paper-badge">CCF A</div>
    <img src="./images/QAST.png" alt="Publication Image">
  </div>
  <div>
    <span style="color: #00308B; font-weight: bold">[AAAI 2023]</span> Quality-Aware Self-Training on Differentiable Synthesis of Rare Relational Data.
    <br>
    Chongsheng Zhang, <strong style="color:#4B0082;">Yaxin Hou</strong>, Ke Chen, Shuang Cao, Gaojuan Fan, Ji Liu.
  </div>
</div>

<ul style="margin-top: 0.1em; margin-bottom: 0.1em; font-family:Arial; font-size:0.9em;">
  <li><strong>Journal Papers</strong></li>
</ul>

<div class="publication-container">
  <div class="pub-img-wrapper">
    <div class="paper-badge">CCF B</div>
    <img src="./images/imFTP.png" alt="Publication Image">
  </div>
  <div>
    <span style="color: #00308B; font-weight: bold">[Inf. Sci. 2024]</span> imFTP: Deep imbalance learning via fuzzy transition and prototypical learning.
    <br>
    <strong style="color:#4B0082;">Yaxin Hou</strong>, Weiping Ding, Chongsheng Zhang.
  </div>
</div>


### 👨‍💻Professional Services

<ul style="margin-top: 0.1em; margin-bottom: 0.1em; font-family:Arial; font-size:0.9em;">
  <li><strong>Conference Reviewer/Program Committee Member</strong></li>
  <ul style="margin-top: 0.1em; margin-bottom: 0.1em; padding-left: 1em; font-family:Arial; font-size:0.8em;">
    <li>The International Conference on Machine Learning (ICML), 2026.</li>
    <li>The European Conference on Computer Vision (ECCV), 2026.</li>
    <li>The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026.</li>
    <li>The Annual Conference on Neural Information Processing Systems (NeurIPS), 2025.</li>
    <li>The IEEE International Symposium on Machine Learning and Media Computing (MLMC), 2025-2026.</li>
  </ul>

  <li><strong>Journal Reviewer</strong></li>
  <ul style="margin-top: 0.1em; margin-bottom: 0.1em; padding-left: 1em; font-family:Arial; font-size:0.8em;">
    <li>International Journal of Machine Learning and Cybernetics (IJMLC).</li>
    <li>Transactions on Machine Learning Research (TMLR).</li>
    <li>Pattern Recognition (PR).</li>
  </ul>
</ul>


### 🏆Honors/Awards

<ul style="margin-top: 0.1em; margin-bottom: 0.1em; font-family:Arial; font-size:0.9em;">
  <li><strong>Scholarship</strong></li>
  <ul style="margin-top: 0.1em; margin-bottom: 0.1em; padding-left: 1em; font-family:Arial; font-size:0.8em;">
    <li>National Scholarship (2025, The Chinese Ministry of Education).</li>
    <li>Master's Academic Scholarship (2020, The Henan Department of Education).</li>
    <li>National Encouragement Scholarship (2019, The Henan Department of Education).</li>
    <li>National Encouragement Scholarship (2017, The Henan Department of Education).</li>
  </ul>

  <li><strong>Honor</strong></li>
  <ul style="margin-top: 0.1em; margin-bottom: 0.1em; padding-left: 1em; font-family:Arial; font-size:0.8em;">
    <li>Merit Graduate Student (2025, Southeast University).</li>
    <li>Outstanding Graduate Student (2023, Henan University).</li>
    <li>Outstanding Graduate (2020, The Henan Department of Education).</li>
    <li>Merit Student (2020, The Henan Department of Education).</li>
  </ul>
</ul>


### 📧Contact

<span style="font-family:Arial; font-size:0.8em; text-align:justify;">
  Room 1009, Liberal Arts Building. School of Computer Science and Engineering.
</span>

<div style="display: flex; justify-content: center; align-items: center; width: 100%; margin: 20px 0;">
  <div style="width: 100%; max-width: 300px; text-align: center;">
    <div style="width: 100%; max-height: 300px; overflow: hidden; border-radius: 8px;">
      <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=4D0h1VqEfuXzDioG4SfurpFAjXyS5BKdHFuIwYdKIHE&cl=ffffff&w=a"></script>
    </div>
  </div>
</div>
