---
title: "CBA-Access: Cost-Balanced Accessibility Modeling Toolkit"
collection: portfolio
permalink: /research-projects/cba-access/
author_profile: true
---

<style>
.project-hero {
  padding: 2rem;
  margin-bottom: 2rem;
  border-radius: 18px;
  background: linear-gradient(135deg, #f7f9fc, #eef3f8);
  border: 1px solid #e4eaf1;
}

.project-hero h1 {
  margin-top: 0;
  font-size: 2rem;
  color: #2f5d8c;
}

.project-hero p {
  line-height: 1.75;
  color: #3f4a56;
}

.project-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
  margin-top: 1rem;
}

.project-badges span {
  padding: 0.3rem 0.65rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid #d8e2ec;
  color: #2f5d8c;
  font-size: 0.8rem;
  font-weight: 600;
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1rem;
  margin: 1.5rem 0;
}

.info-card {
  padding: 1.1rem;
  border-radius: 16px;
  background: #ffffff;
  border: 1px solid #e5e9f0;
  box-shadow: 0 8px 22px rgba(0,0,0,0.04);
}

.info-card h3 {
  margin-top: 0;
  font-size: 1rem;
  color: #2f5d8c;
}

.info-card p {
  font-size: 0.92rem;
  line-height: 1.65;
  color: #4a5568;
}

.figure-box {
  margin: 1.6rem 0;
}

.figure-box img {
  width: 100%;
  border-radius: 14px;
  border: 1px solid #e5e9f0;
}

.figure-box figcaption {
  margin-top: 0.5rem;
  font-size: 0.85rem;
  color: #6b7280;
  text-align: center;
}

.roadmap {
  border-left: 4px solid #2f5d8c;
  padding-left: 1rem;
  margin: 1.5rem 0;
}

.roadmap-item {
  margin-bottom: 1rem;
}

.roadmap-item strong {
  color: #2f5d8c;
}

.highlight-box {
  padding: 1.2rem 1.4rem;
  border-radius: 14px;
  background: #f8fafc;
  border: 1px solid #e5e9f0;
  margin: 1.5rem 0;
}

.link-button {
  display: inline-block;
  padding: 0.6rem 0.9rem;
  margin: 0.3rem 0.3rem 0.3rem 0;
  border-radius: 10px;
  background: #2f5d8c;
  color: #ffffff !important;
  text-decoration: none;
  font-size: 0.9rem;
}

.link-button:hover {
  background: #24496f;
}
</style>

<div class="project-hero">
  <h1>CBA-Access</h1>

  <p>
    <strong>CBA-Access</strong> is a research-oriented Python toolkit for implementing and extending the 
    <strong>Cost-Balanced Accessibility (CBA) model</strong>, a new accessibility modeling framework designed 
    to measure urban accessibility with multi-objective considerations.
  </p>

  <p>
    Rather than focusing on a single type of urban facility, CBA-Access is designed as a 
    <strong>general-purpose spatial accessibility toolkit</strong>. It can be adapted to various accessibility 
    scenarios, such as healthcare facilities, elderly care services, grocery stores, green spaces, charging 
    infrastructure, and other public or commercial urban resources.
  </p>

  <div class="project-badges">
    <span>Python Package</span>
    <span>Spatial Accessibility</span>
    <span>CBA Model</span>
    <span>GIScience</span>
    <span>Multi-objective Evaluation</span>
    <span>Open Research Tool</span>
  </div>
</div>

## From Paper to Tool

CBA-Access is developed based on the following study:

> Chen, P., Gong, M., & Li, S. (2025). The cost-balanced accessibility (CBA) model: a new framework for measuring urban accessibility with multi-objective considerations. *International Journal of Geographical Information Science*, 1–24.

The package represents an effort to transform a theoretical accessibility model into a reusable computational tool. My long-term goal is to gradually develop it into a specialized Python toolkit for spatial accessibility analysis.

<div class="highlight-box">
  <strong>Core idea:</strong> CBA-Access is not only a code implementation of one model. It is an early-stage attempt to build a more systematic, reusable, and extensible accessibility modeling toolkit for GIScience and urban studies.
</div>

## What Makes CBA Different?

Traditional accessibility models often focus on whether people can reach facilities within a given distance or travel time. The CBA model further considers the balance between accessibility benefits and multiple types of costs or constraints.

<div class="info-grid">

  <div class="info-card">
    <h3>Beyond Distance</h3>
    <p>
      Accessibility is not only about spatial proximity. It is also shaped by resource capacity, demand pressure,
      travel impedance, and planning constraints.
    </p>
  </div>

  <div class="info-card">
    <h3>Multi-objective Thinking</h3>
    <p>
      The CBA framework introduces a cost-balanced perspective, making accessibility evaluation more suitable
      for real-world planning problems with competing objectives.
    </p>
  </div>

  <div class="info-card">
    <h3>General-purpose Design</h3>
    <p>
      The toolkit is designed to support different types of urban facilities and services, rather than being
      limited to one specific application scenario.
    </p>
  </div>

</div>

## Installation

The current prototype version can be installed from TestPyPI:

```bash
pip install -i https://test.pypi.org/simple/ cba-access
