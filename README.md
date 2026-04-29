---
layout: default
title: "Project Dynamica | AI-Driven Quant & Fintech"
description: "Algorithmic trading, MQL5 EAs, sentiment analysis, and fintech automation built by Thabang Makgari."
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Project Dynamica — Quant Systems • AI • Fintech Automation</title>
    <!-- Font Awesome Icons (v6) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Google Fonts: modern sans -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', sans-serif;
            background: #f8fafd;
            color: #0a1c2f;
            line-height: 1.5;
            scroll-behavior: smooth;
        }
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 24px;
        }
        /* Buttons & links */
        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 12px 28px;
            border-radius: 40px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.2s ease;
            background: white;
            color: #0f2b3d;
            border: 1px solid #cfdfed;
        }
        .btn-primary {
            background: #0a2b3e;
            border: none;
            color: white;
            box-shadow: 0 8px 18px rgba(0,20,40,0.12);
        }
        .btn-primary:hover {
            background: #134b66;
            transform: translateY(-2px);
            box-shadow: 0 14px 24px rgba(0,0,0,0.08);
        }
        .btn-outline {
            border: 1px solid #0a2b3e;
            background: transparent;
            color: #0a2b3e;
        }
        .btn-outline:hover {
            background: #eef3fc;
            transform: translateY(-2px);
        }
        .badge {
            background: #e9eff5;
            padding: 6px 14px;
            border-radius: 60px;
            font-size: 0.8rem;
            font-weight: 500;
            display: inline-block;
        }
        /* Hero */
        .hero {
            padding: 60px 0 40px;
            border-bottom: 1px solid #e2edf5;
        }
        .hero h1 {
            font-size: 3.2rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            background: linear-gradient(135deg, #082433, #1f5e7e);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 20px;
        }
        .highlight {
            color: #136b8f;
        }
        /* Section titles */
        .section-title {
            font-size: 2rem;
            font-weight: 700;
            margin: 56px 0 32px 0;
            border-left: 5px solid #1f6e8c;
            padding-left: 20px;
        }
        /* Product grid */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 28px;
            margin: 30px 0;
        }
        .product-card {
            background: white;
            border-radius: 28px;
            padding: 28px 24px;
            box-shadow: 0 8px 22px rgba(0, 0, 0, 0.03), 0 2px 4px rgba(0,0,0,0.02);
            transition: all 0.25s;
            border: 1px solid #e7f0f5;
        }
        .product-card:hover {
            transform: translateY(-6px);
            border-color: #bfdeee;
            box-shadow: 0 24px 40px -16px rgba(20,70,100,0.2);
        }
        .product-icon {
            font-size: 2.2rem;
            color: #1f6e8c;
            margin-bottom: 18px;
        }
        .product-card h3 {
            font-size: 1.6rem;
            font-weight: 700;
            margin-bottom: 12px;
        }
        .product-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 18px 0;
        }
        .product-tag {
            background: #eff5f9;
            font-size: 0.7rem;
            padding: 4px 12px;
            border-radius: 50px;
            font-weight: 500;
        }
        .request-link {
            margin-top: 20px;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            font-weight: 600;
            color: #1f6e8c;
            text-decoration: none;
            border-bottom: 1.5px solid #bddcec;
        }
        .request-link i {
            font-size: 0.8rem;
            transition: transform 0.2s;
        }
        .request-link:hover i {
            transform: translateX(4px);
        }
        .contact-block {
            background: #eef4fa;
            border-radius: 40px;
            padding: 48px 32px;
            margin: 60px 0;
            text-align: center;
            border: 1px solid #d4e3ef;
        }
        .contact-details {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 40px;
            margin: 30px 0 20px;
        }
        .contact-item {
            background: white;
            padding: 14px 28px;
            border-radius: 70px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.03);
            display: inline-flex;
            align-items: center;
            gap: 14px;
            font-weight: 600;
            font-size: 1.2rem;
        }
        .contact-item a {
            text-decoration: none;
            color: #0a3b4f;
        }
        footer {
            text-align: center;
            padding: 40px 0 32px;
            border-top: 1px solid #deeaf1;
            font-size: 0.85rem;
            color: #3f6479;
        }
        @media (max-width: 700px) {
            .hero h1 { font-size: 2.2rem; }
            .section-title { font-size: 1.8rem; }
            .contact-item { font-size: 1rem; padding: 10px 20px; }
        }
        .disclaimer {
            background: #fcf4e8;
            border-radius: 18px;
            padding: 14px 20px;
            font-size: 0.75rem;
            margin-top: 40px;
            color: #6e4f1e;
        }
    </style>
