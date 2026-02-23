<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Irfan · Sr Full‑Stack · Azure DevOps</title>
    <!-- Font & Icons (clean & professional) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Devicon for technology icons (same style as original) -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #f2f5fa;
            font-family: 'Inter', sans-serif;
            color: #1e293b;
            line-height: 1.5;
            padding: 2rem 1rem;
            display: flex;
            justify-content: center;
        }

        .github-profile {
            max-width: 1200px;
            width: 100%;
            background: white;
            border-radius: 2rem;
            box-shadow: 0 25px 50px -12px rgba(0,0,0,0.2);
            overflow: hidden;
        }

        /* header — Muhammad Irfan */
        .profile-header {
            background: linear-gradient(115deg, #0b1f33, #183b56);
            color: white;
            padding: 2rem 2.5rem;
        }

        .greeting {
            font-size: 2.2rem;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 8px;
            margin-bottom: 0.3rem;
        }

        .greeting i {
            font-size: 2rem;
            color: #ffd966;
        }

        .role-badge {
            font-size: 1.4rem;
            font-weight: 500;
            color: #b6d0e9;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            flex-wrap: wrap;
            margin-bottom: 1.5rem;
        }

        .role-badge i {
            font-size: 1.8rem;
        }

        .quick-links {
            display: flex;
            flex-wrap: wrap;
            gap: 1.8rem 2.5rem;
            background: rgba(255,255,255,0.06);
            border-radius: 48px;
            padding: 1rem 2rem;
            border: 1px solid #2d557a;
            margin-top: 1rem;
        }

        .quick-links a {
            color: white;
            text-decoration: none;
            font-size: 1.05rem;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: 0.2s;
            font-weight: 500;
        }

        .quick-links a i {
            font-size: 1.4rem;
            color: #98c1ff;
        }

        .quick-links a:hover {
            color: #d4e2ff;
            transform: translateY(-2px);
        }

        /* main area: two column */
        .core-content {
            display: grid;
            grid-template-columns: 1fr 2.2fr;
            background: white;
        }

        /* left panel — skills, education, languages (like Irfan PDF) */
        .left-panel {
            background: #f8fbfe;
            padding: 2.2rem 2rem;
            border-right: 1px solid #e2e8f0;
        }

        .section {
            margin-bottom: 2.4rem;
        }

        .section-title {
            font-size: 1.1rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.03em;
            color: #1e3a5f;
            border-bottom: 3px solid #1e3a5f;
            padding-bottom: 0.45rem;
            display: inline-block;
            margin-bottom: 1.2rem;
        }

        .skill-cat {
            font-weight: 700;
            margin: 1rem 0 0.4rem 0;
            color: #0f2b40;
            font-size: 0.95rem;
        }

        .skill-cloud {
            display: flex;
            flex-wrap: wrap;
            gap: 0.45rem;
        }

        .skill-tag {
            background: white;
            border: 1px solid #cbd5e1;
            padding: 0.3rem 1.1rem;
            border-radius: 40px;
            font-size: 0.85rem;
            font-weight: 500;
            color: #1e3a5f;
            box-shadow: 0 1px 4px rgba(0,0,0,0.02);
        }

        .skill-tag i {
            margin-right: 4px;
            color: #2563ad;
            font-size: 0.9rem;
        }

        .lang-row {
            display: flex;
            justify-content: space-between;
            padding: 0.45rem 0;
            border-bottom: 1px dashed #cfddee;
        }

        .lang-row strong {
            font-weight: 600;
        }

        .edu-item {
            margin: 1rem 0 0.8rem;
        }

        .edu-item h4 {
            font-weight: 700;
            font-size: 1rem;
        }

        .edu-meta {
            color: #3f5468;
            font-size: 0.9rem;
        }

        /* right panel — experience & projects (PDF style) */
        .right-panel {
            padding: 2.2rem 2.2rem 2.2rem 2rem;
        }

        .exp-block, .project-block {
            margin-bottom: 2.2rem;
        }

        .exp-header {
            display: flex;
            flex-wrap: wrap;
            align-items: baseline;
            justify-content: space-between;
        }

        .exp-header h3 {
            font-size: 1.3rem;
            font-weight: 700;
            color: #0b263b;
        }

        .exp-company {
            font-weight: 600;
            color: #1f4a7a;
            margin-right: 1rem;
        }

        .exp-date {
            background: #e2eaf3;
            padding: 0.2rem 1.1rem;
            border-radius: 30px;
            font-size: 0.8rem;
            font-weight: 600;
            color: #1e3a5f;
        }

        .exp-sub {
            font-weight: 600;
            margin: 0.6rem 0 0.3rem;
            color: #2b4764;
        }

        .exp-desc {
            list-style: none;
        }

        .exp-desc li {
            display: flex;
            gap: 0.8rem;
            margin-bottom: 0.65rem;
            font-size: 0.95rem;
        }

        .exp-desc li i {
            color: #1e3a5f;
            font-size: 0.8rem;
            margin-top: 0.25rem;
            min-width: 1rem;
        }

        .project-item h4 {
            font-size: 1.2rem;
            font-weight: 700;
            color: #0e2d48;
        }

        .project-tech {
            font-weight: 600;
            color: #2563ad;
            font-size: 0.9rem;
            margin: 0.2rem 0 0.5rem;
        }

        .project-desc {
            font-size: 0.95rem;
            color: #253c54;
            margin-bottom: 0.5rem;
        }

        .project-desc strong {
            color: #0b2b4a;
        }

        hr {
            border: 1px solid #e2e8f0;
            margin: 1.5rem 0;
        }

        /* icons row (exactly like original but updated with Irfan's stack) */
        .tech-strip {
            background: #f0f4fa;
            padding: 1.2rem 2rem;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 1.5rem 2rem;
            border-top: 1px solid #cdddec;
            border-bottom: 1px solid #cdddec;
        }

        .tech-strip img, .tech-strip i {
            font-size: 2.2rem;
            color: #1e3a5f;
        }

        .tech-icon {
            display: inline-flex;
            align-items: center;
            gap: 0.2rem;
        }

        .tech-icon i {
            font-size: 2rem;
        }

        /* badge row (github awards style) */
        .github-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem 1.5rem;
            padding: 1.5rem 2rem;
            background: #ffffff;
            align-items: center;
        }

        .github-badges img {
            height: 42px;
            width: auto;
        }

        .fun-note {
            font-size: 0.95rem;
            color: #28527a;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .vaunt-badge {
            margin-top: 0.2rem;
            background: #eef3f9;
            padding: 0.5rem 1.2rem;
            border-radius: 40px;
            font-weight: 500;
        }

        .contact-row {
            display: flex;
            flex-wrap: wrap;
            gap: 1.8rem;
            padding: 1rem 2rem 1.5rem;
            background: #f0f6fd;
            border-top: 1px solid #bdd0e6;
            align-items: center;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            background: white;
            padding: 0.5rem 1.4rem;
            border-radius: 60px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.02);
            color: #1e3a5f;
            font-weight: 500;
        }

        .contact-item i {
            font-size: 1.3rem;
            color: #1f4e85;
        }
    </style>
