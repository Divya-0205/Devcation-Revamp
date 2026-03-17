<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Devcation Hack 'N' Solve — IIT Delhi 2026</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700;800&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet" />
  <style>
    /* ===========================
       CSS RESET & VARIABLES
    =========================== */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --bg-primary:   #06070F;
      --bg-secondary: #0D0F1E;
      --bg-card:      #111327;
      --bg-card-hover:#161933;
      --accent-blue:  #5B8DEF;
      --accent-purple:#9B6DFF;
      --accent-teal:  #00D4AA;
      --accent-pink:  #FF6B9D;
      --accent-orange:#FF8C42;
      --text-primary: #F0F2FF;
      --text-secondary:#A8B2D8;
      --text-muted:   #606888;
      --border:       rgba(255,255,255,0.07);
      --border-accent:rgba(91,141,239,0.35);
      --glow-blue:    rgba(91,141,239,0.18);
      --glow-purple:  rgba(155,109,255,0.18);
      --radius-sm:    8px;
      --radius-md:    16px;
      --radius-lg:    24px;
      --radius-xl:    32px;
      --font-heading: 'Space Grotesk', sans-serif;
      --font-body:    'Inter', sans-serif;
      --nav-height:   72px;
      --max-w:        1200px;
    }

    html { scroll-behavior: smooth; }

    body {
      background: var(--bg-primary);
      color: var(--text-primary);
      font-family: var(--font-body);
      font-size: 16px;
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* ===========================
       UTILITY CLASSES
    =========================== */
    .container { max-width: var(--max-w); margin: 0 auto; padding: 0 24px; }
    .section    { padding: 96px 0; }
    .section--sm{ padding: 64px 0; }

    .tag {
      display: inline-flex; align-items: center; gap: 6px;
      font-size: 11px; font-weight: 600; letter-spacing: 1.2px; text-transform: uppercase;
      padding: 5px 12px; border-radius: 100px;
      background: rgba(91,141,239,0.12); color: var(--accent-blue);
      border: 1px solid rgba(91,141,239,0.25);
    }
    .tag--teal  { background: rgba(0,212,170,0.10); color: var(--accent-teal);  border-color: rgba(0,212,170,0.25); }
    .tag--purple{ background: rgba(155,109,255,0.10); color: var(--accent-purple); border-color: rgba(155,109,255,0.25); }
    .tag--pink  { background: rgba(255,107,157,0.10); color: var(--accent-pink);  border-color: rgba(255,107,157,0.25); }
    .tag--orange{ background: rgba(255,140,66,0.10);  color: var(--accent-orange); border-color: rgba(255,140,66,0.25); }

    .gradient-text {
      background: linear-gradient(135deg, var(--accent-blue) 0%, var(--accent-purple) 60%, var(--accent-pink) 100%);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
    }

    .section-label {
      font-size: 12px; font-weight: 600; letter-spacing: 2px; text-transform: uppercase;
      color: var(--accent-teal); margin-bottom: 12px; display: block;
    }
    .section-title {
      font-family: var(--font-heading); font-size: clamp(28px, 4vw, 42px);
      font-weight: 700; line-height: 1.15; color: var(--text-primary);
      margin-bottom: 16px;
    }
    .section-sub {
      font-size: 17px; color: var(--text-secondary); max-width: 600px; line-height: 1.7;
    }

    /* ===========================
       NAVIGATION
    =========================== */
    .nav {
      position: fixed; top: 0; left: 0; right: 0; z-index: 1000;
      height: var(--nav-height);
      background: rgba(6,7,15,0.75);
      backdrop-filter: blur(20px) saturate(180%);
      -webkit-backdrop-filter: blur(20px) saturate(180%);
      border-bottom: 1px solid var(--border);
      transition: background 0.3s ease;
    }
    .nav-inner {
      max-width: var(--max-w); margin: 0 auto; padding: 0 24px;
      height: 100%; display: flex; align-items: center; justify-content: space-between;
    }
    .nav-logo {
      display: flex; align-items: center; gap: 10px;
      font-family: var(--font-heading); font-weight: 800; font-size: 20px;
      text-decoration: none; color: var(--text-primary);
    }
    .nav-logo-icon {
      width: 34px; height: 34px; border-radius: 10px;
      background: linear-gradient(135deg, var(--accent-blue), var(--accent-purple));
      display: flex; align-items: center; justify-content: center;
      font-size: 16px; font-weight: 800;
    }
    .nav-links {
      display: flex; align-items: center; gap: 8px;
      list-style: none;
    }
    .nav-links a {
      font-size: 14px; font-weight: 500; color: var(--text-secondary);
      text-decoration: none; padding: 6px 14px; border-radius: 8px;
      transition: color 0.2s, background 0.2s;
    }
    .nav-links a:hover { color: var(--text-primary); background: rgba(255,255,255,0.06); }

    .nav-cta {
      display: flex; align-items: center; gap: 12px;
    }
    .btn-ghost {
      font-size: 14px; font-weight: 500; color: var(--text-secondary);
      background: none; border: none; cursor: pointer;
      padding: 8px 16px; border-radius: 8px;
      transition: color 0.2s, background 0.2s;
      text-decoration: none;
    }
    .btn-ghost:hover { color: var(--text-primary); background: rgba(255,255,255,0.06); }

    .btn-primary {
      display: inline-flex; align-items: center; gap: 8px;
      font-size: 14px; font-weight: 600; font-family: var(--font-body);
      color: #fff; background: linear-gradient(135deg, var(--accent-blue), var(--accent-purple));
      border: none; cursor: pointer; padding: 10px 22px; border-radius: 10px;
      text-decoration: none;
      box-shadow: 0 0 20px rgba(91,141,239,0.3);
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .btn-primary:hover { transform: translateY(-1px); box-shadow: 0 0 28px rgba(91,141,239,0.45); }
    .btn-primary:active{ transform: translateY(0); }

    .btn-primary--lg {
      font-size: 16px; padding: 14px 32px; border-radius: 14px;
      box-shadow: 0 0 32px rgba(91,141,239,0.35);
    }

    .btn-outline {
      display: inline-flex; align-items: center; gap: 8px;
      font-size: 15px; font-weight: 600; font-family: var(--font-body);
      color: var(--text-primary); background: transparent;
      border: 1.5px solid var(--border-accent); cursor: pointer;
      padding: 13px 28px; border-radius: 14px; text-decoration: none;
      transition: background 0.2s, border-color 0.2s;
    }
    .btn-outline:hover { background: var(--glow-blue); border-color: var(--accent-blue); }

    /* Hamburger */
    .hamburger {
      display: none; flex-direction: column; gap: 5px;
      cursor: pointer; padding: 8px; border: none; background: none;
    }
    .hamburger span {
      display: block; width: 22px; height: 2px;
      background: var(--text-secondary); border-radius: 2px;
      transition: transform 0.3s, opacity 0.3s;
    }
    .mobile-menu {
      display: none; position: fixed; top: var(--nav-height); left: 0; right: 0;
      background: rgba(13,15,30,0.98); backdrop-filter: blur(20px);
      padding: 24px; z-index: 999;
      border-bottom: 1px solid var(--border);
    }
    .mobile-menu.open { display: block; }
    .mobile-menu a {
      display: block; padding: 14px 0;
      font-size: 16px; font-weight: 500; color: var(--text-secondary);
      text-decoration: none; border-bottom: 1px solid var(--border);
      transition: color 0.2s;
    }
    .mobile-menu a:hover { color: var(--text-primary); }
    .mobile-menu .btn-primary { width: 100%; justify-content: center; margin-top: 20px; font-size: 15px; }

    /* ===========================
       HERO SECTION
    =========================== */
    .hero {
      min-height: 100vh; display: flex; flex-direction: column; justify-content: center;
      padding-top: var(--nav-height); position: relative; overflow: hidden;
    }
    .hero-bg {
      position: absolute; inset: 0; pointer-events: none;
    }
    .hero-orb {
      position: absolute; border-radius: 50%; filter: blur(120px); opacity: 0.35;
    }
    .hero-orb-1 {
      width: 600px; height: 600px;
      background: radial-gradient(circle, var(--accent-blue), transparent 70%);
      top: -100px; right: -150px;
    }
    .hero-orb-2 {
      width: 500px; height: 500px;
      background: radial-gradient(circle, var(--accent-purple), transparent 70%);
      bottom: -100px; left: -100px;
    }
    .hero-orb-3 {
      width: 300px; height: 300px;
      background: radial-gradient(circle, var(--accent-teal), transparent 70%);
      top: 50%; left: 40%; transform: translate(-50%,-50%);
      opacity: 0.15;
    }
    /* Grid pattern */
    .hero-grid {
      position: absolute; inset: 0;
      background-image:
        linear-gradient(rgba(255,255,255,0.025) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,255,255,0.025) 1px, transparent 1px);
      background-size: 60px 60px;
      mask-image: radial-gradient(ellipse 80% 80% at 50% 50%, black 20%, transparent 100%);
    }

    .hero-content {
      position: relative; z-index: 2;
      max-width: var(--max-w); margin: 0 auto; padding: 80px 24px 64px;
      display: grid; grid-template-columns: 1fr 400px; gap: 64px; align-items: center;
    }

    .hero-badge {
      display: inline-flex; align-items: center; gap: 8px;
      background: rgba(0,212,170,0.08); border: 1px solid rgba(0,212,170,0.2);
      border-radius: 100px; padding: 6px 16px 6px 8px; margin-bottom: 24px;
    }
    .hero-badge-dot {
      width: 8px; height: 8px; border-radius: 50%;
      background: var(--accent-teal);
      box-shadow: 0 0 8px var(--accent-teal);
      animation: pulse 2s infinite;
    }
    @keyframes pulse {
      0%,100% { opacity:1; transform:scale(1); }
      50% { opacity:0.5; transform:scale(0.85); }
    }
    .hero-badge span { font-size: 13px; font-weight: 500; color: var(--accent-teal); }

    .hero-title {
      font-family: var(--font-heading);
      font-size: clamp(38px, 6vw, 72px);
      font-weight: 800; line-height: 1.05; letter-spacing: -1.5px;
      margin-bottom: 20px;
    }
    .hero-title em { font-style: normal; }

    .hero-desc {
      font-size: 18px; color: var(--text-secondary); line-height: 1.75;
      max-width: 520px; margin-bottom: 36px;
    }

    .hero-actions {
      display: flex; flex-wrap: wrap; align-items: center; gap: 14px;
      margin-bottom: 48px;
    }

    .hero-stats {
      display: flex; align-items: center; gap: 32px; flex-wrap: wrap;
    }
    .hero-stat {}
    .hero-stat-value {
      font-family: var(--font-heading); font-size: 28px; font-weight: 800;
      background: linear-gradient(135deg, var(--accent-blue), var(--accent-purple));
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
    }
    .hero-stat-label { font-size: 13px; color: var(--text-muted); margin-top: 2px; }
    .hero-stat-divider { width: 1px; height: 36px; background: var(--border); }

    /* Countdown card */
    .countdown-card {
      background: var(--bg-card);
      border: 1px solid var(--border);
      border-radius: var(--radius-xl);
      padding: 32px 28px;
      box-shadow: 0 0 60px rgba(0,0,0,0.5), 0 0 0 1px rgba(255,255,255,0.03);
      position: relative; overflow: hidden;
    }
    .countdown-card::before {
      content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
      background: linear-gradient(90deg, var(--accent-blue), var(--accent-purple), var(--accent-teal));
    }
    .countdown-label {
      font-size: 12px; font-weight: 600; letter-spacing: 1.5px; text-transform: uppercase;
      color: var(--text-muted); margin-bottom: 20px;
      display: flex; align-items: center; gap: 8px;
    }
    .countdown-label::after {
      content:''; flex:1; height:1px; background: var(--border);
    }
    .countdown-grid {
      display: grid; grid-template-columns: repeat(4,1fr); gap: 10px;
      margin-bottom: 28px;
    }
    .countdown-unit {
      background: rgba(255,255,255,0.04);
      border: 1px solid var(--border);
      border-radius: var(--radius-md); padding: 16px 8px;
      text-align: center;
    }
    .countdown-number {
      font-family: var(--font-heading); font-size: 32px; font-weight: 800;
      background: linear-gradient(135deg, #fff, var(--text-secondary));
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
      line-height: 1;
    }
    .countdown-unit-label { font-size: 10px; color: var(--text-muted); margin-top: 6px; text-transform: uppercase; letter-spacing: 0.8px; }

    .event-meta {
      display: flex; flex-direction: column; gap: 12px;
    }
    .event-meta-row {
      display: flex; align-items: center; gap: 10px;
      font-size: 14px; color: var(--text-secondary);
    }
    .event-meta-icon {
      width: 32px; height: 32px; border-radius: 8px;
      background: rgba(255,255,255,0.05); display: flex; align-items: center; justify-content: center;
      font-size: 14px; flex-shrink: 0;
    }
    .event-meta-row strong { color: var(--text-primary); font-weight: 600; }

    /* ===========================
       SCROLL INDICATOR
    =========================== */
    .scroll-indicator {
      position: absolute; bottom: 32px; left: 50%; transform: translateX(-50%);
      display: flex; flex-direction: column; align-items: center; gap: 8px;
      animation: bobble 2s ease-in-out infinite;
    }
    .scroll-indicator span { font-size: 11px; color: var(--text-muted); letter-spacing: 1px; text-transform: uppercase; }
    .scroll-line {
      width: 1px; height: 40px;
      background: linear-gradient(to bottom, var(--text-muted), transparent);
    }
    @keyframes bobble {
      0%,100% { transform: translateX(-50%) translateY(0); }
      50% { transform: translateX(-50%) translateY(8px); }
    }

    /* ===========================
       ABOUT SECTION
    =========================== */
    .about-grid {
      display: grid; grid-template-columns: 1fr 1fr; gap: 80px;
      align-items: center;
    }
    .about-visual {
      position: relative;
    }
    .about-main-card {
      background: var(--bg-card); border: 1px solid var(--border);
      border-radius: var(--radius-xl); padding: 36px;
      box-shadow: 0 24px 64px rgba(0,0,0,0.4);
      position: relative; z-index: 2;
    }
    .about-icon-grid {
      display: grid; grid-template-columns: 1fr 1fr; gap: 12px;
      margin-bottom: 24px;
    }
    .about-icon-item {
      background: rgba(255,255,255,0.04); border: 1px solid var(--border);
      border-radius: var(--radius-md); padding: 20px 16px;
      text-align: center;
    }
    .about-icon-item .icon { font-size: 28px; margin-bottom: 8px; }
    .about-icon-item .label { font-size: 12px; color: var(--text-muted); font-weight: 500; }
    .about-floating-tag {
      position: absolute; background: var(--bg-card);
      border: 1px solid var(--border-accent); border-radius: var(--radius-md);
      padding: 12px 16px; font-size: 13px; font-weight: 600;
      display: flex; align-items: center; gap: 8px; z-index: 3;
      box-shadow: 0 8px 24px rgba(0,0,0,0.3);
    }
    .about-floating-1 { top: -20px; right: -20px; color: var(--accent-teal); }
    .about-floating-2 { bottom: -16px; left: -16px; color: var(--accent-purple); }
    .about-floating-dot {
      width: 8px; height: 8px; border-radius: 50%;
      background: currentColor; box-shadow: 0 0 8px currentColor;
    }

    .feature-list { margin-top: 32px; display: flex; flex-direction: column; gap: 16px; }
    .feature-item {
      display: flex; align-items: flex-start; gap: 14px;
    }
    .feature-icon {
      width: 40px; height: 40px; border-radius: 10px; flex-shrink: 0;
      display: flex; align-items: center; justify-content: center; font-size: 18px;
    }
    .feature-icon--blue { background: rgba(91,141,239,0.12); }
    .feature-icon--purple { background: rgba(155,109,255,0.12); }
    .feature-icon--teal { background: rgba(0,212,170,0.12); }
    .feature-icon--pink { background: rgba(255,107,157,0.12); }
    .feature-text h4 { font-size: 15px; font-weight: 600; margin-bottom: 4px; }
    .feature-text p { font-size: 14px; color: var(--text-secondary); line-height: 1.6; }

    /* ===========================
       TIMELINE SECTION
    =========================== */
    .timeline-header { text-align: center; margin-bottom: 64px; }
    .timeline-header .section-sub { margin: 0 auto; }

    .timeline {
      position: relative; max-width: 860px; margin: 0 auto;
    }
    .timeline::before {
      content: ''; position: absolute; left: 50%; transform: translateX(-50%);
      top: 24px; bottom: 24px; width: 2px;
      background: linear-gradient(to bottom, var(--accent-blue), var(--accent-purple), var(--accent-teal));
      opacity: 0.3;
    }
    .timeline-item {
      display: grid; grid-template-columns: 1fr auto 1fr; gap: 24px;
      align-items: start; margin-bottom: 48px; position: relative;
    }
    .timeline-item:nth-child(odd) .timeline-card  { grid-column: 1; grid-row: 1; }
    .timeline-item:nth-child(odd) .timeline-empty { grid-column: 3; grid-row: 1; }
    .timeline-item:nth-child(even) .timeline-card  { grid-column: 3; grid-row: 1; order: 3; }
    .timeline-item:nth-child(even) .timeline-empty { grid-column: 1; grid-row: 1; }
    .timeline-item:nth-child(even) .timeline-node  { order: 2; }

    .timeline-node {
      display: flex; flex-direction: column; align-items: center; gap: 0;
      grid-column: 2; position: relative; z-index: 2;
    }
    .timeline-dot {
      width: 48px; height: 48px; border-radius: 50%;
      background: var(--bg-card);
      border: 2px solid var(--accent-blue);
      display: flex; align-items: center; justify-content: center;
      font-size: 18px;
      box-shadow: 0 0 20px var(--glow-blue);
    }
    .timeline-dot--purple { border-color: var(--accent-purple); box-shadow: 0 0 20px var(--glow-purple); }
    .timeline-dot--teal   { border-color: var(--accent-teal);   box-shadow: 0 0 16px rgba(0,212,170,0.2); }
    .timeline-dot--pink   { border-color: var(--accent-pink);   box-shadow: 0 0 16px rgba(255,107,157,0.2); }

    .timeline-card {
      background: var(--bg-card); border: 1px solid var(--border);
      border-radius: var(--radius-lg); padding: 24px;
      transition: border-color 0.3s, transform 0.3s, box-shadow 0.3s;
      cursor: default;
    }
    .timeline-card:hover {
      border-color: var(--border-accent);
      transform: translateY(-2px);
      box-shadow: 0 12px 32px rgba(0,0,0,0.3), 0 0 0 1px rgba(91,141,239,0.1);
    }
    .timeline-step {
      font-size: 11px; font-weight: 700; letter-spacing: 1.5px;
      text-transform: uppercase; color: var(--text-muted);
      margin-bottom: 8px;
    }
    .timeline-card-title {
      font-family: var(--font-heading); font-size: 18px; font-weight: 700;
      margin-bottom: 8px; color: var(--text-primary);
    }
    .timeline-date {
      display: inline-flex; align-items: center; gap: 6px;
      font-size: 13px; color: var(--accent-blue); font-weight: 500;
      margin-bottom: 12px;
    }
    .timeline-date--purple { color: var(--accent-purple); }
    .timeline-date--teal   { color: var(--accent-teal); }
    .timeline-date--pink   { color: var(--accent-pink); }
    .timeline-card p { font-size: 14px; color: var(--text-secondary); line-height: 1.65; }
    .timeline-empty {}

    /* ===========================
       TRACKS SECTION
    =========================== */
    .tracks-header { margin-bottom: 48px; }
    .tracks-grid {
      display: grid; grid-template-columns: repeat(2, 1fr); gap: 24px;
    }
    .track-card {
      background: var(--bg-card); border: 1px solid var(--border);
      border-radius: var(--radius-xl); padding: 36px;
      position: relative; overflow: hidden;
      transition: transform 0.3s, box-shadow 0.3s, border-color 0.3s;
    }
    .track-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 20px 60px rgba(0,0,0,0.4);
    }
    .track-card--premium {
      border-color: rgba(155,109,255,0.3);
      background: linear-gradient(145deg, rgba(155,109,255,0.05) 0%, var(--bg-card) 100%);
    }
    .track-card--premium:hover { box-shadow: 0 20px 60px rgba(0,0,0,0.4), 0 0 0 1px rgba(155,109,255,0.2); }
    .track-card--open {
      border-color: rgba(91,141,239,0.3);
    }
    .track-card--open:hover { box-shadow: 0 20px 60px rgba(0,0,0,0.4), 0 0 0 1px rgba(91,141,239,0.2); }
    .track-glow {
      position: absolute; width: 200px; height: 200px; border-radius: 50%;
      filter: blur(80px); opacity: 0.12; pointer-events: none;
      top: -40px; right: -40px;
    }
    .track-glow--purple { background: var(--accent-purple); }
    .track-glow--blue   { background: var(--accent-blue); }
    .track-badge-row {
      display: flex; align-items: center; justify-content: space-between;
      margin-bottom: 20px;
    }
    .track-icon {
      width: 52px; height: 52px; border-radius: 14px;
      display: flex; align-items: center; justify-content: center;
      font-size: 24px;
    }
    .track-icon--purple { background: rgba(155,109,255,0.12); }
    .track-icon--blue   { background: rgba(91,141,239,0.12); }
    .track-title {
      font-family: var(--font-heading); font-size: 22px; font-weight: 700;
      margin-bottom: 10px;
    }
    .track-subtitle {
      font-size: 14px; color: var(--text-secondary); margin-bottom: 20px; line-height: 1.65;
    }
    .track-features {
      list-style: none; display: flex; flex-direction: column; gap: 10px;
      margin-bottom: 28px;
    }
    .track-features li {
      display: flex; align-items: center; gap: 10px;
      font-size: 14px; color: var(--text-secondary);
    }
    .track-features li::before {
      content: ''; width: 18px; height: 18px; border-radius: 50%; flex-shrink: 0;
      background: rgba(91,141,239,0.15); border: 1px solid rgba(91,141,239,0.3);
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12'%3E%3Cpath d='M2 6l3 3 5-5' stroke='%235B8DEF' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: no-repeat; background-position: center;
    }
    .track-card--premium .track-features li::before {
      background-color: rgba(155,109,255,0.15); border-color: rgba(155,109,255,0.3);
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12'%3E%3Cpath d='M2 6l3 3 5-5' stroke='%239B6DFF' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
    }
    .track-prize {
      display: flex; align-items: center; gap: 8px;
      font-family: var(--font-heading); font-size: 24px; font-weight: 700;
      color: var(--accent-orange); margin-bottom: 6px;
    }
    .track-prize-label { font-size: 13px; color: var(--text-muted); }

    /* ===========================
       ELIGIBILITY SECTION
    =========================== */
    .eligibility-wrapper {
      background: var(--bg-secondary); border: 1px solid var(--border);
      border-radius: var(--radius-xl); padding: 48px;
    }
    .eligibility-inner {
      display: grid; grid-template-columns: 1fr 1fr; gap: 64px; align-items: center;
    }
    .eligibility-tags {
      display: flex; flex-wrap: wrap; gap: 10px; margin-top: 24px;
    }
    .eligibility-tag {
      display: inline-flex; align-items: center; gap: 8px;
      background: rgba(255,255,255,0.05); border: 1px solid var(--border);
      border-radius: 10px; padding: 10px 16px;
      font-size: 14px; font-weight: 500; color: var(--text-secondary);
      transition: background 0.2s, border-color 0.2s;
    }
    .eligibility-tag:hover { background: rgba(255,255,255,0.08); border-color: rgba(255,255,255,0.12); color: var(--text-primary); }
    .eligibility-tag .dot { width: 8px; height: 8px; border-radius: 50%; background: var(--accent-teal); }

    .checklist { display: flex; flex-direction: column; gap: 14px; }
    .check-item {
      display: flex; align-items: flex-start; gap: 12px;
      font-size: 15px; color: var(--text-secondary);
    }
    .check-item .check-icon {
      width: 24px; height: 24px; border-radius: 8px; flex-shrink: 0;
      background: rgba(0,212,170,0.12); border: 1px solid rgba(0,212,170,0.25);
      display: flex; align-items: center; justify-content: center;
      font-size: 12px; color: var(--accent-teal);
      margin-top: 1px;
    }
    .check-item strong { color: var(--text-primary); font-weight: 600; }

    /* ===========================
       FAQ SECTION
    =========================== */
    .faq-header { text-align: center; margin-bottom: 56px; }
    .faq-grid {
      max-width: 780px; margin: 0 auto;
      display: flex; flex-direction: column; gap: 12px;
    }
    .faq-item {
      background: var(--bg-card); border: 1px solid var(--border);
      border-radius: var(--radius-md); overflow: hidden;
      transition: border-color 0.3s;
    }
    .faq-item.open { border-color: var(--border-accent); }
    .faq-question {
      display: flex; align-items: center; justify-content: space-between;
      padding: 20px 24px; cursor: pointer;
      font-size: 15px; font-weight: 600; color: var(--text-primary);
      background: none; border: none; width: 100%; text-align: left;
    }
    .faq-arrow {
      width: 28px; height: 28px; border-radius: 8px;
      background: rgba(255,255,255,0.05);
      display: flex; align-items: center; justify-content: center;
      font-size: 12px; flex-shrink: 0; margin-left: 12px;
      transition: transform 0.3s, background 0.3s;
    }
    .faq-item.open .faq-arrow { transform: rotate(180deg); background: rgba(91,141,239,0.15); }
    .faq-answer {
      display: none; padding: 0 24px 20px;
      font-size: 14px; color: var(--text-secondary); line-height: 1.75;
    }
    .faq-item.open .faq-answer { display: block; }

    /* ===========================
       CTA SECTION
    =========================== */
    .cta-section {
      position: relative; overflow: hidden;
      background: linear-gradient(135deg, rgba(91,141,239,0.08) 0%, rgba(155,109,255,0.08) 100%);
      border: 1px solid rgba(91,141,239,0.15);
      border-radius: var(--radius-xl);
      margin: 0 24px 96px;
      padding: 80px 48px;
      text-align: center;
    }
    .cta-orb-1 {
      position: absolute; width: 300px; height: 300px; border-radius: 50%;
      background: radial-gradient(circle, var(--accent-blue), transparent);
      filter: blur(80px); opacity: 0.15;
      top: -80px; left: -80px; pointer-events: none;
    }
    .cta-orb-2 {
      position: absolute; width: 300px; height: 300px; border-radius: 50%;
      background: radial-gradient(circle, var(--accent-purple), transparent);
      filter: blur(80px); opacity: 0.15;
      bottom: -80px; right: -80px; pointer-events: none;
    }
    .cta-content { position: relative; z-index: 2; max-width: 600px; margin: 0 auto; }
    .cta-title {
      font-family: var(--font-heading); font-size: clamp(30px, 4vw, 48px);
      font-weight: 800; line-height: 1.1; letter-spacing: -1px; margin-bottom: 16px;
    }
    .cta-desc { font-size: 17px; color: var(--text-secondary); margin-bottom: 36px; line-height: 1.7; }
    .cta-actions { display: flex; flex-wrap: wrap; gap: 14px; justify-content: center; }
    .deadline-note {
      display: inline-flex; align-items: center; gap: 6px;
      font-size: 13px; color: var(--text-muted); margin-top: 20px;
    }

    /* ===========================
       FOOTER
    =========================== */
    .footer {
      border-top: 1px solid var(--border);
      padding: 48px 0 32px;
    }
    .footer-inner {
      max-width: var(--max-w); margin: 0 auto; padding: 0 24px;
      display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 40px;
    }
    .footer-brand p {
      font-size: 14px; color: var(--text-muted); line-height: 1.7; margin-top: 12px;
    }
    .footer-col h4 {
      font-size: 13px; font-weight: 600; letter-spacing: 1px; text-transform: uppercase;
      color: var(--text-muted); margin-bottom: 16px;
    }
    .footer-col ul { list-style: none; display: flex; flex-direction: column; gap: 10px; }
    .footer-col ul a {
      font-size: 14px; color: var(--text-secondary); text-decoration: none;
      transition: color 0.2s;
    }
    .footer-col ul a:hover { color: var(--text-primary); }
    .footer-bottom {
      max-width: var(--max-w); margin: 32px auto 0; padding: 24px 24px 0;
      border-top: 1px solid var(--border);
      display: flex; align-items: center; justify-content: space-between;
      flex-wrap: wrap; gap: 12px;
    }
    .footer-bottom p { font-size: 13px; color: var(--text-muted); }

    /* ===========================
       DESIGN SYSTEM SECTION
    =========================== */
    .design-section {
      background: var(--bg-secondary);
      padding: 64px 0;
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
    }
    .design-grid {
      display: grid; grid-template-columns: repeat(3, 1fr); gap: 32px;
    }
    .design-card {
      background: var(--bg-card); border: 1px solid var(--border);
      border-radius: var(--radius-lg); padding: 28px;
    }
    .design-card h4 {
      font-size: 12px; font-weight: 700; letter-spacing: 1.5px; text-transform: uppercase;
      color: var(--text-muted); margin-bottom: 20px;
    }
    .color-swatches {
      display: flex; flex-direction: column; gap: 10px;
    }
    .color-swatch {
      display: flex; align-items: center; gap: 12px;
    }
    .swatch { width: 40px; height: 40px; border-radius: 10px; flex-shrink: 0; }
    .swatch-info { }
    .swatch-name { font-size: 13px; font-weight: 600; color: var(--text-primary); }
    .swatch-hex  { font-size: 11px; color: var(--text-muted); font-family: monospace; }
    .type-sample { display: flex; flex-direction: column; gap: 14px; }
    .type-item {}
    .type-label { font-size: 11px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px; margin-bottom: 4px; }
    .type-preview-h1 { font-family: var(--font-heading); font-size: 32px; font-weight: 800; line-height: 1.1; }
    .type-preview-h2 { font-family: var(--font-heading); font-size: 22px; font-weight: 700; }
    .type-preview-h3 { font-family: var(--font-heading); font-size: 16px; font-weight: 600; }
    .type-preview-body { font-size: 14px; color: var(--text-secondary); line-height: 1.65; }
    .component-samples { display: flex; flex-direction: column; gap: 14px; }
    .component-row { display: flex; flex-wrap: wrap; gap: 8px; align-items: center; }

    /* ===========================
       RESPONSIVE
    =========================== */
    @media (max-width: 1024px) {
      .hero-content { grid-template-columns: 1fr; gap: 48px; padding: 64px 24px; }
      .countdown-card { max-width: 480px; }
      .about-grid { grid-template-columns: 1fr; gap: 48px; }
      .about-visual { order: -1; }
      .design-grid { grid-template-columns: 1fr; }
      .footer-inner { grid-template-columns: 1fr 1fr; }
    }

    @media (max-width: 768px) {
      .nav-links, .nav-cta .btn-ghost { display: none; }
      .hamburger { display: flex; }
      .hero-stats { gap: 20px; }
      .section { padding: 64px 0; }
      .timeline::before { left: 24px; }
      .timeline-item { grid-template-columns: 48px 1fr; gap: 16px; }
      .timeline-item:nth-child(odd) .timeline-card,
      .timeline-item:nth-child(even) .timeline-card { grid-column: 2; }
      .timeline-empty { display: none; }
      .timeline-item:nth-child(even) .timeline-node { order: 0; grid-column: 1; }
      .timeline-item:nth-child(even) .timeline-card { grid-column: 2; order: 1; }
      .tracks-grid { grid-template-columns: 1fr; }
      .eligibility-inner { grid-template-columns: 1fr; gap: 36px; }
      .eligibility-wrapper { padding: 32px 24px; }
      .cta-section { margin: 0 16px 64px; padding: 56px 24px; }
      .footer-inner { grid-template-columns: 1fr; }
      .footer-bottom { flex-direction: column; text-align: center; }
      .countdown-grid { grid-template-columns: repeat(2,1fr); }
    }

    @media (max-width: 480px) {
      .hero-title { letter-spacing: -0.8px; }
      .hero-actions { flex-direction: column; }
      .hero-actions a { width: 100%; justify-content: center; }
      .btn-primary--lg, .btn-outline { width: 100%; justify-content: center; }
    }

    /* ===========================
       ANIMATED PARTICLES (subtle)
    =========================== */
    .particles {
      position: absolute; inset: 0; pointer-events: none; overflow: hidden;
    }
    .particle {
      position: absolute; width: 2px; height: 2px; background: rgba(255,255,255,0.3);
      border-radius: 50%;
      animation: float linear infinite;
    }
    @keyframes float {
      0%   { transform: translateY(100vh) translateX(0); opacity: 0; }
      10%  { opacity: 1; }
      90%  { opacity: 1; }
      100% { transform: translateY(-10vh) translateX(var(--drift)); opacity: 0; }
    }

    /* ===========================
       SPONSORS / ORGANIZERS STRIP
    =========================== */
    .organizers-strip {
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
      padding: 28px 0;
      background: var(--bg-secondary);
    }
    .organizers-inner {
      max-width: var(--max-w); margin: 0 auto; padding: 0 24px;
      display: flex; align-items: center; justify-content: center; gap: 40px;
      flex-wrap: wrap;
    }
    .organizer-label { font-size: 12px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px; }
    .org-divider { width: 1px; height: 28px; background: var(--border); }
    .org-badge {
      display: flex; align-items: center; gap: 10px;
      font-size: 14px; font-weight: 600; color: var(--text-secondary);
    }
    .org-badge-icon {
      width: 32px; height: 32px; border-radius: 8px;
      background: rgba(255,255,255,0.07);
      display: flex; align-items: center; justify-content: center; font-size: 14px;
    }
  </style>
</head>
<body>

  <!-- ========================
       NAVIGATION
  ========================= -->
  <nav class="nav" role="navigation" aria-label="Main navigation">
    <div class="nav-inner">
      <a href="#" class="nav-logo" aria-label="Devcation home">
        <div class="nav-logo-icon">D</div>
        Devcation
      </a>
      <ul class="nav-links" role="list">
        <li><a href="#about">About</a></li>
        <li><a href="#timeline">Timeline</a></li>
        <li><a href="#tracks">Tracks</a></li>
        <li><a href="#eligibility">Eligibility</a></li>
        <li><a href="#faq">FAQ</a></li>
      </ul>
      <div class="nav-cta">
        <a href="#" class="btn-ghost">Sign In</a>
        <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary" target="_blank" rel="noopener">
          Register Now →
        </a>
      </div>
      <button class="hamburger" onclick="toggleMenu()" aria-label="Toggle menu" aria-expanded="false">
        <span></span><span></span><span></span>
      </button>
    </div>
  </nav>

  <!-- Mobile menu -->
  <div class="mobile-menu" id="mobileMenu" role="dialog" aria-label="Mobile navigation">
    <a href="#about" onclick="closeMenu()">About</a>
    <a href="#timeline" onclick="closeMenu()">Timeline</a>
    <a href="#tracks" onclick="closeMenu()">Tracks</a>
    <a href="#eligibility" onclick="closeMenu()">Eligibility</a>
    <a href="#faq" onclick="closeMenu()">FAQ</a>
    <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary" target="_blank" rel="noopener">
      Register Now →
    </a>
  </div>

  <!-- ========================
       HERO SECTION
  ========================= -->
  <section class="hero" aria-label="Hero">
    <div class="hero-bg">
      <div class="hero-grid"></div>
      <div class="hero-orb hero-orb-1"></div>
      <div class="hero-orb hero-orb-2"></div>
      <div class="hero-orb hero-orb-3"></div>
      <div class="particles" id="particles"></div>
    </div>

    <div class="hero-content">
      <!-- Left: Text -->
      <div class="hero-text">
        <div class="hero-badge">
          <div class="hero-badge-dot"></div>
          <span>Registration Open · IIT Delhi 2026</span>
        </div>

        <h1 class="hero-title">
          <em class="gradient-text">Hack. Build.</em><br />
          <em>Solve.</em><br />
          <span style="color: var(--text-secondary); font-size: 0.65em; font-weight: 500; letter-spacing: -0.5px;">Devcation Hack 'N' Solve</span>
        </h1>

        <p class="hero-desc">
          A flagship hackathon by <strong>GDG IGDTUW</strong> × <strong>GDG IIT Delhi</strong> — where developers, innovators, and students unite to build technology that matters. Code, collaborate, and create at IIT Delhi.
        </p>

        <div class="hero-actions">
          <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary btn-primary--lg" target="_blank" rel="noopener">
            🚀 Register Now
          </a>
          <a href="#timeline" class="btn-outline">
            View Timeline
          </a>
        </div>

        <div class="hero-stats">
          <div class="hero-stat">
            <div class="hero-stat-value">2</div>
            <div class="hero-stat-label">Tracks</div>
          </div>
          <div class="hero-stat-divider"></div>
          <div class="hero-stat">
            <div class="hero-stat-value">IIT</div>
            <div class="hero-stat-label">Grand Finale Venue</div>
          </div>
          <div class="hero-stat-divider"></div>
          <div class="hero-stat">
            <div class="hero-stat-value">4</div>
            <div class="hero-stat-label">Competition Stages</div>
          </div>
          <div class="hero-stat-divider"></div>
          <div class="hero-stat">
            <div class="hero-stat-value">Free</div>
            <div class="hero-stat-label">To Participate</div>
          </div>
        </div>
      </div>

      <!-- Right: Countdown Card -->
      <div class="countdown-card" aria-label="Event countdown">
        <div class="countdown-label">Submission Round Opens In</div>
        <div class="countdown-grid">
          <div class="countdown-unit">
            <div class="countdown-number" id="days">15</div>
            <div class="countdown-unit-label">Days</div>
          </div>
          <div class="countdown-unit">
            <div class="countdown-number" id="hours">08</div>
            <div class="countdown-unit-label">Hours</div>
          </div>
          <div class="countdown-unit">
            <div class="countdown-number" id="minutes">34</div>
            <div class="countdown-unit-label">Mins</div>
          </div>
          <div class="countdown-unit">
            <div class="countdown-number" id="seconds">22</div>
            <div class="countdown-unit-label">Secs</div>
          </div>
        </div>
        <div class="event-meta">
          <div class="event-meta-row">
            <div class="event-meta-icon">📅</div>
            <span>Registration: <strong>Mar 14 – Apr 1, 2026</strong></span>
          </div>
          <div class="event-meta-row">
            <div class="event-meta-icon">📤</div>
            <span>Submission: <strong>Apr 2 – Apr 4, 2026</strong></span>
          </div>
          <div class="event-meta-row">
            <div class="event-meta-icon">🏛️</div>
            <span>Finale: <strong>IIT Delhi Campus</strong></span>
          </div>
          <div class="event-meta-row">
            <div class="event-meta-icon">🌐</div>
            <span>Mode: <strong>Online + Offline Finale</strong></span>
          </div>
        </div>
      </div>
    </div>

    <div class="scroll-indicator" aria-hidden="true">
      <span>Scroll</span>
      <div class="scroll-line"></div>
    </div>
  </section>

  <!-- ========================
       ORGANIZERS STRIP
  ========================= -->
  <div class="organizers-strip" aria-label="Organizers">
    <div class="organizers-inner">
      <span class="organizer-label">Organized by</span>
      <div class="org-divider"></div>
      <div class="org-badge">
        <div class="org-badge-icon">🔵</div>
        GDG IGDTUW
      </div>
      <div class="org-divider"></div>
      <div class="org-badge">
        <div class="org-badge-icon">🟣</div>
        GDG IIT Delhi
      </div>
      <div class="org-divider"></div>
      <div class="org-badge">
        <div class="org-badge-icon">🎓</div>
        Indian Institute of Technology, Delhi
      </div>
    </div>
  </div>

  <!-- ========================
       ABOUT SECTION
  ========================= -->
  <section class="section" id="about" aria-labelledby="about-title">
    <div class="container">
      <div class="about-grid">
        <!-- Visual side -->
        <div class="about-visual">
          <div class="about-main-card">
            <div class="about-icon-grid">
              <div class="about-icon-item">
                <div class="icon">💻</div>
                <div class="label">Hacking</div>
              </div>
              <div class="about-icon-item">
                <div class="icon">🤝</div>
                <div class="label">Collaboration</div>
              </div>
              <div class="about-icon-item">
                <div class="icon">🎓</div>
                <div class="label">Mentorship</div>
              </div>
              <div class="about-icon-item">
                <div class="icon">🏆</div>
                <div class="label">Recognition</div>
              </div>
            </div>
            <div style="background: rgba(255,255,255,0.03); border: 1px solid var(--border); border-radius: 12px; padding: 20px;">
              <div style="font-size: 12px; color: var(--text-muted); margin-bottom: 10px; text-transform: uppercase; letter-spacing: 1px;">Event Highlight</div>
              <div style="font-family: var(--font-heading); font-size: 20px; font-weight: 700; margin-bottom: 8px;">Grand Finale @ IIT Delhi</div>
              <div style="font-size: 14px; color: var(--text-secondary);">Top teams fly to IIT Delhi campus for a live pitch session in front of industry expert judges. 🚀</div>
            </div>
          </div>
          <div class="about-floating-tag about-floating-1">
            <div class="about-floating-dot"></div>
            Registration Open
          </div>
          <div class="about-floating-tag about-floating-2">
            <div class="about-floating-dot"></div>
            100% Free to Join
          </div>
        </div>

        <!-- Text side -->
        <div class="about-text">
          <span class="section-label">About the Event</span>
          <h2 class="section-title" id="about-title">
            Where Builders Come to <span class="gradient-text">Make an Impact</span>
          </h2>
          <p class="section-sub">
            Devcation Delhi 2026 is a flagship hackathon that brings together students from across India to build real-world solutions through intense collaboration, expert mentorship, and creative problem-solving.
          </p>

          <div class="feature-list">
            <div class="feature-item">
              <div class="feature-icon feature-icon--blue">🎯</div>
              <div class="feature-text">
                <h4>Multiple Thematic Tracks</h4>
                <p>Choose from Open Innovation to premium TigerGraph challenges with cash prizes up for grabs.</p>
              </div>
            </div>
            <div class="feature-item">
              <div class="feature-icon feature-icon--purple">🧠</div>
              <div class="feature-text">
                <h4>Expert Mentorship Sessions</h4>
                <p>Get 1:1 guidance from industry leaders and senior engineers to sharpen your project.</p>
              </div>
            </div>
            <div class="feature-item">
              <div class="feature-icon feature-icon--teal">🌐</div>
              <div class="feature-text">
                <h4>Talks & Workshops</h4>
                <p>Attend curated sessions on cutting-edge tech topics, from graph databases to AI/ML.</p>
              </div>
            </div>
            <div class="feature-item">
              <div class="feature-icon feature-icon--pink">🏛️</div>
              <div class="feature-text">
                <h4>Grand Finale @ IIT Delhi</h4>
                <p>Top teams compete on campus at one of India's most prestigious engineering institutions.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========================
       TIMELINE SECTION
  ========================= -->
  <section class="section" id="timeline" aria-labelledby="timeline-title" style="background: var(--bg-secondary);">
    <div class="container">
      <div class="timeline-header">
        <span class="section-label">Stages & Timeline</span>
        <h2 class="section-title" id="timeline-title">Your Journey to the <span class="gradient-text">Grand Finale</span></h2>
        <p class="section-sub">Four stages. One goal. Prove your skills and claim your spot at IIT Delhi.</p>
      </div>

      <div class="timeline" role="list">

        <!-- Stage 1 -->
        <div class="timeline-item" role="listitem">
          <div class="timeline-card">
            <div class="timeline-step">Stage 01</div>
            <h3 class="timeline-card-title">📋 Mandatory Registration</h3>
            <div class="timeline-date">📅 Mar 14 – Apr 1, 2026</div>
            <p>Lock in your spot by completing the mandatory registration form. Don't miss your chance to officially begin your Devcation journey. Teams must register to be eligible for any subsequent round.</p>
            <div style="margin-top: 16px;">
              <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary" target="_blank" rel="noopener" style="font-size: 13px; padding: 8px 16px;">
                Fill Registration Form →
              </a>
            </div>
          </div>
          <div class="timeline-node">
            <div class="timeline-dot">📋</div>
          </div>
          <div class="timeline-empty"></div>
        </div>

        <!-- Stage 2 -->
        <div class="timeline-item" role="listitem">
          <div class="timeline-empty"></div>
          <div class="timeline-node">
            <div class="timeline-dot timeline-dot--purple">📤</div>
          </div>
          <div class="timeline-card">
            <div class="timeline-step">Stage 02</div>
            <h3 class="timeline-card-title">📤 Hack 'N' Solve Submission</h3>
            <div class="timeline-date timeline-date--purple">📅 Apr 2 – Apr 4, 2026</div>
            <p>Submit your project via Google Form. Include a PPT covering your problem, solution & tech stack, a GitHub repository with code and documentation, and a deployed demo link.</p>
            <div style="margin-top: 14px; display: flex; gap: 8px; flex-wrap: wrap;">
              <span class="tag tag--purple">PPT Required</span>
              <span class="tag tag--blue">GitHub Link</span>
              <span class="tag tag--teal">Live Demo</span>
            </div>
          </div>
        </div>

        <!-- Stage 3 -->
        <div class="timeline-item" role="listitem">
          <div class="timeline-card">
            <div class="timeline-step">Stage 03</div>
            <h3 class="timeline-card-title">🧠 Mentorship Round</h3>
            <div class="timeline-date timeline-date--teal">📅 Apr 5 – Apr 7, 2026</div>
            <p>Shortlisted teams receive expert mentorship to refine and strengthen their projects. This is an eliminatory round — teams are evaluated on progress, implementation quality, and real-world viability.</p>
            <div style="margin-top: 14px;">
              <span class="tag tag--teal">Eliminatory Round</span>
            </div>
          </div>
          <div class="timeline-node">
            <div class="timeline-dot timeline-dot--teal">🧠</div>
          </div>
          <div class="timeline-empty"></div>
        </div>

        <!-- Stage 4 -->
        <div class="timeline-item" role="listitem">
          <div class="timeline-empty"></div>
          <div class="timeline-node">
            <div class="timeline-dot timeline-dot--pink">🏆</div>
          </div>
          <div class="timeline-card" style="border-color: rgba(255,107,157,0.25); background: linear-gradient(145deg, rgba(255,107,157,0.04), var(--bg-card));">
            <div class="timeline-step">Stage 04 — Grand Finale</div>
            <h3 class="timeline-card-title">🏆 Grand Finale @ IIT Delhi</h3>
            <div class="timeline-date timeline-date--pink">📅 Mar 15 – Mar 29, 2026</div>
            <p>The best teams make it to IIT Delhi to pitch their solutions live before industry judges. Impress, compete, and battle it out for top prizes at the Devcation Delhi 2026 Grand Finale. 🚀</p>
            <div style="margin-top: 14px; display: flex; gap: 8px; flex-wrap: wrap;">
              <span class="tag tag--pink">Live Pitch</span>
              <span class="tag tag--orange">Cash Prizes</span>
              <span class="tag" style="background: rgba(255,140,66,0.08); color: var(--accent-orange); border-color: rgba(255,140,66,0.2);">IIT Delhi Campus</span>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ========================
       TRACKS SECTION
  ========================= -->
  <section class="section" id="tracks" aria-labelledby="tracks-title">
    <div class="container">
      <div class="tracks-header">
        <span class="section-label">Competition Tracks</span>
        <h2 class="section-title" id="tracks-title">Choose Your <span class="gradient-text">Track</span></h2>
        <p class="section-sub" style="margin-bottom: 40px;">Two tracks, one mission — build something that makes a difference. Pick the challenge that excites you most.</p>
      </div>

      <div class="tracks-grid">

        <!-- Premium Track -->
        <div class="track-card track-card--premium">
          <div class="track-glow track-glow--purple"></div>
          <div class="track-badge-row">
            <div class="track-icon track-icon--purple">🐯</div>
            <span class="tag tag--purple">⭐ Premium Track</span>
          </div>
          <h3 class="track-title">TigerGraph Track</h3>
          <p class="track-subtitle">Build graph-powered solutions using TigerGraph MCP and related technologies. An open innovation track with premium cash prizes for the most impactful graph database applications.</p>
          <ul class="track-features">
            <li>Use TigerGraph MCP technology</li>
            <li>Open Innovation theme</li>
            <li>Exclusive cash prize pool</li>
            <li>Mentorship from TigerGraph experts</li>
          </ul>
          <div class="track-prize">💰 Cash Prizes</div>
          <div class="track-prize-label">Exclusive rewards for top-performing graph solutions</div>
          <div style="margin-top: 24px;">
            <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary" target="_blank" rel="noopener" style="width: 100%; justify-content: center;">
              Register for This Track →
            </a>
          </div>
        </div>

        <!-- Open Track -->
        <div class="track-card track-card--open">
          <div class="track-glow track-glow--blue"></div>
          <div class="track-badge-row">
            <div class="track-icon track-icon--blue">🛠️</div>
            <span class="tag">🔓 Open Track</span>
          </div>
          <h3 class="track-title">Hack 'N' Solve</h3>
          <p class="track-subtitle">An open-ended hackathon track where teams identify real-world problems and engineer creative, functional solutions using any technology of their choice. No constraints — just innovation.</p>
          <ul class="track-features">
            <li>Any tech stack, any domain</li>
            <li>Problem-solution focus</li>
            <li>Mentored project refinement</li>
            <li>Live IIT Delhi pitch opportunity</li>
          </ul>
          <div style="margin-top: auto; padding-top: 24px;">
            <div class="track-prize" style="color: var(--accent-blue);">🚀 Recognition</div>
            <div class="track-prize-label">Certificates, networking, and IIT Delhi finale experience</div>
          </div>
          <div style="margin-top: 24px;">
            <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary" target="_blank" rel="noopener" style="width: 100%; justify-content: center; background: linear-gradient(135deg, var(--accent-blue), #4a7fd4);">
              Register for This Track →
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ========================
       ELIGIBILITY SECTION
  ========================= -->
  <section class="section--sm" id="eligibility" aria-labelledby="eligibility-title" style="background: var(--bg-secondary);">
    <div class="container">
      <div class="eligibility-wrapper">
        <div class="eligibility-inner">
          <div>
            <span class="section-label">Who Can Apply</span>
            <h2 class="section-title" id="eligibility-title">Open to All <span class="gradient-text">Students</span></h2>
            <p class="section-sub" style="font-size: 15px;">Whether you're an engineering undergrad or a science postgrad — Devcation welcomes builders from all backgrounds.</p>
            <div class="eligibility-tags">
              <div class="eligibility-tag"><div class="dot"></div> Engineering Students</div>
              <div class="eligibility-tag"><div class="dot"></div> Postgraduate</div>
              <div class="eligibility-tag"><div class="dot"></div> Undergraduate</div>
              <div class="eligibility-tag" style="--accent-teal: #6EE7B7;"><div class="dot"></div> Arts & Commerce</div>
              <div class="eligibility-tag"><div class="dot"></div> Sciences & Others</div>
            </div>
          </div>

          <div class="checklist">
            <div class="check-item">
              <div class="check-icon">✓</div>
              <span><strong>Team size:</strong> Form a team (size details on registration form)</span>
            </div>
            <div class="check-item">
              <div class="check-icon">✓</div>
              <span><strong>Student status:</strong> Must be an enrolled student at any institution</span>
            </div>
            <div class="check-item">
              <div class="check-icon">✓</div>
              <span><strong>Experience level:</strong> Beginners to advanced — all are welcome</span>
            </div>
            <div class="check-item">
              <div class="check-icon">✓</div>
              <span><strong>Submission:</strong> PPT + GitHub repo + Live demo link required</span>
            </div>
            <div class="check-item">
              <div class="check-icon">✓</div>
              <span><strong>Cost:</strong> Completely free to register and participate</span>
            </div>
            <div style="margin-top: 20px;">
              <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary" target="_blank" rel="noopener">
                Check Full Eligibility →
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========================
       FAQ SECTION
  ========================= -->
  <section class="section" id="faq" aria-labelledby="faq-title">
    <div class="container">
      <div class="faq-header">
        <span class="section-label">FAQ</span>
        <h2 class="section-title" id="faq-title">Frequently Asked <span class="gradient-text">Questions</span></h2>
        <p class="section-sub" style="margin: 0 auto; text-align: center;">Everything you need to know before diving in.</p>
      </div>

      <div class="faq-grid" role="list">
        <div class="faq-item open" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="true">
            What is Devcation Hack 'N' Solve?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            Devcation Hack 'N' Solve is a flagship hackathon organized by Google Developer Groups IGDTUW in collaboration with GDG IIT Delhi. It brings together developers, innovators, and students to build impactful technology solutions through coding, collaboration, and mentorship — culminating in a Grand Finale at IIT Delhi.
          </div>
        </div>

        <div class="faq-item" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="false">
            Is it free to participate?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            Yes! Participation is completely free for all stages. Simply complete the mandatory registration form to begin your journey.
          </div>
        </div>

        <div class="faq-item" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="false">
            What do I need to submit for the Hack 'N' Solve round?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            Your submission must include: (1) A PPT explaining your problem statement, solution, key features, and tech stack; (2) A GitHub repository with your project code and basic documentation; (3) A deployed demo link showing your working solution. All three fields are mandatory.
          </div>
        </div>

        <div class="faq-item" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="false">
            What is the TigerGraph Premium Track?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            The TigerGraph Track is an open innovation challenge where participants build solutions using TigerGraph MCP and related technologies. Top performers in this track compete for exclusive cash prizes on top of the regular hackathon prizes.
          </div>
        </div>

        <div class="faq-item" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="false">
            Who is eligible to participate?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            The hackathon is open to Engineering Students, Postgraduate, Undergraduate students, and Arts/Commerce/Sciences students from any institution. Beginners and experienced developers are both welcome!
          </div>
        </div>

        <div class="faq-item" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="false">
            What happens in the Mentorship Round?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            Shortlisted teams from the Submission Round receive personalized mentorship from domain experts to help refine and improve their projects. This is an eliminatory round — teams are evaluated on their progress, quality of implementation, and ability to advance to the Grand Finale.
          </div>
        </div>

        <div class="faq-item" role="listitem">
          <button class="faq-question" onclick="toggleFaq(this)" aria-expanded="false">
            How will teams be selected for the Grand Finale?
            <div class="faq-arrow">▼</div>
          </button>
          <div class="faq-answer">
            Teams will be evaluated on the quality of their submission (PPT, code, demo), then shortlisted for the Mentorship Round. After the mentorship round evaluation, the best-performing teams will be invited to the IIT Delhi campus for the Grand Finale live pitch.
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========================
       DESIGN SYSTEM PREVIEW
  ========================= -->
  <section class="design-section" aria-labelledby="design-title">
    <div class="container">
      <div style="margin-bottom: 40px;">
        <span class="section-label">Design System</span>
        <h2 class="section-title" id="design-title" style="font-size: 28px;">Color Palette, Typography & Components</h2>
        <p class="section-sub" style="font-size: 15px;">A cohesive visual language crafted for the modern UG tech audience.</p>
      </div>
      <div class="design-grid">

        <!-- Colors -->
        <div class="design-card">
          <h4>Color Palette</h4>
          <div class="color-swatches">
            <div class="color-swatch">
              <div class="swatch" style="background: #5B8DEF;"></div>
              <div class="swatch-info">
                <div class="swatch-name">Electric Blue</div>
                <div class="swatch-hex">#5B8DEF — Primary CTA</div>
              </div>
            </div>
            <div class="color-swatch">
              <div class="swatch" style="background: #9B6DFF;"></div>
              <div class="swatch-info">
                <div class="swatch-name">Vivid Purple</div>
                <div class="swatch-hex">#9B6DFF — Gradients, Accents</div>
              </div>
            </div>
            <div class="color-swatch">
              <div class="swatch" style="background: #00D4AA;"></div>
              <div class="swatch-info">
                <div class="swatch-name">Neon Teal</div>
                <div class="swatch-hex">#00D4AA — Live Status, Icons</div>
              </div>
            </div>
            <div class="color-swatch">
              <div class="swatch" style="background: #FF6B9D;"></div>
              <div class="swatch-info">
                <div class="swatch-name">Coral Pink</div>
                <div class="swatch-hex">#FF6B9D — Finale Highlight</div>
              </div>
            </div>
            <div class="color-swatch">
              <div class="swatch" style="background: #06070F; border: 1px solid #333;"></div>
              <div class="swatch-info">
                <div class="swatch-name">Deep Void</div>
                <div class="swatch-hex">#06070F — Background</div>
              </div>
            </div>
          </div>
        </div>

        <!-- Typography -->
        <div class="design-card">
          <h4>Typography</h4>
          <div class="type-sample">
            <div class="type-item">
              <div class="type-label">H1 — Space Grotesk 800</div>
              <div class="type-preview-h1 gradient-text">Hack 'N' Solve</div>
            </div>
            <div class="type-item">
              <div class="type-label">H2 — Space Grotesk 700</div>
              <div class="type-preview-h2">Grand Finale @ IIT Delhi</div>
            </div>
            <div class="type-item">
              <div class="type-label">H3 — Space Grotesk 600</div>
              <div class="type-preview-h3">Mentorship Round Opens Apr 5</div>
            </div>
            <div class="type-item">
              <div class="type-label">Body — Inter 400</div>
              <div class="type-preview-body">Build impactful solutions with collaboration, code, and creativity. Devcation 2026 welcomes all student builders.</div>
            </div>
          </div>
        </div>

        <!-- Components -->
        <div class="design-card">
          <h4>UI Components</h4>
          <div class="component-samples">
            <div class="component-row">
              <a href="#" class="btn-primary" onclick="return false;">Primary CTA</a>
              <a href="#" class="btn-outline" onclick="return false;" style="padding: 9px 20px; font-size: 14px;">Secondary</a>
            </div>
            <div class="component-row">
              <span class="tag">🔵 Online</span>
              <span class="tag tag--teal">✅ Open</span>
              <span class="tag tag--purple">⭐ Premium</span>
            </div>
            <div class="component-row">
              <div style="display: flex; align-items: center; gap: 8px; font-size: 13px; color: var(--text-secondary);">
                <div class="hero-badge-dot"></div>
                <span style="color: var(--accent-teal);">Live Status Indicator</span>
              </div>
            </div>
            <div style="background: rgba(255,255,255,0.04); border: 1px solid var(--border); border-radius: 10px; padding: 14px 16px;">
              <div style="font-size: 12px; color: var(--text-muted); margin-bottom: 6px;">CARD PATTERN</div>
              <div style="font-size: 14px; font-weight: 600;">Dark glass cards with subtle borders + hover glow effects for depth and interactivity.</div>
            </div>
            <div style="font-size: 13px; color: var(--text-muted); line-height: 1.6;">
              <strong style="color: var(--text-secondary);">Spacing system:</strong> 4/8/12/16/24/32/48/64/96px scale. Border radius: 8/16/24/32px.
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ========================
       CTA SECTION
  ========================= -->
  <section class="section--sm" aria-label="Call to action">
    <div class="cta-section">
      <div class="cta-orb-1"></div>
      <div class="cta-orb-2"></div>
      <div class="cta-content">
        <span class="tag tag--teal" style="margin-bottom: 20px;">🚀 Registration Closing Soon</span>
        <h2 class="cta-title">
          Ready to <span class="gradient-text">Build Something</span> Incredible?
        </h2>
        <p class="cta-desc">
          Join hundreds of student innovators at Devcation Delhi 2026. Bring your ideas, your team, and your passion for technology — we'll handle the rest.
        </p>
        <div class="cta-actions">
          <a href="https://forms.gle/nNuA4GM5tf2JSUW89" class="btn-primary btn-primary--lg" target="_blank" rel="noopener">
            🚀 Register Now — It's Free
          </a>
          <a href="#timeline" class="btn-outline">
            See Full Timeline
          </a>
        </div>
        <p class="deadline-note">⏰ Registration deadline: April 1, 2026 · Grand Finale: IIT Delhi</p>
      </div>
    </div>
  </section>

  <!-- ========================
       FOOTER
  ========================= -->
  <footer class="footer" role="contentinfo">
    <div class="footer-inner">
      <div class="footer-brand">
        <a href="#" class="nav-logo" style="margin-bottom: 8px; display: inline-flex;">
          <div class="nav-logo-icon">D</div>
          Devcation
        </a>
        <p>A flagship hackathon by GDG IGDTUW × GDG IIT Delhi. Building the future, one hack at a time.</p>
      </div>
      <div class="footer-col">
        <h4>Event</h4>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#timeline">Timeline</a></li>
          <li><a href="#tracks">Tracks</a></li>
          <li><a href="#eligibility">Eligibility</a></li>
          <li><a href="#faq">FAQ</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <h4>Quick Links</h4>
        <ul>
          <li><a href="https://forms.gle/nNuA4GM5tf2JSUW89" target="_blank" rel="noopener">Register Now</a></li>
          <li><a href="https://unstop.com/hackathons/devcation-hack-n-solve-iit-delhi-1659241" target="_blank" rel="noopener">Unstop Page</a></li>
          <li><a href="#" target="_blank" rel="noopener">GDG IGDTUW</a></li>
          <li><a href="#" target="_blank" rel="noopener">GDG IIT Delhi</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <p>© 2026 Devcation Hack 'N' Solve — IIT Delhi. Listed on Unstop.</p>
      <p style="color: var(--text-muted);">Redesigned concept · GDG IGDTUW × GDG IIT Delhi</p>
    </div>
  </footer>

  <!-- ========================
       JAVASCRIPT
  ========================= -->
  <script>
    // Mobile menu toggle
    function toggleMenu() {
      const menu = document.getElementById('mobileMenu');
      const btn = document.querySelector('.hamburger');
      menu.classList.toggle('open');
      btn.setAttribute('aria-expanded', menu.classList.contains('open'));
    }
    function closeMenu() {
      document.getElementById('mobileMenu').classList.remove('open');
    }

    // FAQ toggle
    function toggleFaq(btn) {
      const item = btn.parentElement;
      const isOpen = item.classList.contains('open');
      document.querySelectorAll('.faq-item').forEach(i => i.classList.remove('open'));
      document.querySelectorAll('.faq-question').forEach(b => b.setAttribute('aria-expanded', 'false'));
      if (!isOpen) {
        item.classList.add('open');
        btn.setAttribute('aria-expanded', 'true');
      }
    }

    // Countdown timer to Apr 2, 2026 06:30 PM CUT
    function updateCountdown() {
      const target = new Date('2026-04-02T18:30:00Z');
      const now = new Date();
      const diff = target - now;
      if (diff <= 0) {
        document.getElementById('days').textContent = '00';
        document.getElementById('hours').textContent = '00';
        document.getElementById('minutes').textContent = '00';
        document.getElementById('seconds').textContent = '00';
        return;
      }
      const d = Math.floor(diff / 86400000);
      const h = Math.floor((diff % 86400000) / 3600000);
      const m = Math.floor((diff % 3600000) / 60000);
      const s = Math.floor((diff % 60000) / 1000);
      document.getElementById('days').textContent    = String(d).padStart(2,'0');
      document.getElementById('hours').textContent   = String(h).padStart(2,'0');
      document.getElementById('minutes').textContent = String(m).padStart(2,'0');
      document.getElementById('seconds').textContent = String(s).padStart(2,'0');
    }
    updateCountdown();
    setInterval(updateCountdown, 1000);

    // Generate floating particles
    const particlesContainer = document.getElementById('particles');
    for (let i = 0; i < 24; i++) {
      const p = document.createElement('div');
      p.className = 'particle';
      p.style.cssText = `
        left: ${Math.random()*100}%;
        top: ${Math.random()*100}%;
        width: ${Math.random() > 0.7 ? 3 : 2}px;
        height: ${Math.random() > 0.7 ? 3 : 2}px;
        --drift: ${(Math.random()-0.5)*80}px;
        animation-duration: ${8 + Math.random()*12}s;
        animation-delay: ${-Math.random()*20}s;
        opacity: ${0.15 + Math.random()*0.3};
      `;
      particlesContainer.appendChild(p);
    }

    // Smooth scroll & active nav
    document.querySelectorAll('a[href^="#"]').forEach(a => {
      a.addEventListener('click', e => {
        const id = a.getAttribute('href');
        if (id === '#') return;
        e.preventDefault();
        const el = document.querySelector(id);
        if (el) el.scrollIntoView({ behavior: 'smooth', block: 'start' });
      });
    });

    // Intersection Observer for subtle entrance animations
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = '1';
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });

    document.querySelectorAll('.timeline-card, .track-card, .about-main-card, .design-card').forEach(el => {
      el.style.opacity = '0';
      el.style.transform = 'translateY(24px)';
      el.style.transition += ', opacity 0.6s ease, transform 0.6s ease';
      observer.observe(el);
    });
  </script>
</body>
</html>
