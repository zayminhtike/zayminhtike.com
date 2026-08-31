<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zay Min Htike | Personal Portfolio</title>
    <style>
        :root {
            --primary: #0f172a;
            --accent: #0284c7;
            --accent-hover: #0369a1;
            --bg-light: #f8fafc;
            --card-bg: #ffffff;
            --text-dark: #1e293b;
            --text-muted: #64748b;
            --border: #e2e8f0;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            position: sticky;
            top: 0;
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(5px);
            border-bottom: 1px solid var(--border);
            z-index: 1000;
        }

        .nav-container {
            max-width: 1100px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-weight: 700;
            font-size: 1.25rem;
            color: var(--primary);
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            gap: 1.5rem;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-muted);
            font-weight: 500;
            transition: color 0.2s;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        /* Layout Container */
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* Hero Section */
        .hero {
            padding: 4rem 0 3rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 2.75rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .hero p.subtitle {
            font-size: 1.25rem;
            color: var(--accent);
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .hero p.location {
            color: var(--text-muted);
            margin-bottom: 1.5rem;
        }

        .btn-group {
            display: flex;
            justify-content: center;
            gap: 1rem;
        }

        .btn {
            display: inline-block;
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.2s;
        }

        .btn-primary {
            background-color: var(--accent);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--accent-hover);
        }

        .btn-secondary {
            background-color: #e0f2fe;
            color: var(--accent);
        }

        .btn-secondary:hover {
            background-color: #bae6fd;
        }

        /* Impact Highlights Grid */
        .metrics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0 4rem 0;
        }

        .metric-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border);
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }

        .metric-card .number {
            font-size: 2rem;
            font-weight: 700;
            color: var(--accent);
        }

        .metric-card .label {
            color: var(--text-muted);
            font-size: 0.9rem;
            margin-top: 0.25rem;
        }

        /* Main Sections */
        section {
            margin-bottom: 4rem;
        }

        .section-title {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            border-bottom: 2px solid var(--border);
            padding-bottom: 0.5rem;
        }

        .card {
            background-color: var(--card-bg);
            border: 1px solid var(--border);
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            box-shadow: 0 1px 3px rgba(0,0,0,0.02);
        }

        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            flex-wrap: wrap;
            margin-bottom: 0.5rem;
        }

        .card-title {
            font-size: 1.15rem;
            font-weight: 700;
            color: var(--primary);
        }

        .card-subtitle {
            font-weight: 600;
            color: var(--accent);
            margin-bottom: 0.75rem;
        }

        .card-meta {
            font-size: 0.875rem;
            color: var(--text-muted);
        }

        ul.bullets {
            padding-left: 1.2rem;
        }

        ul.bullets li {
            margin-bottom: 0.5rem;
        }

        /* Skills Badges */
        .skills-group {
            margin-bottom: 1.5rem;
        }

        .skills-group h3 {
            font-size: 1rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .badge {
            background-color: #f1f5f9;
            color: var(--text-dark);
            padding: 0.35rem 0.75rem;
            border-radius: 20px;
            font-size: 0.875rem;
            border: 1px solid var(--border);
            font-weight: 500;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-muted);
            border-top: 1px solid var(--border);
            font-size: 0.9rem;
        }

        @media (max-width: 600px) {
            .hero h1 { font-size: 2rem; }
            .card-header { flex-direction: column; }
            .nav-links { display: none; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="nav-container">
            <a href="#" class="logo">Zay Min Htike</a>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#leadership">Leadership</a></li>
                <li><a href="#skills">Skills</a></li>
            </ul>
        </div>
    </nav>

    <div class="container">

        <header class="hero" id="about">
            <h1>Zay Min Htike</h1>
            <p class="subtitle">Finance & Business Analytics Student</p>
            <p class="location">Dayton, OH &bull; University of Dayton</p>
            <div class="btn-group">
                <a href="mailto:htikez1@udayton.edu" class="btn btn-primary">Email Me</a>
                <a href="https://www.linkedin.com/in/zay-min-htike" target="_blank" class="btn btn-secondary">LinkedIn</a>
            </div>
        </header>

        <div class="metrics-grid">
            <div class="metric-card">
                <div class="number">3.94</div>
                <div class="label">Cumulative GPA</div>
            </div>
            <div class="metric-card">
                <div class="number">$58,392</div>
                <div class="label">Annual Energy Savings Identified</div>
            </div>
            <div class="metric-card">
                <div class="number">$83,000</div>
                <div class="label">Projected Reusable Container Savings</div>
            </div>
            <div class="metric-card">
                <div class="number">1,500 lbs</div>
                <div class="label">Textiles Diverted from Landfill</div>
            </div>
        </div>

        <section id="education">
            <h2 class="section-title">Education</h2>
            <div class="card">
                <div class="card-header">
                    <div>
                        <div class="card-title">University of Dayton</div>
                        <div class="card-subtitle">Bachelor of Science in Business Administration - Finance & Business Analytics</div>
                    </div>
                    <div class="card-meta">Graduation: May 2027 | Dayton, OH</div>
                </div>
                <ul class="bullets">
                    <li><strong>GPA:</strong> 3.94 / 4.00</li>
                    <li><strong>Scholarships:</strong> UDayton Global Academic Excellence Scholarship, Talbot-Duffy Scholarship</li>
                    <li><strong>Honors:</strong> Dean's List (6/6 semesters), University Honors Program, Beta Gamma Sigma</li>
                </ul>
            </div>
        </section>

        <section id="experience">
            <h2 class="section-title">Professional Experience</h2>

            <div class="card">
                <div class="card-header">
                    <div>
                        <div class="card-title">City of Dayton's Office of Sustainability</div>
                        <div class="card-subtitle">Energy Analyst Intern</div>
                    </div>
                    <div class="card-meta">May 2026 – Aug 2026</div>
                </div>
                <ul class="bullets">
                    <li>Developed 4 programming models in RStudio featuring forecasting and peak-detection algorithms to accurately identify summer peak load days, informing strategic load-shedding decisions and supporting measurable annual cost savings of $58,392.</li>
                    <li>Analyzed historical hedging performance using Excel financial modeling to identify budget implications and provide actionable recommendations to optimize future energy procurement strategy and mitigate risk.</li>
                    <li>Processed, validated, and organized emissions data from 15 municipal sources to establish reliable baseline KPIs that inform the City's 10-year sustainability planning and targeted emissions-reduction initiatives.</li>
                </ul>
            </div>

            <div class="card">
                <div class="card-header">
                    <div>
                        <div class="card-title">Hanley Sustainability Institute</div>
                        <div class="card-subtitle">Student Director of Communication and Outreach</div>
                    </div>
                    <div class="card-meta">Aug 2025 – Present</div>
                </div>
                <ul class="bullets">
                    <li>Launch and manage the institute's podcast platform, overseeing content strategy, production, and distribution to translate complex sustainability research into clear, accessible public education.</li>
                    <li>Develop and coordinate institute-wide communications and outreach across multiple channels to strengthen community engagement with sustainability programs and initiatives.</li>
                </ul>
            </div>

            <div class="card">
                <div class="card-header">
                    <div>
                        <div class="card-title">Hanley Sustainability Institute</div>
                        <div class="card-subtitle">Zero Waste Specialist</div>
                    </div>
                    <div class="card-meta">May 2025 – Aug 2025</div>
                </div>
                <ul class="bullets">
                    <li>Developed an Excel-based ROI and cost-scenario model for University Dining Services' reusable container program, supporting data-driven decision-making and long-term financial planning.</li>
                    <li>Analyzed operational logistics, infrastructure needs, and program expansion scenarios, producing recommendations projected to save costs by $83,000 annually.</li>
                    <li>Planned and executed a reuse pop-up pilot engaging 300+ participants, diverting 1,500 pounds of textiles from the landfill and contributing to institutional waste-reduction goals.</li>
                </ul>
            </div>

            <div class="card">
                <div class="card-header">
                    <div>
                        <div class="card-title">Hanley Sustainability Institute</div>
                        <div class="card-subtitle">Sustainability Student Leader in Circularity Team</div>
                    </div>
                    <div class="card-meta">Dec 2023 – Present</div>
                </div>
                <ul class="bullets">
                    <li>Launch and develop the Flyer Refillery, a student-led sustainability venture, implementing sustainable product sourcing, managing container logistics, and coordinating campus-wide refill operations.</li>
                    <li>Lead sustainability consulting projects for 8 student-run enterprises by conducting operational audits and delivering actionable recommendations to enhance sustainable business practices.</li>
                </ul>
            </div>
        </section>

        <section id="leadership">
            <h2 class="section-title">Leadership & Campus Impact</h2>
            <div class="card">
                <div class="card-header">
                    <div>
                        <div class="card-title">Flyer Consulting</div>
                        <div class="card-subtitle">Consultant | Marketing Committee Lead</div>
                    </div>
                    <div class="card-meta">Sep 2025 – Present</div>
                </div>
                <ul class="bullets">
                    <li>Contributed to consulting projects for nonprofit and micro-business clients by conducting research, analyzing operational and financial data, and translating quantitative insights into client-ready recommendations.</li>
                    <li>Led the Marketing Committee for Flyer Consulting by coordinating branding, outreach, and promotional strategies to increase the organization's visibility and engagement.</li>
                </ul>
            </div>
        </section>

        <section id="skills">
            <h2 class="section-title">Technical Skills</h2>
            <div class="card">
                <div class="skills-group">
                    <h3>Data Analytics & Programming</h3>
                    <div class="badge-container">
                        <span class="badge">Python</span>
                        <span class="badge">R</span>
                        <span class="badge">SQL</span>
                        <span class="badge">Power BI</span>
                        <span class="badge">Tableau</span>
                        <span class="badge">Regression Analysis</span>
                        <span class="badge">Hypothesis Testing</span>
                        <span class="badge">Optimization Modeling</span>
                    </div>
                </div>
                <div class="skills-group">
                    <h3>Financial Modeling</h3>
                    <div class="badge-container">
                        <span class="badge">Managerial Accounting</span>
                        <span class="badge">Expense Forecasting</span>
                        <span class="badge">ROI Analysis</span>
                        <span class="badge">Scenario Modeling</span>
                    </div>
                </div>
                <div class="skills-group">
                    <h3>Operations & Consulting</h3>
                    <div class="badge-container">
                        <span class="badge">Consulting</span>
                        <span class="badge">Project Management</span>
                        <span class="badge">Impact Reporting</span>
                        <span class="badge">Process Optimization</span>
                        <span class="badge">Data-Driven Insights</span>
                    </div>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>&copy; 2026 Zay Min Htike &bull; Designed for Portfolio Showcase</p>
    </footer>

</body>
</html>
