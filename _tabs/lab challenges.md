---
layout: default
title: LAB CHALLENGES
icon: fas fa-flask
---
<div class="container">
        <header>
            <div class="header-content">
                <i class="fas fa-flask icon"></i>
                <div>
                    <h1>LAB CHALLENGES</h1>
                    <p class="subtitle">Showcasing my cybersecurity and technical challenge solutions</p>
                </div>
            </div>
        </header>

<div class="challenges-grid">
            <!-- Challenge 1: SQL Injection -->
            <div class="challenge-card">
                <div class="challenge-header">
                    <div class="challenge-icon">
                        <i class="fas fa-database"></i>
                    </div>
                    <h2 class="challenge-title">SQL Injection Exploitation
                        <span class="difficulty-badge difficulty-medium">Medium</span>
                    </h2>
                </div>

<div class="section-title">
                    <i class="fas fa-question-circle"></i>
                    <span>Problem Statement</span>
                </div>
                <div class="problem-statement">
                    "Identify and exploit SQL injection vulnerabilities in a vulnerable web application to extract sensitive user data from the database, including admin credentials and personal information."
                </div>

<div class="section-title">
                    <i class="fas fa-tools"></i>
                    <span>Tools Used</span>
                </div>
                <div class="tech-stack">
                    <div class="tech-item">
                        <i class="fas fa-terminal"></i>
                        <span>Burp Suite</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-code"></i>
                        <span>SQLMap</span>
                    </div>
                    <div class="tech-item">
                        <i class="fab fa-python"></i>
                        <span>Python</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-globe"></i>
                        <span>Browser DevTools</span>
                    </div>
                </div>

 <div class="section-title">
                    <i class="fas fa-route"></i>
                    <span>Approach & Methodology</span>
                </div>
                <div class="approach-steps">
                    <div class="step">
                        <div class="step-number">1</div>
                        <div>Identified input fields vulnerable to SQL injection using manual testing with single quotes and basic payloads</div>
                    </div>
                    <div class="step">
                        <div class="step-number">2</div>
                        <div>Used Burp Suite to intercept and modify requests for automated testing</div>
                    </div>
                    <div class="step">
                        <div class="step-number">3</div>
                        <div>Employed SQLMap for automated database enumeration and data extraction</div>
                    </div>
                    <div class="step">
                        <div class="step-number">4</div>
                        <div>Manually crafted UNION-based queries to extract specific table structures</div>
                    </div>
                </div>

<div class="section-title">
                    <i class="fas fa-camera"></i>
                    <span>Screenshots</span>
                </div>
                <div class="screenshot-gallery">
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/3b82f6?text=SQLMap+Results" alt="SQLMap Results">
                    </div>
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/10b981?text=Database+Schema" alt="Database Schema">
                    </div>
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/f59e0b?text=Extracted+Data" alt="Extracted Data">
                    </div>
                </div>
<div class="section-title">
                    <i class="fas fa-graduation-cap"></i>
                    <span>Key Lessons Learned</span>
                </div>
                <div class="lessons-learned">
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Understanding how UNION-based SQL injection works and when to use it</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Importance of input validation and parameterized queries in web applications</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>How to use automated tools effectively while understanding their limitations</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Database schema enumeration techniques and information extraction</div>
                    </div>
                </div>
            </div>

            <!-- Challenge 2: Buffer Overflow -->
<div class="challenge-card">
                <div class="challenge-header">
                    <div class="challenge-icon">
                        <i class="fas fa-memory"></i>
                    </div>
                    <h2 class="challenge-title">Buffer Overflow Exploitation
                        <span class="difficulty-badge difficulty-hard">Hard</span>
                    </h2>
                </div>

<div class="section-title">
                    <i class="fas fa-question-circle"></i>
                    <span>Problem Statement</span>
                </div>
                <div class="problem-statement">
                    "Exploit a stack-based buffer overflow vulnerability in a custom C application to achieve remote code execution and gain shell access on the target system."
                </div>

<div class="section-title">
                    <i class="fas fa-tools"></i>
                    <span>Tools Used</span>
                </div>
                <div class="tech-stack">
                    <div class="tech-item">
                        <i class="fas fa-bug"></i>
                        <span>GDB</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-code"></i>
                        <span>Python</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-terminal"></i>
                        <span>Pwntools</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-microchip"></i>
                        <span>Metasploit</span>
                    </div>
                </div>

