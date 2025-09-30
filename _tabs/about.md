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
      --bg-color: #18181b;
      --container-bg: #22212a;
      --primary-color: #10b981;
      --accent-color: #818cf8;
      --text-color: #f3f4f6;
      --border-radius: 18px;
      --shadow: 0 4px 24px rgba(16,185,129,0.13);
      --secondary-bg: #26272b;
    }
    body {
      background: var(--bg-color);
      color: var(--text-color);
      font-family: "Segoe UI", "Roboto", "Arial", sans-serif;
      margin: 0;
      min-height: 100vh;
    }
    .about-container {
      background: var(--container-bg);
      border-radius: var(--border-radius);
      box-shadow: var(--shadow);
      margin: 2rem auto;
      padding: 2rem 2.5rem;
      max-width: 750px;
      border: 1px solid #26272b;
    }
    .about-header {
      color: var(--primary-color);
      font-size: 2.3rem;
      font-weight: 700;
      text-align: center;
      margin-bottom: 0.3rem;
      letter-spacing: 1px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 0.6em;
    }
    .about-header .fa-user {
      color: var(--accent-color);
      font-size: 1.6em;
    }
    .about-section {
      margin: 2rem 0 1.5rem 0;
      padding: 1.4rem 1rem;
      background: var(--secondary-bg);
      border-radius: 14px;
      box-shadow: 0 2px 8px rgba(129,140,248,0.08);
    }
    .about-section h2 {
      color: var(--primary-color);
      font-size: 1.23rem;
      margin-bottom: 0.7rem;
      letter-spacing: 1px;
    }
    .about-section ul, .skills-list {
      list-style: none;
      padding-left: 0;
      margin-bottom: 0;
    }
    .about-section li, .skills-list div {
      margin-bottom: 0.6em;
      position: relative;
      padding-left: 1.6em;
      color: var(--accent-color);
      font-size: 1rem;
    }
    .about-section li:before {
      content: "✅";
      color: var(--primary-color);
      position: absolute;
      left: 0;
      font-size: 1em;
    }
    .skills-list {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 0.6em 2em;
      margin-top: 0.5em;
    }
    .skill-icon {
      color: var(--primary-color);
      font-size: 1.12em;
      margin-right: 0.5em;
      vertical-align: middle;
      padding-left: 0;
    }
    .skill-label {
      color: var(--accent-color);
      font-weight: 500;
    }
    @media (max-width: 650px) {
      .about-container {
        padding: 1.2rem 0.6rem;
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
        I’m a passionate <span class="skill-label">Data Scientist</span> and <span class="skill-label">AI/ML Engineer</span> with hands-on experience in Deep Learning, software engineering, and data-driven problem solving.<br>
        I specialize in transforming raw data into intelligent systems that power insights, automation, and innovation.<br>
        I enjoy bridging the gap between data and intelligent systems—whether it’s model development, AI integration, or end-to-end product pipelines.<br>
        <b>Always exploring, always building.</b>
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
        <div><span class="skill-icon">🔹</span><span class="skill-label">Programming & Scripting:</span> Python, R, SQL</div>
        <div><span class="skill-icon">🔹</span><span class="skill-label">Data Analysis & Visualization:</span> Pandas, NumPy, Matplotlib, Seaborn, Excel, Power BI, Tableau</div>
        <div><span class="skill-icon">🔹</span><span class="skill-label">Machine Learning & Deep Learning:</span> Scikit-learn, TensorFlow, PyTorch, Keras, XGBoost</div>
        <div><span class="skill-icon">🔹</span><span class="skill-label">AI & NLP:</span> SpaCy, NLTK, Hugging Face, Transformers</div>
        <div><span class="skill-icon">🔹</span><span class="skill-label">Big Data & Databases:</span> MySQL, PostgreSQL, MongoDB, Spark</div>
        <div><span class="skill-icon">🔹</span><span class="skill-label">Deployment & Engineering:</span> Docker, Flask, FastAPI, Git/GitHub, AWS, GCP, Azure</div>
      </div>
    </div>
  </div>
</body>
</html>


