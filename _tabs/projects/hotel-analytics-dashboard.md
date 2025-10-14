<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hotel Analytics Dashboard</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

   :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --success: #2ecc71;
            --warning: #f39c12;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --gradient: linear-gradient(135deg, #3498db, #2c3e50);
            --shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: var(--dark);
            line-height: 1.6;
            min-height: 100vh;
            padding-bottom: 2rem;
        }

.container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

header {
            background: var(--gradient);
            color: white;
            padding: 3rem 0;
            text-align: center;
            border-radius: 0 0 20px 20px;
            margin-bottom: 2rem;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }
 header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 L100,0 L100,100 Z" fill="rgba(255,255,255,0.1)"/></svg>');
            background-size: cover;
        }

h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }

.tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }
.dashboard-section {
            background: white;
            border-radius: 15px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: var(--shadow);
            transition: transform 0.3s ease;
        }

  .dashboard-section:hover {
            transform: translateY(-5px);
        }

  h2 {
            color: var(--primary);
            margin-bottom: 1.5rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid var(--light);
            display: flex;
            align-items: center;
        }

h2 i {
            margin-right: 10px;
            color: var(--secondary);
        }

 .download-cta {
            background: linear-gradient(135deg, var(--success), #27ae60);
            color: white;
            text-align: center;
            padding: 2rem;
            border-radius: 15px;
            margin: 2rem 0;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }

  .download-cta::before {
            content: "";
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.2) 0%, transparent 70%);
            transform: rotate(30deg);
        }

  .cta-button {
            display: inline-block;
            background: white;
            color: var(--success);
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 1rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

 .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
        }

   .metrics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
            margin: 1.5rem 0;
        }

 .metric-card {
            background: white;
            border-radius: 10px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border-top: 4px solid var(--secondary);
            transition: all 0.3s ease;
        }

.metric-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
        }

.metric-value {
            font-size: 1.8rem;
            font-weight: bold;
            margin: 10px 0;
            color: var(--primary);
        }

 .metric-performance {
            display: inline-block;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
        }

.performance-excellent {
            background: rgba(46, 204, 113, 0.2);
            color: var(--success);
        }

 .performance-strong {
            background: rgba(52, 152, 219, 0.2);
            color: var(--secondary);
        }

 .performance-good {
            background: rgba(243, 156, 18, 0.2);
            color: var(--warning);
        }

.performance-optimal {
            background: rgba(155, 89, 182, 0.2);
            color: #9b59b6;
        }

 .performance-manageable {
            background: rgba(149, 165, 166, 0.2);
            color: #95a5a6;
        }

 .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
        }

   .feature-card {
            background: var(--light);
            border-radius: 10px;
            padding: 1.5rem;
            border-left: 4px solid var(--secondary);
        }

 .feature-card h3 {
            margin-bottom: 0.5rem;
            color: var(--primary);
        }

 .properties-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 1rem;
        }

 .property-card {
            background: white;
            border-radius: 10px;
            padding: 1.2rem;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
            border: 1px solid #eee;
            transition: all 0.3s ease;
        }

 .property-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

 .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 1rem;
        }

 .tech-item {
            background: var(--gradient);
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
        }

 .tech-item i {
            margin-right: 5px;
        }

.kpi-container {
            background: var(--light);
            border-radius: 10px;
            padding: 1.5rem;
            font-family: 'Courier New', monospace;
            margin-top: 1rem;
            overflow-x: auto;
        }

.kpi-line {
            margin: 8px 0;
            display: flex;
            align-items: center;
        }

.kpi-line i {
            margin-right: 10px;
            width: 20px;
        }

 footer {
            text-align: center;
            margin-top: 3rem;
            padding: 1.5rem;
            color: var(--dark);
            opacity: 0.7;
        }

 @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
.metrics-grid {
                grid-template-columns: 1fr;
            }
            
  .features-grid {
                grid-template-columns: 1fr;
            }
            
 .properties-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>🏨 Hotel Analytics Dashboard</h1>
            <p class="tagline">A Stunning Power BI Dashboard for Hotel Performance Intelligence</p>
        </div>
    </header>

<div class="container">
        <section class="download-cta">
            <h2>🎮 Interactive Dashboard Available!</h2>
            <p>Fully functional .pbix file ready for exploration</p>
            <a href="#" class="cta-button">📁 Download Power BI File</a>
        </section>

  <section class="dashboard-section">
            <h2><i class="fas fa-chart-line"></i> Executive Dashboard Highlights</h2>
            <div class="metrics-grid">
                <div class="metric-card">
                    <i class="fas fa-chart-bar fa-2x"></i>
                    <div class="metric-value">1.68B</div>
                    <div class="metric-title">Total Revenue</div>
                    <div class="metric-performance performance-excellent">Excellent</div>
                </div>
                <div class="metric-card">
                    <i class="fas fa-dollar-sign fa-2x"></i>
                    <div class="metric-value">12,696</div>
                    <div class="metric-title">Average ADR</div>
                    <div class="metric-performance performance-strong">Strong</div>
                </div>
                <div class="metric-card">
                    <i class="fas fa-bed fa-2x"></i>
                    <div class="metric-value">57.79%</div>
                    <div class="metric-title">Occupancy Rate</div>
                    <div class="metric-performance performance-good">Good</div>
                </div>
                <div class="metric-card">
                    <i class="fas fa-star fa-2x"></i>
                    <div class="metric-value">70.14%</div>
                    <div class="metric-title">Realization Rate</div>
                    <div class="metric-performance performance-optimal">Optimal</div>
                </div>
                <div class="metric-card">
                    <i class="fas fa-times-circle fa-2x"></i>
                    <div class="metric-value">24.84%</div>
                    <div class="metric-title">Cancellation Rate</div>
                    <div class="metric-performance performance-manageable">Manageable</div>
                </div>
            </div>
        </section>

