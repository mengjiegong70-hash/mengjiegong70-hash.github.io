---
layout: single
title: "Sense+ 城市环境健康地图 / Urban Environmental Health Map"
permalink: /research-projects/sense-plus/
author_profile: true
---

<style>
.sense-hero {
  padding: 2rem;
  margin-bottom: 1.5rem;
  border-radius: 22px;
  background: linear-gradient(135deg, #f7fbfc, #eef5f7);
  border: 1px solid #e3e9f2;
  box-shadow: 0 12px 32px rgba(0, 0, 0, 0.05);
}

.sense-hero h1 {
  margin-top: 0;
  margin-bottom: 0.35rem;
  font-size: 2rem;
  letter-spacing: -0.03em;
}

.sense-hero h2 {
  margin-top: 0;
  margin-bottom: 0.9rem;
  font-size: 1.18rem;
  font-weight: 600;
  color: #2f5d8c;
}

.sense-hero p {
  max-width: 880px;
  line-height: 1.75;
  color: #4a5568;
}

.sense-kicker {
  display: inline-block;
  margin-bottom: 0.8rem;
  padding: 0.35rem 0.72rem;
  border-radius: 999px;
  background: #e9f5f7;
  color: #2f5d8c;
  font-size: 0.78rem;
  font-weight: 700;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

.sense-media {
  margin: 1.5rem 0;
}

.sense-cover,
.sense-video {
  width: 100%;
  border-radius: 18px;
  border: 1px solid #e3e9f2;
  box-shadow: 0 10px 28px rgba(0, 0, 0, 0.08);
}

.sense-video {
  margin-top: 1rem;
  background: #000;
}

.sense-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 1rem;
  margin: 1.5rem 0;
}

.sense-card {
  padding: 1.15rem;
  border-radius: 16px;
  background: #ffffff;
  border: 1px solid #e5e9f0;
  box-shadow: 0 8px 22px rgba(0, 0, 0, 0.04);
}

.sense-card h3 {
  margin-top: 0;
  color: #2f5d8c;
  font-size: 1.02rem;
}

.sense-card p,
.sense-card li {
  color: #4a5568;
  line-height: 1.65;
  font-size: 0.92rem;
}

.sense-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
  margin: 1rem 0 1.5rem 0;
}

.sense-tags span {
  padding: 0.3rem 0.65rem;
  border-radius: 999px;
  background: #f1f5f9;
  color: #3f4a56;
  font-size: 0.78rem;
  border: 1px solid #e6edf5;
}

.sense-section {
  margin-top: 2rem;
}

.sense-section p,
.sense-section li {
  line-height: 1.75;
}

