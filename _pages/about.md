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
  --about-soft: #f6f8fb;
  --about-border: #e3e9f2;
  --about-card: #ffffff;
}

.about-wrap {
  color: var(--about-ink);
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

.hero-actions,
.link-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
  margin-top: 1.2rem;
}

.hero-actions a,
.link-buttons a {
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

.hero-actions a.secondary,
.link-buttons a.secondary {
  color: var(--about-blue-dark) !important;
  background: #ffffff;
  border: 1px solid var(--about-border);
  box-shadow: none;
}

.hero-actions a:hover,
.link-buttons a:hover {
  transform: translateY(-2px);
  background: var(--about-blue-dark);
  text-decoration: none;
}

.hero-actions a.secondary:hover,
.link-buttons a.secondary:hover {
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

.research-grid,
.toolbox-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1rem;
  margin: 1.4rem 0 2rem 0;
}

.research-card,
.tool-card {
  position: relative;
  padding: 1.25rem;
  border-radius: 18px;
  background: #ffffff;
  border: 1px solid var(--about-border);
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.04);
  transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
}

.research-card:hover,
.tool-card:hover {
  transform: translateY(-4px);
  border-color: rgba(47, 93, 140, 0.28);
  box-shadow: 0 16px 36px rgba(36, 73, 111, 0.1);
}

.research-card h3,
.tool-card h3 {
  margin-top: 0;
  margin-bottom: 0.65rem;
  color: var(--about-blue);
  font-size: 1.05rem;
}

.research-card p,
.tool-card p {
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

.compass {
  margin: 1.4rem 0 2.2rem 0;
  padding: 1.25rem;
  border: 1px solid var(--about-border);
  border-radius: 22px;
  background: linear-gradient(180deg, #ffffff, #f8fafc);
  box-shadow: 0 12px 32px rgba(36, 73, 111, 0.06);
}

.compass input {
  position: absolute;
  opacity: 0;
  pointer-events: none;
}

.compass-tabs {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 0.7rem;
  margin-bottom: 1rem;
}

.compass-tabs label {
  cursor: pointer;
  padding: 0.82rem 0.9rem;
  border-radius: 14px;
  border: 1px solid var(--about-border);
  background: #ffffff;
  color: var(--about-muted);
  font-size: 0.9rem;
  font-weight: 700;
  text-align: center;
  transition: all 0.18s ease;
}

#compass-access:checked ~ .compass-tabs label[for="compass-access"],
#compass-causal:checked ~ .compass-tabs label[for="compass-causal"],
#compass-exposure:checked ~ .compass-tabs label[for="compass-exposure"],
#compass-visual:checked ~ .compass-tabs label[for="compass-visual"] {
  color: #ffffff;
  background: var(--about-blue);
  border-color: var(--about-blue);
  box-shadow: 0 8px 18px rgba(47, 93, 140, 0.18);
}

.compass-panel {
  display: none;
  padding: 1.15rem;
  border-radius: 18px;
  background: #ffffff;
  border: 1px solid var(--about-border);
}

#compass-access:checked ~ .compass-content #panel-access,
#compass-causal:checked ~ .compass-content #panel-causal,
#compass-exposure:checked ~ .compass-content #panel-exposure,
#compass-visual:checked ~ .compass-content #panel-visual {
  display: block;
}

.compass-panel h3 {
  margin: 0 0 0.5rem 0;
  color: var(--about-blue-dark);
}

.compass-panel p {
  margin: 0.45rem 0;
  line-height: 1.65;
  color: #4a5568;
}

.compass-panel strong {
  color: var(--about-ink);
}

.pipeline {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 0.85rem;
  margin: 1.4rem 0 2.2rem 0;
}

.pipeline-step {
  position: relative;
  padding: 1rem;
  min-height: 120px;
  border-radius: 18px;
  background: #ffffff;
  border: 1px solid var(--about-border);
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.04);
}

.pipeline-step span {
  display: inline-flex;
  width: 32px;
  height: 32px;
  align-items: center;
  justify-content: center;
  margin-bottom: 0.7rem;
  border-radius: 50%;
  background: rgba(47, 93, 140, 0.1);
  color: var(--about-blue);
  font-weight: 800;
}

.pipeline-step h3 {
  margin: 0 0 0.45rem 0;
  color: var(--about-ink);
  font-size: 0.98rem;
}

.pipeline-step p {
  margin: 0;
  color: var(--about-muted);
  font-size: 0.86rem;
  line-height: 1.55;
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

  .compass,
  .compass-panel {
    padding: 1rem;
  }
}
</style>

<div class="about-wrap">

<div class="about-hero">
  <div class="about-kicker">GIScience · Urban Analytics · Environmental Health</div>
  <h1>Hello, I am Mengjie Gong.</h1>

  <p>
    I am a master’s student in <span class="about-highlight">Geographic Information Systems (GIS)</span>
    at <span class="about-highlight">Sun Yat-sen University</span>. My research lies at the intersection of
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
    <strong>Master’s Student in GIS</strong>
  </div>
  <div class="identity-item">
    <span>Research Theme</span>
    <strong>Spatial Data Science for Equitable Cities</strong>
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

## Research Compass

<p class="section-intro">
  My work can be understood through four connected directions. Each direction links a research question,
  a methodological strategy, and a practical urban application.
</p>

