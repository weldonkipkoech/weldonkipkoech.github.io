---
title: ABOUT
icon: fas fa-user
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>About</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
  <style>
    :root {
      --theme-dark: #181c24;
      --container-bg: #202530;
      --primary: #2dd4bf;
      --accent: #f472b6;
      --text: #f3f4f6;
      --heading: #38bdf8;
      --card-bg: #232a35;
      --border-radius: 20px;
      --shadow: 0 4px 32px rgba(45,212,191,0.12);
      --badge-bg: #334155;
      --badge-text: #81e6d9;
    }
    body {
      background: var(--theme-dark);
      color: var(--text);
      font-family: "Segoe UI", "Roboto", "Arial", sans-serif;
      margin: 0;
      min-height: 100vh;
    }
    .about-container {
      background: var(--container-bg);
      border-radius: var(--border-radius);
      box-shadow: var(--shadow);
      margin: 2.2rem auto 2.2rem auto;
      padding: 2.2rem 2.8rem;
      max-width: 800px;
      border: 1.5px solid var(--primary);
      position: relative;
    }
    .about-header {
      color: var(--primary);
      font-size: 2.5rem;
      font-weight: bold;
      text-align: center;
      margin-bottom: 0.5rem;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 0.7em;
      letter-spacing: 1px;
      text-shadow: 0 2px 16px #09626e1a;
    }
    .about-header .fa-user {
      color: var(--accent);
      font-size: 1.8em;
    }
    .about-section {
      margin: 2.2rem 0 1.7rem 0;
      padding: 1.7rem 1.1rem;
      background: var(--card-bg);
      border-radius: 16px;
      box-shadow: 0 2px 12px rgba(45,212,191,0.09);
      border-left: 5px solid var(--primary);
      transition: background 0.3s;
    }
    .about-section h2 {
      color: var(--heading);
      font-size: 1.35rem;
      margin-bottom: 1rem;
      letter-spacing: 1px;
    }
    .about-section p {
      font-size: 1.07rem;
      line-height: 1.7;
    }
    .about-section ul {
      list-style: none;
      padding-left: 0;
      margin-bottom: 0;
    }
    .about-section li {
      margin-bottom: 1em;
      position: relative;
      padding-left: 2.1em;
      color: var(--accent);
      font-size: 1.06rem;
      font-weight: 500;
      transition: color 0.2s;
    }
    .about-section li:before {
      content: "🌈";
      color: var(--primary);
      position: absolute;
      left: 0;
      font-size: 1.2em;
      top: 2px;
    }
    .skills-list {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 0.8em 2em;
      margin-top: 0.7em;
    }
    .skill-badge {
      background: var(--badge-bg);
      color: var(--badge-text);
      display: inline-block;
      padding: 0.28em 0.9em;
      border-radius: 12px;
      font-size: 0.95em;
      margin-right: 0.6em;
      margin-bottom: 0.5em;
      font-weight: 600;
      letter-spacing: 0.5px;
      box-shadow: 0 1px 8px #0e74901a;
    }
    .skill-label {
      color: var(--primary);
      font-weight: 700;
      margin-right: 0.4em;
    }
    .skill-icon {
      color: var(--accent);
      margin-right: 0.4em;
      font-size: 1em;
    }
    @media (max-width: 800px) {
      .about-container {
        padding: 1.4rem 0.7rem;
      }
      .skills-list {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <div class="about-container">
    <div class="about-header">
      <i class="fas fa-user"></i>
      ABOUT
    </div>
    <div class="about-section">
      <h2>👋 About Me</h2>
      <p>
        I’m a passionate <span class="skill-badge">Data Scientist</span>
        and <span class="skill-badge">AI/ML Engineer</span> with hands-on experience in <span class="skill-badge">Deep Learning</span>,
        <span class="skill-badge">software engineering</span>, and data-driven problem solving.<br>
        I specialize in transforming raw data into intelligent systems that power insights, automation, and innovation.<br>
        I enjoy bridging the gap between data and intelligent systems—whether it’s model development, AI integration, or end-to-end product pipelines.<br>
        <span style="color:var(--accent);font-weight:700;">Always exploring, always building.</span>
      </p>
    </div>
    <div class="about-section">
      <h2>💡 My Strengths</h2>
      <ul>
        <li>Building and deploying Machine Learning and Deep Learning models</li>
        <li>Designing AI solutions for real-world applications</li>
        <li>Data preprocessing, visualization, and predictive analytics</li>
        <li>Software development practices for scalable AI systems</li>
        <li>Continuous learning and integrating cutting-edge tools in ML, DL, and Data Engineering</li>
      </ul>
    </div>
    <div class="about-section">
      <h2>🛠️ Tools & Technologies</h2>
      <div class="skills-list">
        <div>
          <span class="skill-icon">🔹</span>
          <span class="skill-label">Programming & Scripting:</span>
          <span class="skill-badge">Python</span>
          <span class="skill-badge">R</span>
          <span class="skill-badge">SQL</span>
        </div>
        <div>
          <span class="skill-icon">🔹</span>
          <span class="skill-label">Data Analysis & Visualization:</span>
          <span class="skill-badge">Pandas</span>
          <span class="skill-badge">NumPy</span>
          <span class="skill-badge">Matplotlib</span>
          <span class="skill-badge">Seaborn</span>
          <span class="skill-badge">Excel</span>
          <span class="skill-badge">Power BI</span>
          <span class="skill-badge">Tableau</span>
        </div>
        <div>
          <span class="skill-icon">🔹</span>
          <span class="skill-label">Machine Learning & Deep Learning:</span>
          <span class="skill-badge">Scikit-learn</span>
          <span class="skill-badge">TensorFlow</span>
          <span class="skill-badge">PyTorch</span>
          <span class="skill-badge">Keras</span>
          <span class="skill-badge">XGBoost</span>
        </div>
        <div>
          <span class="skill-icon">🔹</span>
          <span class="skill-label">AI & NLP:</span>
          <span class="skill-badge">SpaCy</span>
          <span class="skill-badge">NLTK</span>
          <span class="skill-badge">Hugging Face</span>
          <span class="skill-badge">Transformers</span>
        </div>
        <div>
          <span class="skill-icon">🔹</span>
          <span class="skill-label">Big Data & Databases:</span>
          <span class="skill-badge">MySQL</span>
          <span class="skill-badge">PostgreSQL</span>
          <span class="skill-badge">MongoDB</span>
          <span class="skill-badge">Spark</span>
        </div>
        <div>
          <span class="skill-icon">🔹</span>
          <span class="skill-label">Deployment & Engineering:</span>
          <span class="skill-badge">Docker</span>
          <span class="skill-badge">Flask</span>
          <span class="skill-badge">FastAPI</span>
          <span class="skill-badge">Git/GitHub</span>
          <span class="skill-badge">AWS</span>
          <span class="skill-badge">GCP</span>
          <span class="skill-badge">Azure</span>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
