---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
:root {
  --about-blue: #2f5d8c;
  --about-blue-dark: #24496f;
  --about-ink: #243447;
  --about-muted: #5b6778;
  --about-border: #e3e9f2;
  --about-card: #ffffff;
}

.about-hero {
  position: relative;
  overflow: hidden;
  padding: 2.2rem;
  margin-bottom: 1.8rem;
  border-radius: 24px;
  background:
    radial-gradient(circle at 88% 16%, rgba(47, 93, 140, 0.16), transparent 28%),
    linear-gradient(135deg, #f8fbff 0%, #eef4fa 52%, #f7f9fc 100%);
  border: 1px solid var(--about-border);
  box-shadow: 0 16px 40px rgba(36, 73, 111, 0.08);
}

.about-hero::after {
  content: "";
  position: absolute;
  right: -80px;
  bottom: -90px;
  width: 240px;
  height: 240px;
  border-radius: 50%;
  border: 34px solid rgba(47, 93, 140, 0.07);
}

.about-kicker {
  display: inline-flex;
  align-items: center;
  gap: 0.45rem;
  padding: 0.34rem 0.72rem;
  margin-bottom: 1rem;
  border-radius: 999px;
  background: rgba(47, 93, 140, 0.09);
  color: var(--about-blue-dark);
  font-size: 0.78rem;
  font-weight: 700;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

.about-hero h1 {
  margin: 0 0 0.8rem 0;
  font-size: clamp(2rem, 4vw, 3rem);
  line-height: 1.08;
  letter-spacing: -0.04em;
}

.about-hero p {
  position: relative;
  max-width: 850px;
  font-size: 1rem;
  line-height: 1.78;
  color: #3f4a56;
  z-index: 1;
}

.about-highlight {
  font-weight: 700;
  color: var(--about-blue);
}

.hero-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
  margin-top: 1.2rem;
}

.hero-actions a {
  display: inline-block;
  padding: 0.68rem 0.95rem;
  border-radius: 12px;
  background: var(--about-blue);
  color: #ffffff !important;
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 650;
  box-shadow: 0 8px 20px rgba(47, 93, 140, 0.16);
  transition: transform 0.18s ease, background 0.18s ease, box-shadow 0.18s ease;
}

.hero-actions a.secondary {
  color: var(--about-blue-dark) !important;
  background: #ffffff;
  border: 1px solid var(--about-border);
  box-shadow: none;
}

.hero-actions a:hover {
  transform: translateY(-2px);
  background: var(--about-blue-dark);
  text-decoration: none;
}

.hero-actions a.secondary:hover {
  background: #f1f5f9;
}

.identity-dashboard {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 0.9rem;
  margin: 1.5rem 0 2.2rem 0;
}

.identity-item {
  padding: 1rem;
  border: 1px solid var(--about-border);
  border-radius: 18px;
  background: var(--about-card);
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.04);
}

.identity-item span {
  display: block;
  margin-bottom: 0.35rem;
  color: var(--about-muted);
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

.identity-item strong {
  color: var(--about-ink);
  font-size: 0.98rem;
}

.section-intro {
  max-width: 840px;
  color: var(--about-muted);
  line-height: 1.72;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1rem;
  margin: 1.4rem 0 2rem 0;
}

.research-card {
  position: relative;
  padding: 1.25rem;
  border-radius: 18px;
  background: #ffffff;
  border: 1px solid var(--about-border);
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.04);
  transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
}

.research-card:hover {
  transform: translateY(-4px);
  border-color: rgba(47, 93, 140, 0.28);
  box-shadow: 0 16px 36px rgba(36, 73, 111, 0.1);
}

.research-card h3 {
  margin-top: 0;
  margin-bottom: 0.65rem;
  color: var(--about-blue);
  font-size: 1.05rem;
}

.research-card p {
  margin-bottom: 0;
  font-size: 0.92rem;
  line-height: 1.68;
  color: #4a5568;
}

.keyword-row {
  display: flex;
  flex-wrap: wrap;
  gap: 0.48rem;
  margin: 1rem 0 2.1rem 0;
}

.keyword-row span {
  padding: 0.34rem 0.7rem;
  border-radius: 999px;
  background: #f1f5f9;
  color: #3f4a56;
  font-size: 0.8rem;
  border: 1px solid #e6edf5;
}

.question-list {
  display: grid;
  gap: 0.85rem;
  margin: 1.3rem 0 2.1rem 0;
}

.question-card {
  border: 1px solid var(--about-border);
  border-radius: 18px;
  background: #ffffff;
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.04);
  overflow: hidden;
}

.question-card summary {
  cursor: pointer;
  padding: 1rem 1.1rem;
  color: var(--about-blue-dark);
  font-weight: 750;
  line-height: 1.45;
  list-style: none;
}

.question-card summary::-webkit-details-marker {
  display: none;
}

.question-card summary::after {
  content: "+";
  float: right;
  color: var(--about-blue);
  font-size: 1.1rem;
}

.question-card[open] summary::after {
  content: "-";
}

.question-card div {
  padding: 0 1.1rem 1.05rem 1.1rem;
  color: #4a5568;
  line-height: 1.68;
}

.question-card p {
  margin: 0.5rem 0;
}

.service-list li {
  margin-bottom: 0.35rem;
}

