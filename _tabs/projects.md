---
layout: default
title: "PROJECTS"
icon: fas fa-rocket
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projects Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

:root {
            --dark-bg: #0f172a;
            --card-bg: #1e293b;
            --accent: #3b82f6;
            --accent-hover: #2563eb;
            --text-primary: #f1f5f9;
            --text-secondary: #94a3b8;
            --success: #10b981;
            --warning: #f59e0b;
            --border: #334155;
            --gradient: linear-gradient(135deg, #6366f1, #3b82f6);
            --shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }

body {
            background: var(--dark-bg);
            color: var(--text-primary);
            line-height: 1.6;
            min-height: 100vh;
            padding: 2rem 1rem;
        }

 .container {
            max-width: 1200px;
            margin: 0 auto;
        }

header {
            text-align: center;
            margin-bottom: 3rem;
            padding: 2rem 0;
        }
 .header-content {
            display: inline-flex;
            align-items: center;
            gap: 1rem;
            background: rgba(30, 41, 59, 0.7);
            padding: 1rem 2rem;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid var(--border);
        }

 h1 {
            font-size: 2.5rem;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 0.5rem;
        }

.subtitle {
            color: var(--text-secondary);
            font-size: 1.1rem;
        }

 .icon {
            font-size: 2rem;
            color: var(--accent);
        }

 .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(500px, 1fr));
            gap: 2rem;
        }

.project-card {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 2rem;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }

 .project-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: var(--gradient);
        }

.project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4);
        }

  .project-header {
            display: flex;
            align-items: center;
            margin-bottom: 1.5rem;
            gap: 1rem;
        }

.project-icon {
            font-size: 2rem;
            background: var(--gradient);
            width: 60px;
            height: 60px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

.project-title {
            font-size: 1.5rem;
            font-weight: 700;
        }

 .section-title {
            color: var(--accent);
            font-size: 1.1rem;
            margin: 1.5rem 0 0.5rem 0;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

.tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin: 1rem 0;
        }

 .tech-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            background: rgba(30, 41, 59, 0.8);
            padding: 0.5rem 1rem;
            border-radius: 8px;
            border: 1px solid var(--border);
            transition: all 0.3s ease;
        }

.tech-item:hover {
            background: rgba(56, 70, 94, 0.8);
            transform: translateY(-2px);
        }

 .tech-item img {
            border-radius: 4px;
        }

.description {
            color: var(--text-secondary);
            margin: 1rem 0;
            line-height: 1.7;
        }

 .links {
            display: flex;
            gap: 1rem;
            margin: 1.5rem 0;
            flex-wrap: wrap;
        }

.btn {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.7rem 1.5rem;
            background: var(--gradient);
            color: white;
            text-decoration: none;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }

.btn:hover {
            background: linear-gradient(135deg, #4f46e5, #2563eb);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(37, 99, 235, 0.4);
        }

 .btn-outline {
            background: transparent;
            border: 1px solid var(--accent);
            color: var(--accent);
        }

 .btn-outline:hover {
            background: rgba(59, 130, 246, 0.1);
        }

.metrics {
            background: rgba(30, 41, 59, 0.7);
            padding: 1rem;
            border-radius: 10px;
            margin: 1rem 0;
            border-left: 4px solid var(--accent);
        }

 .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 0.8rem;
            margin: 1rem 0;
        }

.feature {
            display: flex;
            align-items: center;
            gap: 0.7rem;
            padding: 0.7rem;
            background: rgba(30, 41, 59, 0.5);
            border-radius: 8px;
            transition: background 0.3s ease;
        }

 .feature:hover {
            background: rgba(56, 70, 94, 0.5);
        }

.feature-icon {
            color: var(--success);
            font-size: 1.2rem;
        }

 @media (max-width: 768px) {
            .projects-grid {
                grid-template-columns: 1fr;
            }
            
.project-card {
                padding: 1.5rem;
            }
            
.header-content {
                flex-direction: column;
                text-align: center;
            }
            
 h1 {
                font-size: 2rem;
            }
        }

  /* Animation for cards */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