<div class="section-title">
                    <i class="fas fa-route"></i>
                    <span>Approach & Methodology</span>
                </div>
                <div class="approach-steps">
                    <div class="step">
                        <div class="step-number">1</div>
                        <div>Fuzzed the application to identify the exact buffer overflow point</div>
                    </div>
                    <div class="step">
                        <div class="step-number">2</div>
                        <div>Used GDB with Peda to analyze the crash and locate EIP overwrite</div>
                    </div>
                    <div class="step">
                        <div class="step-number">3</div>
                        <div>Identified bad characters and found JMP ESP instruction for EIP control</div>
                    </div>
                    <div class="step">
                        <div class="step-number">4</div>
                        <div>Generated shellcode and created the final exploit payload</div>
                    </div>
                </div>

<div class="section-title">
                    <i class="fas fa-camera"></i>
                    <span>Screenshots</span>
                </div>
                <div class="screenshot-gallery">
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/ef4444?text=GDB+Analysis" alt="GDB Analysis">
                    </div>
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/3b82f6?text=Shellcode+Execution" alt="Shellcode Execution">
                    </div>
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/10b981?text=Reverse+Shell" alt="Reverse Shell">
                    </div>
                </div>

<div class="section-title">
                    <i class="fas fa-graduation-cap"></i>
                    <span>Key Lessons Learned</span>
                </div>
                <div class="lessons-learned">
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Deep understanding of stack memory layout and function prologue/epilogue</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Importance of identifying and avoiding bad characters in shellcode</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Techniques for finding and using ROP gadgets when DEP is enabled</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Shellcode encoding and anti-virus evasion techniques</div>
                    </div>
                </div>
            </div>

            <!-- Challenge 3: Network Forensics -->
<div class="challenge-card">
                <div class="challenge-header">
                    <div class="challenge-icon">
                        <i class="fas fa-network-wired"></i>
                    </div>
                    <h2 class="challenge-title">Network Traffic Analysis
                        <span class="difficulty-badge difficulty-easy">Easy</span>
                    </h2>
                </div>

<div class="section-title">
                    <i class="fas fa-question-circle"></i>
                    <span>Problem Statement</span>
                </div>
                <div class="problem-statement">
                    "Analyze a suspicious network capture file to identify malicious activity, data exfiltration attempts, and reconstruct the attack timeline from the evidence."
                </div>

<div class="section-title">
                    <i class="fas fa-tools"></i>
                    <span>Tools Used</span>
                </div>
                <div class="tech-stack">
                    <div class="tech-item">
                        <i class="fas fa-search"></i>
                        <span>Wireshark</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-filter"></i>
                        <span>tshark</span>
                    </div>
                    <div class="tech-item">
                        <i class="fab fa-python"></i>
                        <span>Python</span>
                    </div>
                    <div class="tech-item">
                        <i class="fas fa-chart-bar"></i>
                        <span>NetworkMiner</span>
                    </div>
                </div>
<div class="section-title">
                    <i class="fas fa-route"></i>
                    <span>Approach & Methodology</span>
                </div>
                <div class="approach-steps">
                    <div class="step">
                        <div class="step-number">1</div>
                        <div>Initial triage using Wireshark statistics and conversation analysis</div>
                    </div>
                    <div class="step">
                        <div class="step-number">2</div>
                        <div>Filtered for DNS queries to identify potential C2 communication</div>
                    </div>
                    <div class="step">
                        <div class="step-number">3</div>
                        <div>Extracted and analyzed HTTP traffic for data exfiltration</div>
                    </div>
                    <div class="step">
                        <div class="step-number">4</div>
                        <div>Reconstructed file transfers and identified malicious payloads</div>
                    </div>
                </div>

 <div class="section-title">
                    <i class="fas fa-camera"></i>
                    <span>Screenshots</span>
                </div>
                <div class="screenshot-gallery">
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/3b82f6?text=Wireshark+Analysis" alt="Wireshark Analysis">
                    </div>
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/f59e0b?text=DNS+Queries" alt="DNS Queries">
                    </div>
                    <div class="screenshot">
                        <img src="https://via.placeholder.com/300x150/1e293b/10b981?text=File+Reconstruction" alt="File Reconstruction">
                    </div>
                </div>

<div class="section-title">
                    <i class="fas fa-graduation-cap"></i>
                    <span>Key Lessons Learned</span>
                </div>
                <div class="lessons-learned">
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Importance of understanding common network protocols and their anomalies</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>DNS tunneling techniques and detection methods</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Network forensics timeline reconstruction and incident analysis</div>
                    </div>
                    <div class="lesson-item">
                        <i class="fas fa-check-circle lesson-icon"></i>
                        <div>Data exfiltration patterns and detection signatures</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