.note-box {
  padding: 1.2rem 1.35rem;
  margin: 1.4rem 0;
  border-left: 4px solid var(--about-blue);
  background: #f8fafc;
  border-radius: 14px;
  color: #4a5568;
  line-height: 1.7;
}

@media (max-width: 600px) {
  .about-hero {
    padding: 1.55rem;
  }
}
</style>

<div class="about-hero">
  <div class="about-kicker">Surveying & Mapping Engineering · GIScience · Urban Analytics</div>
  <h1>Hello, I am Mengjie Gong.</h1>

  <p>
    I am a master’s student in <span class="about-highlight">Surveying and Mapping Engineering</span>
    at <span class="about-highlight">Sun Yat-sen University</span>, with research focused on
    <span class="about-highlight">Geographic Information Systems (GIS)</span>. My work lies at the intersection of
    spatial data science, urban analytics, and environmental health.
  </p>

  <p>
    I am particularly interested in using <span class="about-highlight">GIS, remote sensing, urban big data,
    and computational modeling</span> to understand how people access urban resources, how environmental
    exposures are distributed across space and time, and how spatial methods can support healthier and more
    equitable cities.
  </p>

  <div class="hero-actions">
    <a href="/research-projects/">Explore Projects</a>
    <a class="secondary" href="/publications/">View Publications</a>
    <a class="secondary" href="/cv/">Download CV</a>
  </div>
</div>

<div class="identity-dashboard">
  <div class="identity-item">
    <span>Current Role</span>
    <strong>Master’s Student in Surveying and Mapping Engineering</strong>
  </div>
  <div class="identity-item">
    <span>Research Focus</span>
    <strong>GIScience and Spatial Data Science</strong>
  </div>
  <div class="identity-item">
    <span>Methodological Focus</span>
    <strong>GIS · Remote Sensing · Causal Inference</strong>
  </div>
  <div class="identity-item">
    <span>Application Areas</span>
    <strong>Healthcare · Elderly Care · Exposure · Urban Resources</strong>
  </div>
</div>

## Research Interests

<div class="research-grid">

  <div class="research-card">
    <h3>Spatial Accessibility Modeling</h3>
    <p>
      Developing computational methods and tools for quantifying spatial accessibility, with applications
      in healthcare facilities, elderly care services, grocery stores, urban green spaces, and accessibility
      dynamics under extreme weather events.
    </p>
  </div>

  <div class="research-card">
    <h3>Causal Inference for Spatial Data</h3>
    <p>
      Exploring causal inference methods tailored for spatial and spatiotemporal data, with applications in
      urban studies, environmental assessment, public health, and policy evaluation.
    </p>
  </div>

  <div class="research-card">
    <h3>Environmental Health Exposure Analysis</h3>
    <p>
      Developing dynamic, trajectory-based exposure assessment methods, with applications in sentiment exposure,
      thermal exposure, street-level built environment exposure, and noise exposure.
    </p>
  </div>

</div>

<div class="keyword-row">
  <span>GIScience</span>
  <span>Spatial Accessibility</span>
  <span>Causal Inference</span>
  <span>Environmental Health</span>
  <span>Remote Sensing</span>
  <span>Urban Big Data</span>
  <span>Human Mobility</span>
  <span>Spatial Optimization</span>
</div>

## Research Questions

<p class="section-intro">
  My current work focuses on three connected questions in GIScience, urban analytics, and environmental health.
</p>

<div class="question-list">
  <details class="question-card" open>
    <summary>How can we measure spatial accessibility more accurately across space and time?</summary>
    <div>
      <p><strong>Why it matters:</strong> Static accessibility measures may overlook temporal population dynamics, service availability, and changing travel conditions.</p>
      <p><strong>My approach:</strong> Dynamic population data, 2SFCA-family models, gravity-based modeling, and scenario simulation.</p>
    </div>
  </details>

  <details class="question-card">
    <summary>How can causal inference be adapted to spatial and spatiotemporal data?</summary>
    <div>
      <p><strong>Why it matters:</strong> Spatial dependence and regional heterogeneity challenge conventional causal analysis.</p>
      <p><strong>My approach:</strong> Spatially heterogeneous causal effects, machine learning, double machine learning, and policy-oriented evaluation.</p>
    </div>
  </details>

  <details class="question-card">
    <summary>How do dynamic human mobility patterns shape environmental exposure and health-related risks?</summary>
    <div>
      <p><strong>Why it matters:</strong> People are exposed to environments not only where they live, but also where they travel and spend time.</p>
      <p><strong>My approach:</strong> Trajectory-based exposure assessment, mobility data, environmental sensing, and street-level visual analytics.</p>
    </div>
  </details>
</div>

## Academic Service

I have served as a reviewer for several international journals, including:

<ul class="service-list">
  <li><em>Journal of Transport Geography</em> (Q1)</li>
  <li><em>Humanities & Social Sciences Communications</em> (Q1)</li>
  <li><em>EPJ Data Science</em> (Q1)</li>
  <li><em>Discover Cities</em></li>
</ul>

## Beyond Research

<div class="note-box">
  Beyond formal research projects, I am also interested in geospatial visualization, story maps, urban perception analysis, social media data mining, and public review data analysis. I enjoy using GIS and data visualization to transform complex urban phenomena into more intuitive and communicable forms.
</div>
