---
layout: default
title: "PROJECTS"
icon: fas fa-rocket
---

<div class="container" role="main">
    <header class="site-header" aria-hidden="false">
      <div class="logo-badge">🚀</div>
      <div>
        <h1 class="title">PROJECTS</h1>
        <p class="lead">Selected work — data analytics, Power BI dashboards and visualizations.</p>
      </div>
    </header>
  <section class="projects-grid" aria-label="Projects list">
<!-- Titanic Card -->
    <article class="card" id="titanic">
  <div class="card-head">
          <div style="display:flex;flex-direction:column;">
            <h2>📊 Exploratory Titanic Dataset EDA</h2>
            <div class="chip">Exploratory Data Analysis • EDA</div>
          </div>
        </div>

<div class="tech-list" aria-hidden="false" style="margin-top:8px;">
  <div class="tech-item"><img src="https://www.python.org/static/community_logos/python-logo.png" width="20" alt="Python logo"/> Python</div>
  <div class="tech-item"><img src="https://upload.wikimedia.org/wikipedia/commons/e/ed/Pandas_logo.svg" width="20" alt="Pandas logo"/> Pandas</div>
  <div class="tech-item"><img src="https://matplotlib.org/_static/images/logo2.svg" width="20" alt="Matplotlib logo"/> Matplotlib</div>
  <div class="tech-item"><img src="https://seaborn.pydata.org/_static/logo-wide-lightbg.svg" width="20" alt="Seaborn logo"/> Seaborn</div>
</div>


  <p class="desc">
          <strong>📝 Description:</strong><br>
          Performed in-depth analysis of the Titanic dataset to uncover survival trends based on gender, class, and age. Created visualizations and derived actionable insights to inform model building and storytelling.
        </p>

  <div class="links">
          <a class="btn" href="https://www.kaggle.com/code/weldonsitienei/weldon-kipkoech-eda" target="_blank" rel="noopener noreferrer">🌐 View on Kaggle</a>
          <a class="btn secondary" href="#titanic-details" onclick="document.getElementById('titanic-details').scrollIntoView({behavior:'smooth'});return false;">🔎 Read details</a>
        </div>
      </article>
 <!-- Hotel Card -->
      <article class="card" id="hotel">
        <div class="card-head">
          <div style="display:flex;flex-direction:column;">
            <h2>🏨 Hotel Performance Analytics Dashboard</h2>
            <div class="chip">Power BI • Hospitality Analytics</div>
          </div>
        </div>

<div class="tech-list" style="margin-top:8px;">
          <div class="tech-item"><img src="https://upload.wikimedia.org/wikipedia/commons/c/cf/New_Power_BI_Logo.svg" alt="Power BI"/> Power BI</div>
        </div>

  <p class="desc">
          <strong>📝 Description:</strong><br>
          A visually rich Power BI dashboard analyzing hotel revenue, occupancy, performance metrics, and operational KPIs for multiple luxury properties. Includes ADR, RevPAR, cancellations, and realization-rate insights.
        </p>

  <div class="metric-list" aria-hidden="false">
          <div class="metric">📊 <span class="kpi">1.68B Revenue</span></div>
          <div class="metric">🏨 <span class="kpi">57.79% Occupancy</span></div>
          <div class="metric">💰 <span class="kpi">12,696 ADR</span></div>
          <div class="metric">⭐ <span class="kpi">70.14% Realization</span></div>
        </div>

   <div class="links">
          <a class="btn" href="https://www.kaggle.com/code/weldonsitienei/Business-Intelligence_POWER-BI" target="_blank" rel="noopener noreferrer">📊 View on Kaggle</a>
          <a class="btn" href="https://drive.google.com/file/d/1LxvqWB4g5RawkIOVFaLrMnh07KIFDw0N/view?usp=drive_link" target="_blank" rel="noopener noreferrer">💾 Download PBIX</a>
          <a class="btn secondary" href="#hotel-details" onclick="document.getElementById('hotel-details').scrollIntoView({behavior:'smooth'});return false;">📈 Metrics</a>
        </div>
      </article>

 </section>

<!-- Expanded details section (optional anchors for the 'read details' buttons) -->
<main style="margin-top:36px; display:grid; gap:18px;">
      <section id="titanic-details" class="card" aria-label="Titanic details">
        <h3 style="margin:0 0 8px 0;">📊 Exploratory Titanic Dataset EDA — Details</h3>
        <p class="desc" style="margin-bottom:8px;">
          <strong>Focus:</strong> Survival analysis by gender, class, age; feature exploration for later classification models; clear visual storytelling for stakeholders.
        </p>

  <div class="metric-list" style="margin-bottom:12px;">
          <div class="metric">🔬 <span class="kpi">Data Cleaning</span></div>
          <div class="metric">📈 <span class="kpi">EDA & Visuals</span></div>
          <div class="metric">🤖 <span class="kpi">Prep for ML</span></div>
        </div>

  <p class="desc">
          **Repo / Demo:** <a href="https://www.kaggle.com/code/weldonsitienei/weldon-kipkoech-eda" target="_blank" rel="noopener noreferrer">Kaggle Notebook</a>
        </p>
      </section>

  <section id="hotel-details" class="card" aria-label="Hotel details">
        <h3 style="margin:0 0 8px 0;">🏨 Hotel Performance Analytics Dashboard — Details</h3>

  <p class="desc" style="margin-bottom:6px;"><strong>⭐ Metrics Covered:</strong> ADR, RevPAR, DBRN, DSRN, DURN, Cancellation & Realization Rates</p>

  <ul style="margin-top:6px;color:var(--muted);line-height:1.6">
          <li>📊 <strong>1.68B Revenue</strong> analyzed across multiple properties</li>
          <li>🏨 <strong>57.79% Average Occupancy Rate</strong></li>
          <li>💰 <strong>12,696 Average Daily Rate (ADR)</strong></li>
          <li>⭐ <strong>70.14% Realization Rate</strong></li>
          <li>📈 Interactive filters for city, room type, and date ranges</li>
          <li>🏢 6+ Luxury Hotel Properties analyzed</li>
        </ul>

  <p class="desc" style="margin-top:8px;">
          **Links:** <a href="https://www.kaggle.com/code/weldonsitienei/Business-Intelligence_POWER-BI" target="_blank" rel="noopener noreferrer">View on Kaggle</a> • <a href="https://drive.google.com/file/d/1LxvqWB4g5RawkIOVFaLrMnh07KIFDw0N/view?usp=drive_link" target="_blank" rel="noopener noreferrer">Download PBIX</a>
        </p>
      </section>
    </main>

  </div>