@media (prefers-color-scheme: dark) {
  .sense-hero {
    background: linear-gradient(135deg, #2f3742, #394554);
    border-color: #66707d;
  }

  .sense-hero p,
  .sense-card p,
  .sense-card li,
  .sense-section p,
  .sense-section li {
    color: #dce3ea;
  }

  .sense-card {
    background: #34383f;
    border-color: #66707d;
  }

  .sense-card h3,
  .sense-hero h2,
  .sense-kicker {
    color: #7ddff2;
  }

  .sense-kicker,
  .sense-tags span {
    background: rgba(125, 223, 242, 0.16);
    color: #7ddff2;
    border-color: rgba(125, 223, 242, 0.32);
  }
}
</style>

<div class="sense-hero">
  <div class="sense-kicker">Remote Sensing · Environmental Health · Urban GIS</div>
  <h1>Sense+ 城市环境健康地图</h1>
  <h2>Sense+ Urban Environmental Health Map</h2>
  <p>
    <strong>Sense+</strong> is a remote-sensing-driven urban environmental health mapping project. It integrates
    satellite remote sensing, street-level environmental indicators, air pollution monitoring, AI interpretation,
    and mobile interaction to transform complex urban environmental data into an actionable health map for daily life.
  </p>
</div>

<div class="sense-tags">
  <span>Remote Sensing</span>
  <span>GIS</span>
  <span>Urban Environmental Health</span>
  <span>UEHI</span>
  <span>Healthy Route Planning</span>
  <span>AI Interpretation</span>
</div>

<div class="sense-media">
  <img class="sense-cover" src="/images/环境地图.jpg" alt="Sense+ urban environmental health map preview">

  <video class="sense-video" controls preload="metadata" poster="/images/环境地图.jpg">
    <source src="/images/video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

## Project Overview / 项目概述

Sense+ aims to build a street-level urban environmental health map by combining multi-source remote sensing data, street-view indicators, real-time air pollution information, and AI-based environmental interpretation. The project focuses on how urban environmental factors such as street enclosure, green visibility, sky view, visual distance, and air quality may influence residents’ physical and mental well-being.

Rather than treating remote sensing as a purely technical tool, this project explores how remote sensing can become a public-facing health service: a map that helps users understand nearby environmental risks, identify healthier streets, and choose more comfortable routes for commuting, walking, recreation, and community life.

## What Problem Does It Address? / 解决什么问题？

<div class="sense-grid">
  <div class="sense-card">
    <h3>Environmental health is hard to perceive</h3>
    <p>Citizens often cannot directly assess whether a street is visually open, green, polluted, or potentially stressful.</p>
  </div>
  <div class="sense-card">
    <h3>Urban exposure is spatially uneven</h3>
    <p>Green visibility, sky openness, air quality, and spatial enclosure vary significantly across streets and neighborhoods.</p>
  </div>
  <div class="sense-card">
    <h3>Remote sensing needs public scenarios</h3>
    <p>The project translates high-resolution environmental data into daily decision support for health-oriented urban life.</p>
  </div>
</div>

## Technical Framework / 技术框架

The project constructs an <strong>Urban Environment Health Index (UEHI)</strong> by integrating street-level spatial environment indicators and grid-level air pollution indicators. The framework includes:

<ul>
  <li><strong>Street-level visual environment:</strong> green view index, street enclosure, sky view factor, and visual distance.</li>
  <li><strong>Air pollution indicators:</strong> PM2.5, PM10, CO, O3, NO2, and SO2.</li>
  <li><strong>Data fusion:</strong> remote sensing imagery, street-view data, ground monitoring, AI interpretation, and expert-weighted health evaluation.</li>
  <li><strong>Application output:</strong> health score mapping, environmental risk alerts, and health-oriented route recommendation.</li>
</ul>

## App Design / 应用设计

The Sense+ prototype is designed as a mobile health-map service. Its current and planned functions include:

<div class="sense-grid">
  <div class="sense-card">
    <h3>Environmental Health Map</h3>
    <p>Visualizes urban environmental health scores at street level and helps users identify healthier urban spaces.</p>
  </div>
  <div class="sense-card">
    <h3>Healthy Route Planning</h3>
    <p>Recommends routes with better openness, more greenery, and cleaner air for commuting, walking, and outdoor activities.</p>
  </div>
  <div class="sense-card">
    <h3>Risk Alert</h3>
    <p>Provides environmental risk warnings based on real-time or frequently updated air pollution and spatial environment data.</p>
  </div>
  <div class="sense-card">
    <h3>Future Extensions</h3>
    <p>Future modules may include environmental exposure records, AI prediction, community interaction, AR environmental assessment, and smart-device connection.</p>
  </div>
</div>

## Innovation / 创新点

The main innovation of Sense+ lies in linking <strong>remote sensing, GIS, AI, and environmental health</strong> into a public-facing urban application. It builds a bridge from environmental data acquisition to health-oriented urban decision support, forming a practical workflow from <em>remote sensing indicators → environmental health index → map visualization → daily health guidance</em>.

This project demonstrates how geospatial technologies can support healthier, more equitable, and more human-centered cities.