</head>
<body>

<div class="container">
    
    <!-- Hero Section -->
    <div class="hero">
        <span class="badge"><i class="fas fa-chart-line"></i>  Built & shipped · South Africa</span>
        <h1>Engineer the markets.<br> Automate the edge.</h1>
        <p style="font-size: 1.25rem; max-width: 720px; margin: 20px 0 28px;">Quantitative trading bots, MQL5 EAs, AI sentiment engines, and fintech infrastructure — <strong>Project Dynamica</strong> delivers production-ready systems for traders, funds, and innovators.</p>
        <div style="display: flex; gap: 18px; flex-wrap: wrap;">
            <a href="#products" class="btn btn-primary"><i class="fas fa-robot"></i> Explore solutions</a>
            <a href="#contact" class="btn btn-outline"><i class="fas fa-paper-plane"></i> Contact founder</a>
        </div>
    </div>

    <!-- Products & Core Offerings -->
    <div id="products"></div>
    <div class="section-title">
        <i class="fas fa-cubes" style="margin-right: 12px;"></i> commercial products & platforms
    </div>
    <div class="product-grid">
        
        <!-- Dynamica Trader -->
        <div class="product-card">
            <div class="product-icon"><i class="fas fa-chart-simple"></i></div>
            <h3>Dynamica Trader</h3>
            <p>Python-powered Binance bot fusing Fibonacci retracements, CLT z‑score analysis, chaos volatility filters & Soros reflexivity loops.</p>
            <div class="product-tags"><span class="product-tag">Python</span><span class="product-tag">Binance API</span><span class="product-tag">Quant alpha</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=Dynamica%20Trader%20inquiry&body=Hi%20Thabang,%20I'm%20interested%20in%20licensing%20Dynamica%20Trader." class="request-link">Request pricing / demo <i class="fas fa-arrow-right"></i></a>
        </div>
        
        <!-- Dynamica EA (MQL5) -->
        <div class="product-card">
            <div class="product-icon"><i class="fas fa-chart-line"></i></div>
            <h3>Dynamica_EA.mq5</h3>
            <p>MetaTrader 5 Expert Advisor for forex/CFD automation. Implements quantitative signal logic, risk-aware execution, real-time filtering.</p>
            <div class="product-tags"><span class="product-tag">MQL5</span><span class="product-tag">MT5</span><span class="product-tag">Forex algo</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=MT5%20EA%20inquiry&body=Tell%20me%20more%20about%20Dynamica_EA%20licensing%20and%20backtests." class="request-link">Get EA access <i class="fas fa-arrow-right"></i></a>
        </div>

        <!-- Sentiment analysis system -->
        <div class="product-card">
            <div class="product-icon"><i class="fab fa-facebook"></i></div>
            <h3>Social Sentiment Engine</h3>
            <p>Real-time Facebook/Grammar signal extraction with TextBlob + Graph API. Detects market-moving narratives for alpha generation.</p>
            <div class="product-tags"><span class="product-tag">NLP</span><span class="product-tag">API-first</span><span class="product-tag">Alternative data</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=Sentiment%20system%20integration&body=I%20need%20social%20sentiment%20for%20trading%20or%20risk." class="request-link">Schedule integration <i class="fas fa-arrow-right"></i></a>
        </div>

        <!-- Workflow Builder -->
        <div class="product-card">
            <div class="product-icon"><i class="fas fa-diagram-project"></i></div>
            <h3>Workflow Builder</h3>
            <p>Cross-platform automation: Google Workspace, GitHub, Calendar via Python SDKs. Eliminate repetitive ops, unify business logic.</p>
            <div class="product-tags"><span class="product-tag">Automation</span><span class="product-tag">SaaS tooling</span><span class="product-tag">Low-code ready</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=Workflow%20automation%20project&body=Describe%20your%20company%20workflows%20to%20automate." class="request-link">Book consultancy <i class="fas fa-arrow-right"></i></a>
        </div>

        <!-- USSD Fintech Simulator -->
        <div class="product-card">
            <div class="product-icon"><i class="fas fa-mobile-alt"></i></div>
            <h3>USSD Fintech Simulator</h3>
            <p>Interactive financial inclusion prototype with PIN-only logic, designed for Panacea Mobile / Africa's Talking. Instant deployment ready.</p>
            <div class="product-tags"><span class="product-tag">Telecom</span><span class="product-tag">Financial inclusion</span><span class="product-tag">API integration</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=USSD%20fintech%20simulator&body=We%20need%20a%20low-barrier%20USSD%20banking%20simulation." class="request-link">Demo simulator <i class="fas fa-arrow-right"></i></a>
        </div>

        <!-- WorldQuant BRAIN + Backtester -->
        <div class="product-card">
            <div class="product-icon"><i class="fas fa-brain"></i></div>
            <h3>BRAIN Alpha + Visualizer</h3>
            <p>WorldQuant-style alpha strategy (Fibonacci + CLT + normal distributions) paired with React backtesting dashboard. Institutional signal research.</p>
            <div class="product-tags"><span class="product-tag">React.js</span><span class="product-tag">Quant research</span><span class="product-tag">Backtesting</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=WorldQuant%20alpha%20licensing&body=Interested%20in%20alpha%20strategy%20or%20visualizer%20integration." class="request-link">Request alpha access <i class="fas fa-arrow-right"></i></a>
        </div>
        
        <!-- Custom LSTM / ML -->
        <div class="product-card">
            <div class="product-icon"><i class="fas fa-network-wired"></i></div>
            <h3>LSTM Stock Predictor</h3>
            <p>Deep learning pipeline for market forecasting — data preprocessing, LSTM architecture, performance evaluation. White-label forecasting modules.</p>
            <div class="product-tags"><span class="product-tag">TensorFlow</span><span class="product-tag">Time series</span><span class="product-tag">Predictive AI</span></div>
            <a href="mailto:datathabang1@gmail.com?subject=LSTM%20forecasting%20model&body=I'd%20like%20to%20integrate%20AI%20predictions%20into%20my%20trading%20stack." class="request-link">Consult AI team <i class="fas fa-arrow-right"></i></a>
        </div>
    </div>

    <!-- Additional creds & highlight -->
    <div style="background: #ffffff; border-radius: 28px; padding: 24px 30px; margin: 30px 0; border: 1px solid #e0edf5;">
        <div style="display: flex; flex-wrap: wrap; justify-content: space-between; gap: 20px; align-items: center;">
            <div><i class="fas fa-check-circle" style="color:#1f6e8c;"></i> <strong>📈 WorldQuant BRAIN strategy</strong> – live-tested framework</div>
            <div><i class="fas fa-check-circle" style="color:#1f6e8c;"></i> <strong>🧠 AI 24 novel</strong> – philosophy of AI & surveillance</div>
            <div><i class="fas fa-check-circle" style="color:#1f6e8c;"></i> <strong>🔐 IBM Cybersecurity + GenAI certified</strong> (2026)</div>
        </div>
    </div>

    <!-- Founder & Engineering ethos -->
    <div class="section-title">
        <i class="fas fa-microchip"></i> from the founder — thabang makgari
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 30px; background: #fefefe; border-radius: 28px; padding: 28px 32px; border: 1px solid #e0ecf3;">
        <div style="flex: 1.5;">
            <p style="font-weight: 500; font-size: 1.1rem;">“I build systems that merge statistical rigor (CLT, chaos filters, reflexivity) with production engineering. No fluff — just quant logic that ships.”</p>
            <p style="margin-top: 16px;">🔹 BSc Data Science (Sol Plaatje) · Philosophy & Applied Statistics (UCT)<br>
            🔹 Self-directed builder: Python, MQL5, R, C++ · ML pipelines · React dashboards.<br>
            🔹 Immediate availability for high-trust collaborations, alpha research, or custom fintech infrastructure.</p>
            <div style="margin-top: 24px;">
                <a href="#contact" class="btn btn-outline" style="gap: 8px;"><i class="fas fa-bolt"></i> Partner with Dynamica</a>
            </div>
        </div>
        <div style="flex: 0.8; background: #eaf3f9; border-radius: 24px; padding: 20px; text-align: center;">
            <i class="fas fa-certificate" style="font-size: 2rem; color: #1f6e8c;"></i>
            <p style="margin-top: 8px;"><strong>Latest credentials</strong><br>IBM Generative AI Essentials · Cybersecurity Fundamentals · Google Data Analytics</p>
        </div>
    </div>
    
    <!-- Contact block with phone & email -->
    <div id="contact"></div>
    <div class="contact-block">
        <i class="fas fa-handshake" style="font-size: 2.6rem; color: #115e7c;"></i>
        <h2 style="font-size: 2rem; margin: 12px 0;">Ready to deploy quant power?</h2>
        <p style="max-width: 580px; margin: 0 auto 20px;">Product licensing, custom EA development, fintech automation, or AI integration — direct line to the founder.</p>
        <div class="contact-details">
            <div class="contact-item">
                <i class="fas fa-phone-alt"></i>
                <a href="tel:+27603153191">060 315 3191</a>
            </div>
            <div class="contact-item">
                <i class="fas fa-envelope"></i>
                <a href="mailto:datathabang1@gmail.com">datathabang1@gmail.com</a>
            </div>
        </div>
        <div style="margin-top: 12px;">
            <p><i class="fas fa-globe"></i> South Africa · Remote worldwide · open to relocation for strategic roles</p>
            <p style="font-size: 0.85rem; opacity: 0.7;">response within 4 hours | signal / whatsapp available</p>
        </div>
    </div>

    <!-- Disclaimer & footer -->
    <div class="disclaimer">
        ⚠️ <strong>Risk disclosure:</strong> Quantitative trading systems, EAs and predictive models involve substantial risk of loss. Past simulated performance does not guarantee future results. Project Dynamica provides tooling and research — all live trading decisions remain your responsibility.
    </div>
    <footer>
        <p>© 2026 Project Dynamica — founded by Thabang Makgari. Built with <i class="fas fa-code"></i> for quant finance & AI-first systems.</p>
        <p style="margin-top: 10px;"><i class="fab fa-github"></i> Hosted on GitHub Pages · version 1.0</p>
    </footer>
</div>

<!-- simple analytics / dynamic contact copy (optional but adds dynamic behaviour) -->
<script>
    // Optional: add a small dynamic element for interaction
    const contactNumbers = document.querySelectorAll('.contact-item a[href^="tel:"]');
    if(contactNumbers.length) {
        console.log("Project Dynamica — contact ready");
    }
    // simple highlight for product inquiry links
    const allRequestLinks = document.querySelectorAll('.request-link');
    allRequestLinks.forEach(link => {
        link.addEventListener('click', function(e) {
            // just to show dynamic feedback (no spam)
            console.log('Initiating product inquiry: ' + this.innerText);
        });
    });
</script>
</body>
</html>
