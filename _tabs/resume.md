---
layout: "default"
title: "Here is my CV"
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Weldon Kipkoech — Data Scientist</title>

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#f4f7fb;
      --card:#ffffff;
      --muted:#6b7280;
      --accent:#0f62fe;
      --accent-2:#7c3aed;
      --glass: rgba(255,255,255,0.6);
      --radius: 14px;
      --maxw: 980px;
      --gutter: 20px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: "Roboto", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg, #eef4ff 0%, var(--bg) 100%);
      color:#111827;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:40px 20px;
      display:flex;
      justify-content:center;
    }

    .container{
      width:100%;
      max-width:var(--maxw);
      display:grid;
      grid-template-columns: 320px 1fr;
      gap:var(--gutter);
      align-items:start;
    }

    /* Sidebar card */
    .sidebar{
      background: var(--card);
      border-radius:var(--radius);
      padding:22px;
      box-shadow: 0 8px 30px rgba(12, 18, 31, 0.06);
      position:sticky;
      top:28px;
      height: fit-content;
    }

    .name{
      font-family: "Playfair Display", serif;
      font-size:1.6rem;
      margin:0 0 6px 0;
      letter-spacing:0.2px;
    }
    .role{
      color:var(--muted);
      margin:0 0 14px 0;
      font-weight:700;
    }

    .contact{
      font-size:0.95rem;
      color:var(--muted);
      display:flex;
      flex-direction:column;
      gap:8px;
      margin-bottom:14px;
    }
    .contact a{
      color:inherit;
      text-decoration:none;
    }

    .meta-btns{
      display:flex;
      gap:8px;
      margin-top:12px;
    }
    .btn{
      border:0;
      padding:8px 10px;
      border-radius:9px;
      cursor:pointer;
      font-weight:600;
      font-size:0.9rem;
      background: linear-gradient(90deg,var(--accent),var(--accent-2));
      color:white;
      box-shadow:0 6px 18px rgba(15,98,254,0.14);
    }
    .btn.secondary{
      background:transparent;
      color:var(--accent);
      border:1px solid rgba(15,98,254,0.12);
      box-shadow:none;
    }

    .section-title{
      font-weight:700;
      margin:18px 0 8px 0;
      font-size:0.95rem;
      color:#111827;
    }

    ul.list{
      margin:0;
      padding:0 0 0 16px;
      color:var(--muted);
    }
    ul.list li{margin-bottom:8px}

    /* Main card */
    .main{
      background: var(--card);
      border-radius:var(--radius);
      padding:28px;
      box-shadow: 0 8px 30px rgba(12, 18, 31, 0.06);
    }

    .heading-row{
      display:flex;
      justify-content:space-between;
      gap:12px;
      align-items:start;
    }
    .title{
      margin:0;
      font-family:"Playfair Display", serif;
      font-size:1.4rem;
    }
    .subhead{
      margin:0;
      color:var(--muted);
      font-weight:700;
    }

    .summary{
      margin-top:14px;
      color:#374151;
      line-height:1.6;
      font-size:0.98rem;
    }

    /* Achievements */
    .achievements{
      display:grid;
      grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
      gap:14px;
      margin-top:18px;
    }
    .ach-card{
      background: linear-gradient(180deg, rgba(124,58,237,0.04), rgba(15,98,254,0.02));
      padding:12px;
      border-radius:10px;
      min-height:72px;
    }
    .ach-card p{margin:0; font-size:0.95rem; color:#111827}

    /* Experience timeline */
    .timeline{
      margin-top:18px;
      border-left:3px dashed rgba(17,24,39,0.06);
      padding-left:18px;
      padding-top:8px;
    }
    .role-item{
      margin-bottom:18px;
      position:relative;
    }
    .role-item:before{
      content:"";
      width:12px;
      height:12px;
      border-radius:50%;
      background:var(--accent);
      position:absolute;
      left:-29px;
      top:6px;
      box-shadow:0 6px 18px rgba(15,98,254,0.12);
    }
    .role-title{font-weight:700; margin:0; font-size:1rem}
    .role-meta{font-size:0.88rem; color:var(--muted); margin:6px 0}
    .role-desc{color:#374151; line-height:1.5; margin:6px 0 0 0}

    /* Education & References */
    .two-col{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:14px;
      margin-top:18px;
    }
    .card-mini{
      background:rgba(255,255,255,0.7);
      border-radius:10px;
      padding:12px;
    }
    .school{font-weight:700; margin:0}
    .small{font-size:0.92rem; color:var(--muted); margin:6px 0 0 0}

    /* Footer */
    .footer{
      margin-top:22px;
      color:var(--muted);
      font-size:0.9rem;
      text-align:center;
    }

    /* Small screens */
    @media (max-width:880px){
      .container{grid-template-columns:1fr; padding-bottom:40px}
      .sidebar{position:static}
      .two-col{grid-template-columns:1fr}
    }

    /* Print friendly */
    @media print{
      body{padding:0; background:white}
      .container{max-width:100%; box-shadow:none; gap:0}
      .sidebar{display:none}
      .btn{display:none}
      .main{box-shadow:none; border-radius:0; padding:0 10px}
    }

    /* subtle hover */
    a.contact-link:hover{ text-decoration:underline }
  </style>
</head>
<body>

  <div class="container" role="main">
    <!-- SIDEBAR -->
    <aside class="sidebar" aria-label="Contact and quick actions">
      <div>
        <h1 class="name">Weldon Kipkoech</h1>
        <div class="role">Data Scientist</div>
        <div class="contact" aria-hidden="false">
          <div><strong>Email:</strong> <a id="emailLink" class="contact-link" href="mailto:Sitieneiweldon04@gmail.com">Sitieneiweldon04@gmail.com</a></div>
          <div><strong>Phone:</strong> <a id="phoneLink" class="contact-link" href="tel:+254702885815">+254 702 885 815</a></div>
        </div>
        <div class="meta-btns">
          <button class="btn" id="copyBtn" title="Copy email & phone">Copy Contact</button>
          <button class="btn secondary" id="printBtn" title="Print or save as PDF">Print / PDF</button>
        </div>
        <div class="section-title">Quick Profile</div>
        <p style="color:var(--muted);font-size:0.95rem;line-height:1.5;margin:0">
          Curious & solutions-driven data scientist skilled in machine learning, analytics, and visualization. Bridges technical & non-technical audiences.
        </p>
        <div class="section-title">Skills</div>
        <ul class="list" aria-label="Skills list">
          <li>Python · Pandas · NumPy</li>
          <li>SQL · Matplotlib · Plotly</li>
          <li>Machine Learning · Model Evaluation</li>
          <li>Data Cleaning · Dashboarding</li>
        </ul>
        <div class="section-title">Download</div>
        <ul class="list">
          <li><a class="contact-link" href="#" id="downloadVcard">Download vCard</a></li>
        </ul>
      </div>
    </aside>
    <!-- MAIN CONTENT -->
    <section class="main" aria-label="Resume content">
      <div class="heading-row">
        <div>
          <h2 class="title">Professional Summary</h2>
          <p class="subhead">Data Scientist · Machine Learning · Analytics</p>
        </div>
      </div>
      <p class="summary">
        Curious and solutions-driven data scientist with proven expertise in machine learning, analytics, and predictive modeling.
        Adept at transforming complex datasets into actionable insights using Python, Pandas, SQL, and advanced visualization tools.
        Passionate about building intelligent, scalable, and impactful data solutions. Strong communicator skilled at bridging technical
        and non-technical audiences, with a keen interest in AI innovation.
      </p>
      <div class="section-title" style="margin-top:22px">Key Achievements</div>
      <div class="achievements" role="list">
        <div class="ach-card" role="listitem"><p>Developed predictive models in Python, boosting decision-making accuracy by over 80%.</p></div>
        <div class="ach-card" role="listitem"><p>Cleaned and analyzed large datasets (Pandas, NumPy, SQL) to drive data-based strategies.</p></div>
        <div class="ach-card" role="listitem"><p>Built interactive dashboards and visualizations (Matplotlib, Plotly) to clarify complex findings.</p></div>
        <div class="ach-card" role="listitem"><p>Automated data preprocessing, reducing manual workload and saving analysis time.</p></div>
        <div class="ach-card" role="listitem"><p>Collaborated on AI & software projects, integrating data science with engineering.</p></div>
        <div class="ach-card" role="listitem"><p>Delivered insights that shaped academic and business project outcomes.</p></div>
      </div>
      <div class="section-title">Professional Experience</div>
      <div class="timeline" aria-label="Professional experience timeline">
        <div class="role-item" aria-hidden="false">
          <div class="role-title">Data Analyst Intern</div>
          <div class="role-meta">Techsavanna Technology Ltd · Jan 2025 – Present</div>
          <div class="role-desc">
            Assist in developing web solutions using PHP, JavaScript, Laravel. Test APIs with Postman and integrate front-end with backend services.
            Collaborate with cross-functional teams to enhance UI/UX.
          </div>
        </div>
        <div class="role-item">
          <div class="role-title">IT Support Technician</div>
          <div class="role-meta">Kamureito High School · Jan 2023 – Dec 2024</div>
          <div class="role-desc">
            Provided technical support for hardware, software, and networking. Maintained computer labs & implemented educational software.
            Trained staff and students in basic IT skills and digital safety.
          </div>
        </div>
        <div class="role-item">
          <div class="role-title">Web & Graphics Designer (Freelance)</div>
          <div class="role-meta">Jan 2022 – May 2022</div>
          <div class="role-desc">
            Designed responsive websites (PHP, HTML, JavaScript). Created graphics & animations with Android Studio and 3D tools.
            Delivered projects aligning with clients’ brand identities.
          </div>
        </div>
        <div class="role-item">
          <div class="role-title">ICT Intern</div>
          <div class="role-meta">County Government of Kericho · Jan 2021 – May 2021</div>
          <div class="role-desc">
            Managed network systems and executed software upgrades. Conducted hardware diagnostics and repairs.
            Generated invoices and compiled business/revenue reports.
          </div>
        </div>
      </div>
      <div class="two-col" style="margin-top:22px">
        <div class="card-mini" aria-label="Education">
          <div class="section-title" style="margin-top:0">Education</div>
          <div style="margin-top:8px">
            <div class="school">Techsavanna Institute — Data Science</div>
            <div class="small">Short courses & practical training</div>
          </div>
          <div style="margin-top:10px">
            <div class="school">CyberShujaa — Data & AI</div>
            <div class="small">Workshops & certifications</div>
          </div>
          <div style="margin-top:10px">
            <div class="school">Taita Taveta University — BSc. Information Technology</div>
            <div class="small">2018 – 2022</div>
          </div>
          <div style="margin-top:10px">
            <div class="school">Mara Senior Academy — KCSE</div>
            <div class="small">2014 – 2017</div>
          </div>
        </div>
        <div class="card-mini" aria-label="References">
          <div class="section-title" style="margin-top:0">References</div>
          <div style="margin-top:8px">
            <div class="school">Shadrack Cheruiyot — Safaricom PLC</div>
            <div class="small">shadrackcheruiyot124@gmail.com</div>
          </div>
          <div style="margin-top:10px">
            <div class="school">Mr. Mark Kitur — Safaricom PLC</div>
            <div class="small">marikokitur@gmail.com</div>
          </div>
          <div style="margin-top:10px">
            <div class="school">Dr. Solomon Mwanjel — HoD, Taita Taveta University</div>
            <div class="small">smwanjele@gmail.com</div>
          </div>
        </div>
      </div>
      <div class="footer">
        © <strong>Weldon Kipkoech</strong> · Data Scientist — <span style="color:var(--muted)">Last updated: Sept 2025</span>
      </div>
    </section>
  </div>

  <script>
    // Copy contact info
    const copyBtn = document.getElementById('copyBtn');
    const email = 'Sitieneiweldon04@gmail.com';
    const phone = '+254 702 885 815';
    copyBtn.addEventListener('click', () => {
      const text = `Email: ${email}\nPhone: ${phone}`;
      navigator.clipboard?.writeText(text).then(() => {
        copyBtn.textContent = 'Copied!';
        setTimeout(()=> copyBtn.textContent = 'Copy Contact', 1800);
      }, () => {
        alert('Copy failed — please copy manually.');
      });
    });

    // Print
    document.getElementById('printBtn').addEventListener('click', () => window.print());

    // vCard download generator
    document.getElementById('downloadVcard').addEventListener('click', (e) => {
      e.preventDefault();
      const vcard = [
        'BEGIN:VCARD',
        'VERSION:3.0',
        'FN:Weldon Kipkoech',
        'TITLE:Data Scientist',
        'EMAIL;TYPE=WORK:' + email,
        'TEL;TYPE=CELL:' + phone.replace(/\s+/g,''),
        'END:VCARD'
      ].join('\\r\\n');

      const blob = new Blob([vcard], { type: 'text/vcard' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'Weldon_Kipkoech.vcf';
      document.body.appendChild(a);
      a.click();
      a.remove();
      URL.revokeObjectURL(url);
    });
  </script>
</body>
</html>