<section class="dashboard-section">
            <h2><i class="fas fa-tachometer-alt"></i> Dashboard Features</h2>
            
  <h3>📊 Core Analytics</h3>
            <div class="features-grid">
                <div class="feature-card">
                    <h3>🎯 Revenue Intelligence</h3>
                    <p>Track 1.68B+ revenue across properties with detailed breakdowns and comparisons.</p>
                </div>
                <div class="feature-card">
                    <h3>📈 Occupancy Metrics</h3>
                    <p>Real-time DBRN, DSRN, DURN monitoring with historical trend analysis.</p>
                </div>
                <div class="feature-card">
                    <h3>💰 Rate Optimization</h3>
                    <p>ADR & RevPAR analysis by property, room type, and seasonality factors.</p>
                </div>
                <div class="feature-card">
                    <h3>📅 Trend Analysis</h3>
                    <p>Weekly performance across 12+ weeks with forecasting capabilities.</p>
                </div>
            </div>
            
 <h3 style="margin-top: 2rem;">🏨 Property Performance</h3>
            <div class="properties-grid">
                <div class="property-card">
                    <h4>🏰 Atliq Palace</h4>
                    <p>Revenue: 68M</p>
                    <div>⭐⭐⭐⭐</div>
                </div>
                <div class="property-card">
                    <h4>🌴 Atliq Bay</h4>
                    <p>Revenue: 81M</p>
                    <div>⭐⭐⭐⭐⭐</div>
                </div>
                <div class="property-card">
                    <h4>🌊 Atliq Blu</h4>
                    <p>Revenue: 72M</p>
                    <div>⭐⭐⭐⭐</div>
                </div>
                <div class="property-card">
                    <h4>🏙️ Atliq City</h4>
                    <p>Revenue: 81M</p>
                    <div>⭐⭐⭐⭐⭐</div>
                </div>
            </div>
        </section>

<section class="dashboard-section">
            <h2><i class="fas fa-layer-group"></i> Technical Stack</h2>
            <div class="tech-stack">
                <div class="tech-item"><i class="fas fa-desktop"></i> Power BI Desktop</div>
                <div class="tech-item"><i class="fas fa-calculator"></i> DAX</div>
                <div class="tech-item"><i class="fas fa-database"></i> Power Query</div>
                <div class="tech-item"><i class="fas fa-chart-pie"></i> Custom Charts</div>
                <div class="tech-item"><i class="fas fa-tachometer-alt"></i> KPIs</div>
                <div class="tech-item"><i class="fas fa-trend-up"></i> Trend Lines</div>
                <div class="tech-item"><i class="fas fa-hotel"></i> Revenue Management</div>
                <div class="tech-item"><i class="fas fa-chart-bar"></i> Performance Metrics</div>
            </div>
        </section>

<section class="dashboard-section">
            <h2><i class="fas fa-key"></i> Key Performance Indicators</h2>
            <div class="kpi-container">
                <div class="kpi-line"><i class="fas fa-bullseye"></i> ADR (Average Daily Rate) = 12,696</div>
                <div class="kpi-line"><i class="fas fa-dollar-sign"></i> RevPAR (Revenue per Available Room) = 7,337</div>
                <div class="kpi-line"><i class="fas fa-bed"></i> Occupancy % = 57.79%</div>
                <div class="kpi-line"><i class="fas fa-star"></i> Realisation % = 70.14%</div>
                <div class="kpi-line"><i class="fas fa-times-circle"></i> Cancellation % = 24.84%</div>
                <div class="kpi-line"><i class="fas fa-chart-bar"></i> DBRN (Daily Booked Room Nights) = 1,461</div>
                <div class="kpi-line"><i class="fas fa-home"></i> DSRN (Daily Sellable Room Nights) = 2,528</div>
                <div class="kpi-line"><i class="fas fa-check-circle"></i> DURN (Daily Utilized Room Nights) = 1,025</div>
            </div>
        </section>
    </div>

 <footer>
        <div class="container">
            <p>Hotel Analytics Dashboard &copy; 2023 | Transforming Data into Hotel Excellence</p>
        </div>
    </footer>

<script>
        // Add subtle animations to metric cards on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const metricCards = document.querySelectorAll('.metric-card');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            metricCards.forEach(card => {
                card.style.opacity = '0';
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
