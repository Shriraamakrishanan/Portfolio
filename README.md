# Ex01 Portfolio


## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
## HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shri Raama Krishanan J | Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <nav>
            <div class="logo-container">
                <span class="logo-text">Shri Raama Krishanan J</span>
            </div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#experience">Achievements</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="hero-container">
                <div class="hero-image">
                    <img src="profile.jpeg" alt="Shri Raama Krishanan J">
                </div>
                <div class="hero-content">
                    <h1>Shri Raama Krishanan <span class="highlight">J</span></h1>
                    <p class="subtitle">IT Undergraduate at Saveetha Engineering College | AI & Cloud Strategist</p>
                    <div class="hero-tags">
                        <span>Machine Learning</span> • <span>Cloud Computing</span> • <span>Gen AI</span>
                    </div>
                    <a href="#projects" class="btn">View My Work</a>
                </div>
            </div>
        </section>

        <section id="about" class="container">
            <div class="section-header">
                <span class="eyebrow">Biography</span>
                <h2>Professional Summary</h2>
            </div>
            <p>I am a focused IT student at <strong>Saveetha Engineering College</strong>, currently in my 2nd year. My work sits at the intersection of security and intelligence. Having completed specialized tracks in Machine Learning and Generative AI at Kyndryl, I leverage modern tech stacks to build applications that ensure digital credibility and user integrity.</p>
        </section>

        <section id="projects" class="container">
            <div class="section-header">
                <span class="eyebrow">Portfolio</span>
                <h2>Featured Projects</h2>
            </div>
            <div class="project-grid">
                <div class="project-card">
                    <div class="tag">AI & NLP</div>
                    <h3>Trust AI</h3>
                    <p>A sophisticated credibility assessment tool that detects misinformation. It verifies the integrity of information using real-time true/false detection algorithms.</p>
                </div>
                <div class="project-card">
                    <div class="tag">Cybersecurity</div>
                    <h3>Safe Exam Portal</h3>
                    <p>A secure web-based proctoring solution. It monitors user interactivity and identifies anonymous or unauthorized behavior to ensure a fair testing environment.</p>
                </div>
            </div>
        </section>

        <section id="experience" class="container">
            <div class="section-header">
                <span class="eyebrow">Recognition</span>
                <h2>Milestones</h2>
            </div>
            <div class="timeline">
                <div class="milestone">
                    <h4>Pre-Finalist</h4>
                    <p>Google Developer Program & Hack to Skills.</p>
                </div>
                <div class="milestone">
                    <h4>Event Coordinator</h4>
                    <p>AWS Kyndryl Hackathon — Orchestrated technical logistics and team coordination.</p>
                </div>
                <div class="milestone">
                    <h4>Kyndryl Certified</h4>
                    <p>Expertise in Machine Learning, Cloud Computing, and Generative AI.</p>
                </div>
            </div>
        </section>
    </main>

    <footer id="contact">
        <div class="container">
            <h2>Get In Touch</h2>
            <p>Ready to discuss the next innovation in AI and Cloud.</p>
            <div class="contact-methods">
                <p><strong>Direct:</strong> +91 9025934788</p>
                <div class="social-links">
                    <a href="https://www.linkedin.com/in/shri-raama-krishanan-j-6708bb32a" target="_blank" class="ln-link">Connect on LinkedIn →</a>
                </div>
            </div>
            <p class="copyright">&copy; 2026 Shri Raama Krishanan J. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>
```
## CSS CODE:
```css
:root {
    --primary: #0984e3;
    --dark: #1e272e;
    --light: #f5f6fa;
    --text: #2f3640;
}

* { margin: 0; padding: 0; box-sizing: border-box; }

body {
    font-family: 'Inter', sans-serif;
    line-height: 1.6;
    color: var(--text);
    background-color: #fff;
    scroll-behavior: smooth;
}

/* Layout */
.container {
    max-width: 1000px;
    margin: 0 auto;
    padding: 100px 20px;
}

/* Navigation */
header {
    padding: 20px 0;
    position: sticky;
    top: 0;
    background: rgba(255,255,255,0.9);
    backdrop-filter: blur(10px);
    z-index: 100;
    border-bottom: 1px solid #eee;
}

nav {
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.logo-text {
    font-weight: 800;
    font-size: 1.4rem;
    color: var(--dark);
}

.nav-links { display: flex; list-style: none; }
.nav-links li { margin-left: 30px; }
.nav-links a { text-decoration: none; color: var(--text); font-weight: 500; font-size: 0.9rem; }

/* Hero */
.hero {
    background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
    padding: 100px 20px;
}

.hero-container {
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    gap: 50px;
}

.hero-image img {
    width: 300px;
    height: 300px;
    border-radius: 20px;
    object-fit: cover;
    box-shadow: 0 20px 40px rgba(0,0,0,0.1);
}

.hero h1 { font-size: 3.5rem; font-weight: 800; line-height: 1.1; margin-bottom: 15px; }
.highlight { color: var(--primary); }
.subtitle { font-size: 1.2rem; color: #636e72; margin-bottom: 20px; }

.hero-tags { margin-bottom: 30px; font-size: 0.8rem; font-weight: 600; color: #aaa; text-transform: uppercase; }

.btn {
    padding: 15px 35px;
    background: var(--dark);
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
    font-weight: 600;
    transition: 0.3s;
}

.btn:hover { background: var(--primary); transform: translateY(-3px); }

/* Sections */
.eyebrow { color: var(--primary); text-transform: uppercase; font-size: 0.75rem; font-weight: 700; letter-spacing: 2px; display: block; margin-bottom: 10px; }
h2 { font-size: 2.2rem; font-weight: 800; margin-bottom: 30px; }

/* Project Cards */
.project-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; }
.project-card { padding: 40px; background: var(--light); border-radius: 15px; transition: 0.3s; }
.project-card:hover { background: #fff; box-shadow: 0 15px 30px rgba(0,0,0,0.05); }
.tag { color: var(--primary); font-size: 0.7rem; font-weight: 700; margin-bottom: 10px; }

/* Timeline */
.milestone { margin-bottom: 20px; padding-bottom: 20px; border-bottom: 1px solid #eee; }
.milestone h4 { font-weight: 700; color: var(--dark); }

/* Footer */
footer { background: var(--dark); color: #fff; text-align: center; padding: 100px 20px; }
footer h2 { color: #fff; }
.ln-link { color: var(--primary); text-decoration: none; font-weight: 600; }
.copyright { margin-top: 50px; font-size: 0.8rem; opacity: 0.5; }

/* Responsive */
@media (max-width: 768px) {
    .hero-container { flex-direction: column; text-align: center; }
    .project-grid { grid-template-columns: 1fr; }
    .hero h1 { font-size: 2.5rem; }
}
```

## OUTPUT
## Profile:
![alt text](<Screenshot 2026-04-27 115218.png>)
## About:
![alt text](<Screenshot 2026-04-27 115227.png>)
## Projects:
![alt text](<Screenshot 2026-04-27 115236.png>)
## Achivements:
![alt text](<Screenshot 2026-04-27 115247.png>)
## Contact:
![alt text](<Screenshot 2026-04-27 115301.png>)
## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