.project-card {
            animation: fadeInUp 0.5s ease forwards;
        }

 .project-card:nth-child(2) {
            animation-delay: 0.2s;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="header-content">
                <i class="fas fa-rocket icon"></i>
                <div>
                    <h1>PROJECTS</h1>
                    <p class="subtitle">Showcasing my data analysis and visualization projects</p>
                </div>
            </div>
        </header>

<div class="projects-grid">
            <!-- Titanic EDA Project -->
            <div class="project-card">
                <div class="project-header">
                    <div class="project-icon">
                        <i class="fas fa-chart-bar"></i>
                    </div>
                    <h2 class="project-title">Exploratory Titanic Dataset EDA</h2>
                </div>

<div class="section-title">
                      <i class="fas fa-tools"></i>
                      <span>Tech Stack</span>
                  </div>
                  <div class="tech-stack">
 <div class="tech-item">
                          <img src="https://www.python.org/static/community_logos/python-logo.png" width="26" alt="Python">
                          <span>Python</span>
                      </div>
                      <div class="tech-item">
                          <img src="https://upload.wikimedia.org/wikipedia/commons/e/ed/Pandas_logo.svg" width="26" alt="Pandas">
                          <span>Pandas</span>
</div>
                      <div class="tech-item">
                          <img src="https://matplotlib.org/_static/images/logo2.svg" width="26" alt="Matplotlib">
                          <span>Matplotlib</span>
                      </div>
 <div class="tech-item">
                          <img src="https://seaborn.pydata.org/_static/logo-wide-lightbg.svg" width="26" alt="Seaborn">
                          <span>Seaborn</span>
                      </div>
                  </div>
  
<div class="section-title">
                      <i class="fas fa-file-alt"></i>
                      <span>Description</span>
                  </div>
  <p class="description">
                    Performed in-depth analysis of the Titanic dataset to uncover survival trends based on gender, class, and age. Created visualizations and derived insights to understand the factors that influenced passenger survival rates.
                </p>

<div class="section-title">
                    <i class="fas fa-external-link-alt"></i>
                    <span>Repo / Demo</span>
                </div>
<div class="links">
                    <a href="https://www.kaggle.com/code/weldonsitienei/weldon-kipkoech-eda" class="btn" target="_blank">
                        <i class="fas fa-globe"></i> View on Kaggle
                    </a>
                </div>
            </div>

            <!-- Hotel Dashboard Project -->
 <div class="project-card">
                <div class="project-header">
                    <div class="project-icon">
                        <i class="fas fa-hotel"></i>
                    </div>
                    <h2 class="project-title">Hotel Performance Analytics Dashboard</h2>
                </div>

<div class="section-title">
                    <i class="fas fa-tools"></i>
                    <span>Tech Stack</span>
                </div>
<div class="tech-stack">
                    <div class="tech-item">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/c/cf/New_Power_BI_Logo.svg" width="26" alt="Power BI">
                        <span>Power BI</span>
                    </div>
                </div>

 <div class="section-title">
                    <i class="fas fa-file-alt"></i>
                    <span>Description</span>
                </div>
  <p class="description">
                    A visually rich dashboard analyzing hotel revenue, occupancy, performance metrics, and operational KPIs for multiple luxury properties. Includes insights on ADR, RevPAR, cancellations, and realization rates.
                </p>

<div class="section-title">
                    <i class="fas fa-external-link-alt"></i>
                    <span>Project Links</span>
                </div>
  <div class="links">
                    <a href="https://www.kaggle.com/code/weldonsitienei/Business-Intelligence_POWER-BI" class="btn" target="_blank">
                        <i class="fas fa-chart-bar"></i> View on Kaggle
                    </a>
                    <a href="https://drive.google.com/file/d/1LxvqWB4g5RawkIOVFaLrMnh07KIFDw0N/view?usp=drive_link" class="btn btn-outline" target="_blank">
                        <i class="fas fa-download"></i> Download PBIX
                    </a>
                </div>

                
  <div class="section-title">
                    <i class="fas fa-chart-line"></i>
                    <span>Metrics Covered</span>
                </div>
                <div class="metrics">
                    ADR, RevPAR, DBRN, DSRN, DURN, Cancellation & Realization Rates
                </div>

  <div class="section-title">
                    <i class="fas fa-star"></i>
                    <span>Key Features</span>
                </div>
                <div class="features">
                    <div class="feature">
                        <i class="fas fa-chart-bar feature-icon"></i>
                        <span><strong>1.68B Revenue</strong> analyzed</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-bed feature-icon"></i>
                        <span><strong>57.79%</strong> Occupancy Rate</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-dollar-sign feature-icon"></i>
                        <span><strong>12,696</strong> Average Daily Rate</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-percentage feature-icon"></i>
                        <span><strong>70.14%</strong> Realization Rate</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-sliders-h feature-icon"></i>
                        <span><strong>Interactive filters</strong></span>
                    </div>
                     <div class="feature">
                        <i class="fas fa-building feature-icon"></i>
                        <span><strong>6+ Luxury Properties</strong></span>
                    </div>
                </div>
            </div>
        </div>
    </div>

<script>
        // Add subtle animation on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const projectCards = document.querySelectorAll('.project-card');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
             projectCards.forEach(card => {
                card.style.opacity = '0';
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
