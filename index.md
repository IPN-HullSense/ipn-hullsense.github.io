---
layout: default
title: HullSense
---

<style>
/* 0. Top Navigation Bar */
.navbar {
    position: fixed;
    top: 0; left: 0; right: 0;
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    /* Use percentage padding to ensure consistent horizontal alignment */
    padding: 0 5% !important; 
    box-sizing: border-box !important;
    z-index: 10000;
    transition: all 0.3s ease;
    background: rgba(30, 30, 30, 0.3) !important;
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.navbar-logo {
    display: flex;
    align-items: center;
    gap: 12px;
    text-decoration: none;
    color: #ffffff !important; /* White text for dark background */
    font-weight: 800;
    font-size: 1.2rem;
}

.navbar-logo img {
    height: 40px !important;
    width: auto !important;
    display: block !important;
}

.navbar-links {
    display: flex;
    gap: 25px;
    list-style: none;
    margin: 0;
}

.navbar-links li {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 70px;
}

.navbar-links a {
    text-decoration: none;
    color: #eeeeee !important;
    font-weight: 600;
    font-size: 0.95rem;
    transition: color 0.3s ease;
    display: flex;
    align-items: center;
    height: 100%;
}

.navbar-links a:hover {
    color: #90caf9 !important;
}

/* 1. Reset Body and Background */
body {
margin: 0;
padding: 0;
background: url('{{ "/resources/hullskater.png" | relative_url }}') no-repeat center center fixed;
background-size: cover;
color: #fff;
overflow-x: hidden;
padding-top: 70px;
}

/* 2. Force Jekyll Minimal Theme to expand full width */
.wrapper {
background: none !important;
margin: 0 !important;
padding: 0 !important;
max-width: 100% !important;
width: 100% !important;
box-shadow: none !important;
display: block !important;
}

/* Hide default theme elements */
header, footer, .sidebar, #header, #footer {
display: none !important;
}

section {
background: none !important;
padding: 0 !important;
max-width: 100% !important;
margin: 0 !important;
width: 100% !important;
}

/* 3. Main Hero Container - Locked to the Left */
.home-hero {
  min-height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  text-shadow: 2px 2px 12px rgba(0, 0, 0, 0.9);
  padding-top: 80px; /* Fixed: Added the missing asterisk here */
  box-sizing: border-box;
}

/* 4. Left Side Content Block (Occupies roughly half the screen) */
.hero-left-content {
width: 50vw;
padding-left: 6%;
padding-right: 4%;
box-sizing: border-box;
z-index: 10;
}

.home-hero h1 {
font-size: clamp(2.5rem, 5vw, 4rem);
margin: 0 0 20px 0;
font-weight: 700;
color: #fff;
border: none !important;
line-height: 1.1;
}

.home-hero p {
font-size: 1.25rem;
max-width: 520px;
line-height: 1.6;
margin: 0 0 30px 0;
color: #f0f0f0;
}

/* Link rows */
.links-row {
margin-top: 20px;
font-size: 1.1rem;
display: flex;
flex-wrap: wrap;
align-items: center;
gap: 10px;
}

.learn-link {
display: inline-block;
color: #d8d8d8;
text-decoration: underline;
font-weight: 500;
/* transition: color 0.15s ease; */
}

.learn-link:hover { color: #a8c9e4; }

.home-hero h2 {
font-size: 1.6rem;
margin: 50px 0 20px 0;
font-weight: 600;
color: #fff;
border: none !important;
}

.project-list {
list-style: none;
padding: 0;
margin: 0;
}

.project-item {
margin: 18px 0;
}

.project-item a {
color: #d8d8d8 !important;
text-decoration: underline;
font-size: 1.2rem;
font-weight: 500;
}

.project-item a:hover {
color: #a8c9e4 !important;
}

/* 5. Mobile Fallback */
@media (max-width: 1024px) {
.hero-left-content {
width: 70vw;
}
}

@media (max-width: 768px) {
body { padding-top: 60px; }
.navbar { height: 60px; padding: 0 15px !important; }
.navbar-logo { font-size: 1rem; gap: 8px; }
.navbar-logo img { height: 32px; }
.navbar-links { gap: 15px; }
.navbar-links li { height: 60px; }
.navbar-links a { font-size: 0.85rem; }
.hero-left-content {
width: 100vw;
padding-left: 20px;
padding-right: 20px;
background: rgba(0, 0, 0, 0.5);
}
.home-hero { padding-top: 70px; }
.home-hero h1 { font-size: 2rem; margin: 0 0 15px 0; }
.home-hero p { font-size: 0.95rem; line-height: 1.5; }
.home-hero h2 { font-size: 1.2rem; margin: 30px 0 15px 0; }
.project-item a { font-size: 1rem; }
.learn-link { font-size: 0.9rem; }
}

@media (max-width: 480px) {
body { padding-top: 56px; }
.navbar { height: 56px; padding: 0 10px !important; }
.navbar-logo { font-size: 0.9rem; gap: 6px; }
.navbar-logo img { height: 28px; }
.navbar-links { gap: 10px; }
.navbar-links a { font-size: 0.75rem; }
.navbar-links li { height: 56px; }
.hero-left-content {
padding-left: 15px;
padding-right: 15px;
}
.home-hero h1 { font-size: 1.6rem; }
.home-hero p { font-size: 0.9rem; }
.home-hero h2 { font-size: 1rem; }
.project-item a { font-size: 0.95rem; }
}
</style>

<!-- Navigation Bar -->
<nav class="navbar">
  <a href="/" class="navbar-logo">
    <img src="/resources/hullskater-logo.png" alt="Logo" />
    <span>HullSense</span>
  </a>
  <ul class="navbar-links">
    <li><a href="/">Home</a></li>
    <li><a href="/pages/about/">About</a></li>
    <li><a href="/pages/projects/">Projects</a></li>
  </ul>
</nav>

<div class="home-hero">
<div class="hero-left-content">
<h1>HullSense</h1>
<p>Research of resilient methods for perceptive detection, localization and mapping of submerged structures, with ship hulls and harbors as the primary application case.</p>

<div class="links-row">
  <a class="learn-link" href="https://www.jotun.com/ww-en/industries/solutions-and-brands/hull-skating-solutions/overview" target="_blank" rel="noopener">About Hull Skating Solutions</a>
  <span aria-hidden="true" style="opacity: 0.5;">|</span>
  <a class="learn-link" href="{{ '/pages/about/' | relative_url }}">About HullSense</a>
</div>

<h2>Available Master Project Proposals</h2>
<ul class="project-list">
  <li class="project-item">
    <a href="{{ '/pages/varos-future-design/#varos-track1' | relative_url }}">
      VAROS - Complex AI- and Model-Driven Environments & Optical Realism
    </a>
  </li>
  <li class="project-item">
    <a href="{{ '/pages/varos-future-design/#varos-track2' | relative_url }}">
      VAROS - Advanced Sensor Synthesis
    </a>
  </li>
  <li class="project-item">
    <a href="{{ '/pages/varos-future-design/#varos-track3' | relative_url }}">
      VAROS - Intelligent Motion & Autonomous Control
    </a>
  </li>
</ul>
</div>
</div>