</head>
<body>
    <div class="github-profile">
        <!-- header: Hi I'm Muhammad Irfan (adapted from Arslan style but professional) -->
        <div class="profile-header">
            <div class="greeting">
                <i class="fas fa-hand-peace"></i> Hi👋 I'm Muhammad Irfan
            </div>
            <div class="role-badge">
                <i class="fas fa-code"></i> Senior Full‑Stack Developer | .NET + Angular | Azure & DevOps
                <i class="fas fa-cloud"></i>
            </div>
            <!-- contact / links like original but with Irfan's data -->
            <div class="quick-links">
                <a href="#"><i class="fas fa-envelope"></i> chmuhammadirfan3@gmail.com</a>
                <a href="#"><i class="fas fa-phone-alt"></i> +92 300 7841407</a>
                <a href="#"><i class="fab fa-github"></i> github.com/ch-irfan-1</a>
                <a href="#"><i class="fab fa-linkedin"></i> linkedin.com/in/mirfan-dev</a>
            </div>
        </div>

        <!-- main content: left skills / right exp (from Muhammad_Irfan.pdf) -->
        <div class="core-content">
            <!-- LEFT PANEL (skills, education, languages) -->
            <div class="left-panel">
                <!-- Skills Summary with categories -->
                <div class="section">
                    <div class="section-title"><i class="fas fa-cog" style="margin-right:6px;"></i> SKILLS</div>
                    
                    <div class="skill-cat"><i class="fas fa-code"></i> Languages</div>
                    <div class="skill-cloud">
                        <span class="skill-tag"><i class="devicon-csharp-plain"></i> C#</span>
                        <span class="skill-tag"><i class="devicon-typescript-plain"></i> TypeScript</span>
                        <span class="skill-tag"><i class="fas fa-database"></i> SQL</span>
                    </div>

                    <div class="skill-cat"><i class="fab fa-angular"></i> Frontend</div>
                    <div class="skill-cloud">
                        <span class="skill-tag"><i class="devicon-angularjs-plain"></i> Angular (v8+)</span>
                        <span class="skill-tag"><i class="devicon-html5-plain"></i> HTML5</span>
                        <span class="skill-tag"><i class="devicon-css3-plain"></i> CSS3</span>
                        <span class="skill-tag"><i class="devicon-bootstrap-plain"></i> Bootstrap</span>
                        <span class="skill-tag"><i class="devicon-angularmaterial-plain"></i> Material</span>
                    </div>

                    <div class="skill-cat"><i class="fas fa-server"></i> Backend & Data</div>
                    <div class="skill-cloud">
                        <span class="skill-tag"><i class="devicon-dotnetcore-plain"></i> ASP.NET Core</span>
                        <span class="skill-tag">RESTful APIs</span>
                        <span class="skill-tag">Entity Framework</span>
                        <span class="skill-tag"><i class="devicon-microsoftsqlserver-plain"></i> SQL Server</span>
                        <span class="skill-tag">T-SQL, SP, Indexing</span>
                    </div>

                    <div class="skill-cat"><i class="fas fa-cloud"></i> Cloud & DevOps</div>
                    <div class="skill-cloud">
                        <span class="skill-tag"><i class="devicon-azure-plain"></i> Azure</span>
                        <span class="skill-tag">Azure DevOps</span>
                        <span class="skill-tag"><i class="devicon-jenkins-line"></i> Jenkins</span>
                        <span class="skill-tag">CI/CD Pipelines</span>
                        <span class="skill-tag"><i class="devicon-github-original"></i> GitHub</span>
                        <span class="skill-tag">SVN</span>
                    </div>

                    <div class="skill-cat"><i class="fas fa-chart-line"></i> Testing/Perf</div>
                    <div class="skill-cloud">
                        <span class="skill-tag">Visual Studio Load Test</span>
                        <span class="skill-tag">Performance Analysis</span>
                        <span class="skill-tag">Release Mgmt</span>
                    </div>

                    <div class="skill-cat"><i class="fas fa-users"></i> Soft Skills</div>
                    <div class="skill-cloud">
                        <span class="skill-tag">Problem Solving</span>
                        <span class="skill-tag">Team Collaboration</span>
                        <span class="skill-tag">Communication</span>
                        <span class="skill-tag">Time Mgmt</span>
                    </div>
                </div>

                <!-- Education -->
                <div class="section">
                    <div class="section-title"><i class="fas fa-graduation-cap"></i> EDUCATION</div>
                    <div class="edu-item">
                        <h4>University of Sargodha</h4>
                        <div class="edu-meta">Bachelor of Science in Computer Science</div>
                        <div class="edu-meta" style="color:#4a6582;">Sep 2015 - Jun 2019 · Sargodha, Pakistan</div>
                    </div>
                </div>

                <!-- Languages -->
                <div class="section">
                    <div class="section-title"><i class="fas fa-language"></i> LANGUAGES</div>
                    <div class="lang-row"><strong>English</strong> <span>Professional</span></div>
                    <div class="lang-row"><strong>Urdu</strong> <span>Native</span></div>
                </div>
            </div>

            <!-- RIGHT PANEL : Experience & Projects (exactly from PDF) -->
            <div class="right-panel">
                <!-- Experience -->
                <div class="section" style="margin-top:0;">
                    <div class="section-title"><i class="fas fa-briefcase"></i> EXPERIENCE</div>
                    
                    <div class="exp-block">
                        <div class="exp-header">
                            <h3>NETSOL Technologies</h3>
                            <span class="exp-date">March 2020 - Present</span>
                        </div>
                        <div class="exp-sub">Senior Software Engineer - Full-Stack Developer · Pakistan</div>
                        <ul class="exp-desc">
                            <li><i class="fas fa-angle-right"></i> <strong>Full‑Stack (2023–present)</strong> – ASP.NET Core REST APIs, Angular v8+, SQL Server. Reusable components, RxJS, seamless integration.</li>
                            <li><i class="fas fa-angle-right"></i> <strong>SQL Server (2022–2023)</strong> – Complex queries, stored procedures, performance tuning, data analysis.</li>
                            <li><i class="fas fa-angle-right"></i> <strong>Performance & Load Testing (2021–2022)</strong> – Visual Studio Load Test (controller/agent), bottleneck analysis, scalability.</li>
                            <li><i class="fas fa-angle-right"></i> <strong>Release Management (2019–2021)</strong> – Full lifecycle, versioning, production hotfixes, cross-team coordination.</li>
                            <li><i class="fas fa-angle-right"></i> <strong>CI/CD & DevOps</strong> – Jenkins, Git, automated pipelines, reduced deployment risks.</li>
                        </ul>
                    </div>
                </div>

                <!-- Projects (detailed) -->
                <div class="section">
                    <div class="section-title"><i class="fas fa-project-diagram"></i> PROJECTS</div>
                    
                    <div class="project-block">
                        <h4>Summit Oto Vehicle Leasing Platform</h4>
                        <div class="project-tech">Angular · ASP.NET Core · SQL Server</div>
                        <div class="project-desc"><strong>Description:</strong> Digital leasing for cars/bikes – retail applications, dealer inventory, EMI plans, lease processing.</div>
                        <div class="project-desc"><strong>Responsibilities:</strong> Built Angular retail interfaces, dynamic forms/validations, integrated lease calculation APIs, end‑to‑end workflow.</div>
                    </div>

                    <div class="project-block">
                        <h4>WFS (Wholesale Financing System)</h4>
                        <div class="project-tech">SQL Server · Stored Procedures · C#</div>
                        <div class="project-desc"><strong>Description:</strong> Enterprise wholesale financing for dealers, multi‑country, high‑volume transactions.</div>
                        <div class="project-desc"><strong>Responsibilities:</strong> Optimized stored procedures, schema changes, resolved production invoice/cancellation issues, ensured data integrity.</div>
                    </div>
                </div>

                <!-- additional mini section: objective inline (since PDF had one) -->
                <div style="background: #eaf1fb; padding: 1rem; border-radius: 20px; margin-top: 0.8rem;">
                    <i class="fas fa-bullseye" style="color:#1e3a5f; margin-right: 8px;"></i> 
                    <strong>Objective:</strong> Senior Software Engineer leveraging full‑stack and DevOps skills to deliver scalable, high‑quality solutions in dynamic environment.
                </div>
            </div>
        </div>

        <!-- technology strip exactly as original but updated with Irfan's stack (c#, ts, angular, etc) -->
        <div class="tech-strip">
            <span class="tech-icon"><i class="devicon-csharp-plain colored"></i></span>
            <span class="tech-icon"><i class="devicon-typescript-plain colored"></i></span>
            <span class="tech-icon"><i class="devicon-angularjs-plain colored"></i></span>
            <span class="tech-icon"><i class="devicon-dotnetcore-plain colored"></i></span>
            <span class="tech-icon"><i class="devicon-microsoftsqlserver-plain colored"></i></span>
            <span class="tech-icon"><i class="devicon-azure-plain colored"></i></span>
            <span class="tech-icon"><i class="devicon-jenkins-line colored"></i></span>
            <span class="tech-icon"><i class="devicon-github-original colored"></i></span>
            <span class="tech-icon"><i class="devicon-visualstudio-plain colored"></i></span>
            <span class="tech-icon"><i class="fas fa-chart-bar" style="color:#1e6823;"></i></span> <!-- load test -->
        </div>

        <!-- GitHub badges / contributions (similar to original but tasteful) -->
        <div class="github-badges">
            <a href="#"><img src="https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/acbadge.gif" alt="archive"></a>
            <a href="#"><img src="https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/devbadge.gif" alt="dev"></a>
            <a href="#"><img src="https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/pro.gif" alt="pro"></a>
            <a href="#"><img src="https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/starbadge.gif" width="35" alt="star"></a>
            <span class="fun-note"><i class="fas fa-microchip"></i> Industrial full‑stack · Azure & Angular</span>
        </div>

        <!-- vaunt / extra contributions line (exactly as requested) -->
        <div style="padding: 0.2rem 2rem 1rem;">
            <span class="vaunt-badge"><i class="fas fa-check-circle" style="color:#2a6f97;"></i> ![Vaunt Badge](https://api.vaunt.dev/v1/github/entities/ch-irfan-1/contributions?format=svg&private=false) </span>
        </div>

        <!-- contact row similar to original (with whatsapp/gmail/linkedin) but adapted for Irfan -->
        <div class="contact-row">
            <a href="#" style="text-decoration: none;"><span class="contact-item"><i class="fab fa-linkedin"></i> ch-irfan-1</span></a>
            <a href="#" style="text-decoration: none;"><span class="contact-item"><i class="fab fa-whatsapp"></i> +92 300 7841407</span></a>
            <a href="#" style="text-decoration: none;"><span class="contact-item"><i class="far fa-envelope"></i> chmuhammadirfan3</span></a>
            <span class="contact-item"><i class="fas fa-map-pin"></i> Pakistan</span>
        </div>

        <!-- small note: all original Arslan markers are replaced with Irfan's data, but style kept -->
        <div style="text-align: right; padding: 0.5rem 2rem 1.2rem; font-size:0.8rem; background: white; color:#5d7184; border-top: 1px solid #e4edf5;">
            <i class="fas fa-sync"></i> designed from Muhammad_Irfan.pdf · scalable & consistent
        </div>
    </div>
</body>
</html>
