---
layout: default
title: CONTACT ME
icon: fas fa-phone
---

<style>
  /* Page Styling */
  h1, h2 {
    font-family: 'Bungee', cursive, sans-serif;
    color: white;
    text-align: center;
  }

  .colorful-container {
    text-align: center;
    background: linear-gradient(135deg, #332d64, #ffd36d);
    padding: 30px;
    border-radius: 20px;
    box-shadow: 0 0 20px #00000033;
    max-width: 700px;
    margin: 30px auto;
  }

  .section-title {
    font-size: 1.5rem;
    font-weight: bold;
    margin-bottom: 20px;
    color: white;
  }

  .contact-links {
    display: flex;
    justify-content: center;
    gap: 25px;
    flex-wrap: wrap;
  }

  /* 🔹 Icon Color Control */
  .contact-links img {
    width: 50px;
    height: 50px;
    filter: invert(100%) sepia(100%) saturate(0%) hue-rotate(180deg);
    transition: transform 0.3s ease, filter 0.3s ease;
  }

  /* 🔹 Hover Effect: Slight color + zoom */
  .contact-links img:hover {
    transform: scale(1.2);
    filter: invert(84%) sepia(80%) saturate(1000%) hue-rotate(40deg);
  }

  /* Responsive */
  @media (max-width: 600px) {
    .colorful-container {
      padding: 20px;
    }
  }

  p {
    color: white;
    text-align: center;
    margin-top: 20px;
  }
</style>

<h1>Let's Connect! 💫</h1>
<h2>I'm always excited to hear about new opportunities, collaborate on innovative projects, or simply chat about technology.</h2>

<div class="colorful-container">
  <div class="section-title">🔗 Connect With Me</div>

  <div class="contact-links">
    <a href="mailto:weldonkipkoech@email.com" target="_blank">
      <img src="https://img.icons8.com/ios-filled/50/000000/new-post.png" alt="Email">
    </a>

  <a href="https://github.com/weldonkipkoech" target="_blank">
      <img src="https://img.icons8.com/ios-glyphs/50/000000/github.png" alt="GitHub">
    </a>

  <a href="https://www.kaggle.com/weldonsitienei" target="_blank">
      <img src="https://www.kaggle.com/static/images/site-logo.png" alt="Kaggle">
    </a>
  </div>
</div>

<p>Thank you! Looking forward to your response 💬</p>