<div class="compass">
  <input type="radio" name="research-compass" id="compass-access" checked>
  <input type="radio" name="research-compass" id="compass-causal">
  <input type="radio" name="research-compass" id="compass-exposure">
  <input type="radio" name="research-compass" id="compass-visual">

  <div class="compass-tabs">
    <label for="compass-access">Accessibility</label>
    <label for="compass-causal">Spatial Causality</label>
    <label for="compass-exposure">Exposure</label>
    <label for="compass-visual">Visualization</label>
  </div>

  <div class="compass-content">
    <div class="compass-panel" id="panel-access">
      <h3>Spatial Accessibility & Service Equity</h3>
      <p><strong>Question:</strong> How well do urban services match population demand across space and time?</p>
      <p><strong>Methods:</strong> 2SFCA-family models, gravity-based accessibility, spatial optimization, scenario simulation.</p>
      <p><strong>Applications:</strong> Healthcare facilities, elderly care services, grocery stores, green spaces, and emergency accessibility.</p>
    </div>

    <div class="compass-panel" id="panel-causal">
      <h3>Causal Inference for Spatial and Spatiotemporal Data</h3>
      <p><strong>Question:</strong> How can causal inference be adapted when observations are spatially dependent?</p>
      <p><strong>Methods:</strong> Spatially aware causal modeling, heterogeneity analysis, machine learning, policy evaluation.</p>
      <p><strong>Applications:</strong> Urban planning interventions, environmental assessment, public health, and resource allocation.</p>
    </div>

    <div class="compass-panel" id="panel-exposure">
      <h3>Dynamic Environmental Health Exposure</h3>
      <p><strong>Question:</strong> How do mobility patterns shape people’s exposure to environmental and social conditions?</p>
      <p><strong>Methods:</strong> Trajectory-based exposure assessment, remote sensing, street-view data, social media and review data mining.</p>
      <p><strong>Applications:</strong> Thermal exposure, noise exposure, sentiment exposure, and street-level built environment exposure.</p>
    </div>

    <div class="compass-panel" id="panel-visual">
      <h3>Geospatial Visualization & Urban Storytelling</h3>
      <p><strong>Question:</strong> How can complex spatial patterns be communicated clearly to researchers, planners, and the public?</p>
      <p><strong>Methods:</strong> GIS visualization, story maps, dashboards, spatial data storytelling, and visual analytics.</p>
      <p><strong>Applications:</strong> Communicating accessibility gaps, exposure inequalities, urban perception, and planning scenarios.</p>
    </div>
  </div>
</div>

## Method Toolbox

<p class="section-intro">
  I use a mixed methodological toolkit that connects spatial theory, computational modeling, and urban applications.
</p>

<div class="toolbox-grid">
  <div class="tool-card">
    <h3>GIS & Spatial Analysis</h3>
    <p>Measuring spatial patterns, spatial mismatch, accessibility, and neighborhood-level inequalities.</p>
  </div>
  <div class="tool-card">
    <h3>Remote Sensing</h3>
    <p>Extracting environmental and urban surface information from satellite and earth observation data.</p>
  </div>
  <div class="tool-card">
    <h3>Urban Big Data Mining</h3>
    <p>Using mobility traces, social media, online reviews, and street-level data to understand urban dynamics.</p>
  </div>
  <div class="tool-card">
    <h3>Causal Inference</h3>
    <p>Estimating spatially heterogeneous effects and supporting more evidence-based policy evaluation.</p>
  </div>
  <div class="tool-card">
    <h3>Spatial Optimization</h3>
    <p>Designing facility allocation and service improvement scenarios under equity and efficiency objectives.</p>
  </div>
  <div class="tool-card">
    <h3>Geovisual Analytics</h3>
    <p>Transforming complex spatial results into maps, dashboards, figures, and communicable research stories.</p>
  </div>
</div>

## Research Pipeline

<p class="section-intro">
  A common logic across my projects is to move from urban data to spatial diagnosis, then from diagnosis to planning insight.
</p>

<div class="pipeline">
  <div class="pipeline-step">
    <span>1</span>
    <h3>Urban Data</h3>
    <p>Collect population, mobility, facility, remote sensing, social media, and environmental data.</p>
  </div>
  <div class="pipeline-step">
    <span>2</span>
    <h3>Spatial Modeling</h3>
    <p>Model accessibility, exposure, spatial dependence, and service-demand relationships.</p>
  </div>
  <div class="pipeline-step">
    <span>3</span>
    <h3>Evaluation</h3>
    <p>Assess equity, efficiency, heterogeneity, causal effects, and uncertainty across places.</p>
  </div>
  <div class="pipeline-step">
    <span>4</span>
    <h3>Planning Insight</h3>
    <p>Translate model results into scenario comparison, policy implications, and visual communication.</p>
  </div>
</div>

## Current Research

My current work explores how spatial data, remote sensing, urban big data, and computational modeling can be used to understand urban environments and support evidence-based planning.

<div class="question-list">
  <details class="question-card" open>
    <summary>How can we measure spatial accessibility more accurately across space and time?</summary>
    <div>
      <p><strong>Why it matters:</strong> Static accessibility measures may overlook temporal population dynamics, service availability, and changing travel conditions.</p>
      <p><strong>My approach:</strong> Dynamic population data, 2SFCA-family models, gravity-based modeling, and scenario simulation.</p>
    </div>
  </details>

  <details class="question-card">
    <summary>How do urban resources match population demand?</summary>
    <div>
      <p><strong>Why it matters:</strong> Healthcare facilities, elderly care services, grocery stores, and green spaces are often unevenly distributed.</p>
      <p><strong>My approach:</strong> Spatial mismatch analysis, accessibility indicators, demand-supply modeling, and optimization-based comparison.</p>
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

## More About My Work

You can find more details about my research projects, technical explorations, publications, and selected works through the following pages:

<div class="link-buttons">
  <a href="/research-projects/">Research & Projects</a>
  <a class="secondary" href="/publications/">Publications</a>
  <a class="secondary" href="/cv/">CV</a>
</div>

</div>
