/* ===================================
   PROFESSIONAL PORTFOLIO STYLES
   Premium Design & Enhanced UX ✨
   =================================== */

/* ===================
   CSS VARIABLES (Design Tokens)
   =================== */
   :root {
    /* Refined Color Palette 🎨 */
    --primary-color: #4f46e5;
    --primary-dark: #4338ca;
    --primary-light: #6366f1;
    --secondary-color: #06b6d4;
    --accent-color: #10b981;
    --accent-orange: #f59e0b;
    --accent-purple: #8b5cf6;
    --text-color: #1e293b;
    --text-light: #64748b;
    --text-muted: #94a3b8;
    --background: #ffffff;
    --background-alt: #f8fafc;
    --background-card: #ffffff;
    --border-color: #e2e8f0;
    
    /* Professional Gradients 🌈 */
    --gradient-primary: linear-gradient(135deg, #4f46e5 0%, #7c3aed 100%);
    --gradient-secondary: linear-gradient(135deg, #06b6d4 0%, #3b82f6 100%);
    --gradient-accent: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
    --gradient-warm: linear-gradient(135deg, #f59e0b 0%, #ef4444 100%);
    --gradient-overlay: linear-gradient(180deg, rgba(0,0,0,0.7) 0%, rgba(0,0,0,0.4) 100%);
    
    /* Refined Shadows */
    --shadow-xs: 0 1px 2px rgba(0, 0, 0, 0.04);
    --shadow-sm: 0 2px 4px rgba(0, 0, 0, 0.06);
    --shadow-md: 0 4px 12px rgba(0, 0, 0, 0.08);
    --shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.12);
    --shadow-xl: 0 16px 40px rgba(0, 0, 0, 0.16);
    --shadow-glow: 0 0 24px rgba(79, 70, 229, 0.3);
    
    /* Typography */
    --font-main: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Inter', sans-serif;
    
    /* Spacing */
    --spacing-xs: 0.5rem;
    --spacing-sm: 1rem;
    --spacing-md: 2rem;
    --spacing-lg: 3rem;
    --spacing-xl: 5rem;
    
    /* Border Radius */
    --radius-sm: 0.375rem;
    --radius-md: 0.5rem;
    --radius-lg: 0.75rem;
    --radius-xl: 1rem;
    --radius-2xl: 1.5rem;
    
    /* Professional Transitions */
    --transition-fast: all 0.15s cubic-bezier(0.4, 0, 0.2, 1);
    --transition-base: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
    --transition-slow: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}

/* ===================
   RESET & BASE STYLES
   =================== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    overflow-x: hidden;
}

body {
    font-family: var(--font-main);
    color: var(--text-color);
    background: var(--background);
    line-height: 1.7;
    overflow-x: hidden;
    position: relative;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

/* Subtle Background Pattern */
body::before {
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: 
        radial-gradient(circle at 20% 50%, rgba(79, 70, 229, 0.03) 0%, transparent 50%),
        radial-gradient(circle at 80% 80%, rgba(6, 182, 212, 0.03) 0%, transparent 50%),
        radial-gradient(circle at 40% 20%, rgba(139, 92, 246, 0.02) 0%, transparent 50%);
    pointer-events: none;
    z-index: -1;
}

img {
    max-width: 100%;
    height: auto;
    display: block;
}

a {
    text-decoration: none;
    color: inherit;
}

/* ===================
   CONTAINER & LAYOUT
   =================== */
.container {
    max-width: 1280px;
    margin: 0 auto;
    padding: 0 var(--spacing-md);
}

.section {
    padding: var(--spacing-xl) 0;
    position: relative;
}

.section-alt {
    background: var(--background-alt);
}

.section-title {
    font-size: 2.75rem;
    font-weight: 800;
    margin-bottom: var(--spacing-sm);
    text-align: center;
    color: var(--text-color);
    position: relative;
    display: inline-block;
    width: 100%;
    letter-spacing: -0.02em;
    animation: fadeInUp 0.6s ease-out;
}

.section-title::before {
    content: '';
    position: absolute;
    bottom: -20px;
    left: 50%;
    transform: translateX(-50%);
    width: 0;
    height: 4px;
    background: var(--gradient-primary);
    border-radius: 999px;
    animation: fadeInUp 0.8s ease-out 0.3s both;
}

.section-title::after {
    content: '';
    position: absolute;
    bottom: -16px;
    left: 50%;
    transform: translateX(-50%);
    width: 80px;
    height: 4px;
    background: var(--gradient-primary);
    border-radius: 999px;
    box-shadow: 0 0 20px rgba(79, 70, 229, 0.5);
}

.section-subtitle {
    font-size: 1.125rem;
    color: var(--text-light);
    text-align: center;
    margin-bottom: var(--spacing-lg);
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.8;
}

/* ===================
   ENHANCED ANIMATIONS
   =================== */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes slideInLeft {
    from {
        opacity: 0;
        transform: translateX(-30px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes slideInRight {
    from {
        opacity: 0;
        transform: translateX(30px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-12px); }
}

@keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.05); }
}

@keyframes shimmer {
    0% { background-position: -1000px 0; }
    100% { background-position: 1000px 0; }
}

@keyframes gradientShift {
    0%, 100% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
}

@keyframes glow {
    0%, 100% { box-shadow: 0 0 20px rgba(79, 70, 229, 0.3); }
    50% { box-shadow: 0 0 40px rgba(79, 70, 229, 0.6); }
}

@keyframes rotate {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
}

/* ===================
   NAVIGATION BAR
   =================== */
.navbar {
    background: rgba(255, 255, 255, 0.85);
    backdrop-filter: blur(20px) saturate(180%);
    -webkit-backdrop-filter: blur(20px) saturate(180%);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
    border-bottom: 1px solid rgba(226, 232, 240, 0.8);
    position: sticky;
    top: 0;
    z-index: 1000;
    padding: 1.125rem 0;
    transition: var(--transition-base);
}

.navbar::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 1px;
    background: var(--gradient-primary);
    opacity: 0;
    transition: var(--transition-base);
}

.navbar:hover::before {
    opacity: 1;
}

.navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-brand a {
    font-size: 1.5rem;
    font-weight: 800;
    background: var(--gradient-primary);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    transition: var(--transition-base);
    letter-spacing: -0.02em;
}

.nav-brand a:hover {
    opacity: 0.8;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 0.25rem;
}

.nav-menu a {
    color: var(--text-color);
    font-weight: 600;
    font-size: 0.9375rem;
    padding: 0.625rem 1.25rem;
    border-radius: var(--radius-md);
    position: relative;
    transition: var(--transition-base);
    overflow: hidden;
}

.nav-menu a::before {
    content: '';
    position: absolute;
    inset: 0;
    background: var(--gradient-primary);
    opacity: 0;
    border-radius: inherit;
    transition: var(--transition-base);
    z-index: -1;
    transform: scale(0.8);
}

.nav-menu a::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 0;
    height: 2px;
    background: var(--primary-color);
    transform: translateX(-50%);
    transition: var(--transition-base);
}

.nav-menu a:hover {
    color: white;
    transform: translateY(-2px);
}

.nav-menu a:hover::before {
    opacity: 1;
    transform: scale(1);
}

.nav-menu a:hover::after {
    width: 80%;
}

.nav-menu a.active {
    color: var(--primary-color);
    font-weight: 700;
}

.nav-menu a.active::after {
    width: 80%;
    background: var(--primary-color);
}

/* Mobile Navigation */
.nav-toggle {
    display: none;
    width: 44px;
    height: 44px;
    border-radius: var(--radius-md);
    background: var(--background);
    box-shadow: var(--shadow-sm);
    align-items: center;
    justify-content: center;
    gap: 5px;
    flex-direction: column;
    cursor: pointer;
    transition: var(--transition-base);
    border: 1px solid var(--border-color);
}

.nav-toggle span {
    width: 24px;
    height: 2px;
    border-radius: 999px;
    background: var(--primary-color);
    transition: var(--transition-base);
}

.nav-toggle.active span:nth-child(1) {
    transform: translateY(7px) rotate(45deg);
}

.nav-toggle.active span:nth-child(2) {
    opacity: 0;
}

.nav-toggle.active span:nth-child(3) {
    transform: translateY(-7px) rotate(-45deg);
}

@media (max-width: 992px) {
    .nav-toggle {
        display: flex;
    }
    
    .nav-menu {
        position: absolute;
        top: calc(100% + 12px);
        right: var(--spacing-md);
        width: min(300px, calc(100vw - var(--spacing-lg)));
        flex-direction: column;
        padding: var(--spacing-sm);
        background: rgba(255, 255, 255, 0.98);
        backdrop-filter: blur(16px);
        border-radius: var(--radius-xl);
        box-shadow: var(--shadow-lg);
        border: 1px solid var(--border-color);
        opacity: 0;
        pointer-events: none;
        transform: translateY(-10px);
        transition: var(--transition-base);
    }
    
    .nav-menu.active {
        opacity: 1;
        pointer-events: all;
        transform: translateY(0);
    }
    
    .nav-menu a {
        display: block;
        text-align: center;
        width: 100%;
    }
}

/* ===================
   HERO SECTION
   =================== */
.hero {
    padding: calc(var(--spacing-xl) + 2rem) 0;
    min-height: 90vh;
    display: flex;
    align-items: center;
    position: relative;
    overflow: hidden;
}

.hero::before {
    content: '';
    position: absolute;
    top: -50%;
    right: -10%;
    width: 600px;
    height: 600px;
    background: var(--gradient-primary);
    border-radius: 50%;
    opacity: 0.08;
    filter: blur(80px);
    animation: float 8s ease-in-out infinite;
    z-index: -1;
}

.hero::after {
    content: '';
    position: absolute;
    bottom: -30%;
    left: -10%;
    width: 500px;
    height: 500px;
    background: var(--gradient-secondary);
    border-radius: 50%;
    opacity: 0.06;
    filter: blur(80px);
    animation: float 10s ease-in-out infinite reverse;
    z-index: -1;
}

.hero-content {
    display: grid;
    grid-template-columns: 380px 1fr;
    gap: var(--spacing-xl);
    align-items: center;
}

.hero-image {
    position: relative;
}

.hero-image::before {
    content: '';
    position: absolute;
    inset: -20px;
    background: var(--gradient-primary);
    border-radius: 50%;
    opacity: 0.15;
    filter: blur(50px);
    animation: pulse 4s ease-in-out infinite;
    z-index: -1;
}

.hero-image::after {
    content: '';
    position: absolute;
    inset: -10px;
    border-radius: 50%;
    border: 3px solid transparent;
    border-top-color: var(--primary-color);
    border-right-color: var(--secondary-color);
    animation: rotate 8s linear infinite;
    opacity: 0.3;
}

.hero-image img {
    width: 100%;
    max-width: 380px;
    aspect-ratio: 1;
    border-radius: 50%;
    object-fit: cover;
    border: 6px solid var(--background);
    box-shadow: var(--shadow-xl), 0 0 0 0 rgba(79, 70, 229, 0.4);
    position: relative;
    transition: var(--transition-slow);
    animation: fadeInUp 0.8s ease-out 0.2s both;
}

.hero-image img:hover {
    transform: scale(1.05) rotate(2deg);
    box-shadow: var(--shadow-xl), 0 0 40px rgba(79, 70, 229, 0.5);
    border-color: rgba(79, 70, 229, 0.2);
}

.hero-text h1 {
    font-size: 3.75rem;
    font-weight: 900;
    margin-bottom: var(--spacing-sm);
    line-height: 1.1;
    letter-spacing: -0.03em;
    color: var(--text-color);
    animation: fadeInUp 0.8s ease-out 0.1s both;
}

.hero-text .highlight {
    background: var(--gradient-primary);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: gradientShift 3s ease infinite;
    position: relative;
    display: inline-block;
}

.hero-text .highlight::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 4px;
    background: var(--gradient-primary);
    border-radius: 2px;
    opacity: 0.3;
    animation: pulse 2s ease-in-out infinite;
}

.tagline {
    font-size: 1.5rem;
    color: var(--primary-color);
    margin-bottom: var(--spacing-md);
    font-weight: 700;
}

.intro {
    font-size: 1.125rem;
    color: var(--text-light);
    margin-bottom: var(--spacing-lg);
    line-height: 1.8;
    max-width: 600px;
}

.hero-buttons {
    display: flex;
    gap: var(--spacing-md);
    flex-wrap: wrap;
}

/* ===================
   MODERN BUTTONS
   =================== */
.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 0.875rem 2rem;
    border-radius: var(--radius-md);
    font-weight: 700;
    font-size: 1rem;
    text-align: center;
    cursor: pointer;
    border: none;
    position: relative;
    overflow: hidden;
    transition: var(--transition-base);
    letter-spacing: 0.01em;
    z-index: 1;
}

.btn::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.3);
    transform: translate(-50%, -50%);
    transition: width 0.6s, height 0.6s;
    z-index: -1;
}

.btn:hover::before {
    width: 300px;
    height: 300px;
}

.btn-primary {
    background: var(--gradient-primary);
    color: white;
    box-shadow: var(--shadow-md);
}

.btn-primary:hover {
    transform: translateY(-3px);
    box-shadow: var(--shadow-lg), 0 0 20px rgba(79, 70, 229, 0.4);
}

.btn-primary:active {
    transform: translateY(-1px);
}

.btn-secondary {
    background: var(--background);
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
    box-shadow: var(--shadow-sm);
}

.btn-secondary:hover {
    background: var(--gradient-primary);
    color: white;
    border-color: transparent;
    transform: translateY(-3px);
    box-shadow: var(--shadow-lg);
}

.btn-small {
    padding: 0.625rem 1.5rem;
    font-size: 0.875rem;
}

/* ===================
   MODERN CARDS
   =================== */
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: var(--spacing-md);
    margin-top: var(--spacing-lg);
}

.card {
    background: var(--background-card);
    padding: var(--spacing-lg);
    border-radius: var(--radius-xl);
    box-shadow: var(--shadow-sm);
    text-align: center;
    border: 1px solid var(--border-color);
    transition: var(--transition-base);
    position: relative;
    overflow: hidden;
}

.card::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(79, 70, 229, 0.1), transparent);
    transition: var(--transition-slow);
}

.card:hover::before {
    left: 100%;
}

.card:hover {
    transform: translateY(-8px) scale(1.02);
    box-shadow: var(--shadow-xl), 0 0 30px rgba(79, 70, 229, 0.15);
    border-color: var(--primary-light);
}

.card-icon {
    font-size: 3rem;
    margin-bottom: var(--spacing-sm);
    background: var(--gradient-primary);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.card h3 {
    font-size: 1.5rem;
    margin-bottom: var(--spacing-xs);
    color: var(--text-color);
    font-weight: 700;
}

.card p {
    color: var(--text-light);
    line-height: 1.7;
}

/* ===================
   ABOUT PREVIEW SECTION
   =================== */
.about-preview {
    padding: var(--spacing-xl) 0;
    position: relative;
}

.about-preview h2 {
    font-size: 2.5rem;
    font-weight: 800;
    text-align: center;
    margin-bottom: var(--spacing-lg);
    color: var(--text-color);
    animation: fadeInUp 0.6s ease-out;
}

/* ===================
   SKILLS SECTION
   =================== */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: var(--spacing-md);
    margin-top: var(--spacing-lg);
}

.skill-category {
    background: var(--background-card);
    padding: var(--spacing-lg);
    border-radius: var(--radius-xl);
    box-shadow: var(--shadow-sm);
    border: 1px solid var(--border-color);
    border-left: 4px solid var(--primary-color);
    transition: var(--transition-base);
}

.skill-category:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-md);
}

.skill-category h3 {
    font-size: 1.375rem;
    margin-bottom: var(--spacing-md);
    color: var(--text-color);
    font-weight: 700;
}

.skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: var(--spacing-xs);
}

.skill-tag {
    background: var(--background-alt);
    color: var(--text-color);
    padding: 0.5rem 1rem;
    border-radius: var(--radius-md);
    font-size: 0.875rem;
    font-weight: 600;
    border: 1px solid var(--border-color);
    transition: var(--transition-fast);
}

.skill-tag:hover {
    background: var(--primary-color);
    color: white;
    transform: translateY(-2px);
    border-color: var(--primary-color);
}

/* ===================
   PROJECTS SECTION
   =================== */
.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
    gap: var(--spacing-lg);
    margin-top: var(--spacing-lg);
}

.project-card {
    background: var(--background-card);
    border-radius: var(--radius-xl);
    overflow: hidden;
    box-shadow: var(--shadow-sm);
    border: 1px solid var(--border-color);
    transition: var(--transition-base);
    position: relative;
}

.project-card::after {
    content: '';
    position: absolute;
    inset: 0;
    background: var(--gradient-primary);
    opacity: 0;
    transition: var(--transition-base);
    z-index: 1;
    pointer-events: none;
}

.project-card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: var(--shadow-xl), 0 0 40px rgba(79, 70, 229, 0.2);
    border-color: var(--primary-color);
}

.project-card:hover::after {
    opacity: 0.03;
}

.project-image {
    width: 100%;
    height: 240px;
    overflow: hidden;
    position: relative;
    background: var(--gradient-primary);
}

.project-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition-slow);
}

.project-card:hover .project-image img {
    transform: scale(1.05);
}

.project-content {
    padding: var(--spacing-lg);
}

.project-content h3 {
    font-size: 1.5rem;
    margin-bottom: var(--spacing-sm);
    color: var(--text-color);
    font-weight: 700;
}

.project-content p {
    color: var(--text-light);
    margin-bottom: var(--spacing-md);
    line-height: 1.7;
}

.project-tags {
    margin-bottom: var(--spacing-md);
}

.project-tags span {
    background: var(--background-alt);
    color: var(--primary-color);
    padding: 0.375rem 0.875rem;
    border-radius: var(--radius-md);
    font-size: 0.8125rem;
    font-weight: 600;
    border: 1px solid var(--border-color);
    display: inline-block;
    margin-right: var(--spacing-xs);
    margin-bottom: var(--spacing-xs);
}

.project-links {
    display: flex;
    flex-wrap: wrap;
    gap: var(--spacing-sm);
}

/* ===================
   CERTIFICATES SECTION
   =================== */
.certificates-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
    gap: var(--spacing-lg);
    margin-top: var(--spacing-lg);
}

.certificate-card {
    background: var(--background-card);
    border-radius: var(--radius-xl);
    box-shadow: var(--shadow-sm);
    border: 1px solid var(--border-color);
    overflow: hidden;
    transition: var(--transition-base);
}

.certificate-card:hover {
    transform: translateY(-6px);
    box-shadow: var(--shadow-lg);
}

.certificate-image {
    position: relative;
    overflow: hidden;
    border-bottom: 1px solid var(--border-color);
}

.certificate-image img {
    width: 100%;
    height: 220px;
    object-fit: cover;
}

.certificate-overlay {
    position: absolute;
    inset: 0;
    background: var(--gradient-overlay);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: var(--transition-base);
}

.certificate-card:hover .certificate-overlay {
    opacity: 1;
}

.certificate-info {
    padding: var(--spacing-lg);
}

.certificate-info h3 {
    font-size: 1.375rem;
    font-weight: 700;
    color: var(--text-color);
    margin-bottom: var(--spacing-xs);
}

.certificate-issuer,
.certificate-date {
    color: var(--text-light);
    font-weight: 600;
    font-size: 0.9375rem;
}

.certificate-link {
    margin-top: var(--spacing-sm);
    font-weight: 700;
    color: var(--primary-color);
    display: inline-flex;
    align-items: center;
    gap: 6px;
    transition: var(--transition-fast);
}

.certificate-link:hover {
    color: var(--secondary-color);
}

/* ===================
   CONTACT SECTION
   =================== */
.contact-wrapper {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: var(--spacing-md);
    margin-top: var(--spacing-lg);
}

.contact-card {
    background: var(--background-card);
    padding: var(--spacing-lg);
    border-radius: var(--radius-xl);
    border: 1px solid var(--border-color);
    box-shadow: var(--shadow-sm);
    text-align: center;
    transition: var(--transition-base);
}

.contact-card:hover {
    transform: translateY(-6px);
    box-shadow: var(--shadow-md);
}

.contact-icon {
    font-size: 2.5rem;
    margin-bottom: var(--spacing-sm);
}

.contact-link {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    font-weight: 700;
    color: var(--primary-color);
    margin-bottom: var(--spacing-xs);
    transition: var(--transition-fast);
}

.contact-link:hover {
    color: var(--secondary-color);
}

/* ===================
   SOCIAL LINKS
   =================== */
.social-links {
    display: flex;
    justify-content: center;
    gap: var(--spacing-md);
    flex-wrap: wrap;
    margin-top: var(--spacing-lg);
}

.social-links a {
    width: 56px;
    height: 56px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: var(--background-card);
    border-radius: 50%;
    color: var(--text-color);
    box-shadow: var(--shadow-sm);
    border: 1px solid var(--border-color);
    transition: var(--transition-base);
    font-size: 1.5rem;
    position: relative;
    overflow: hidden;
}

.social-links a::before {
    content: '';
    position: absolute;
    inset: 0;
    background: var(--gradient-primary);
    opacity: 0;
    transition: var(--transition-base);
    border-radius: 50%;
    transform: scale(0);
}

.social-links a:hover::before {
    opacity: 1;
    transform: scale(1);
}

.social-links a:hover {
    color: white;
    transform: translateY(-6px) scale(1.1) rotate(5deg);
    box-shadow: var(--shadow-lg), 0 0 20px rgba(79, 70, 229, 0.4);
    border-color: transparent;
}

.social-links a svg {
    position: relative;
    z-index: 1;
}

/* ===================
   FOOTER
   =================== */
.footer {
    background: linear-gradient(135deg, var(--text-color) 0%, #334155 100%);
    color: white;
    padding: var(--spacing-lg) 0;
    margin-top: var(--spacing-xl);
}

.footer .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: var(--spacing-md);
}

.footer p {
    margin: 0;
    opacity: 0.9;
}

.footer-links {
    display: flex;
    gap: var(--spacing-md);
}

.footer-links a {
    transition: var(--transition-base);
    opacity: 0.9;
}

.footer-links a:hover {
    opacity: 1;
}

/* ===================
   SCROLL TO TOP
   =================== */
.scroll-to-top,
.back-to-top {
    position: fixed;
    bottom: 32px;
    right: 32px;
    width: 52px;
    height: 52px;
    background: var(--gradient-primary);
    color: white;
    border: none;
    border-radius: 50%;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.25rem;
    box-shadow: var(--shadow-lg);
    opacity: 0;
    pointer-events: none;
    transition: var(--transition-base);
    z-index: 999;
}

.scroll-to-top.show,
.back-to-top.show {
    opacity: 1;
    pointer-events: all;
    animation: fadeIn 0.3s ease-out;
}

.scroll-to-top:hover,
.back-to-top:hover {
    transform: translateY(-6px) scale(1.1);
    box-shadow: var(--shadow-xl), 0 0 30px rgba(79, 70, 229, 0.5);
    animation: glow 2s ease-in-out infinite;
}

.scroll-to-top:active,
.back-to-top:active {
    transform: translateY(-2px) scale(1.05);
}

/* ===================
   UTILITY CLASSES
   =================== */
.badge-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: var(--spacing-md);
    margin-top: var(--spacing-md);
}

.badge-link {
    display: flex;
    justify-content: center;
    padding: var(--spacing-sm);
    border-radius: var(--radius-md);
    transition: var(--transition-base);
    border: 1px solid var(--border-color);
    background: var(--background-card);
}

.badge-link:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-md);
}

/* ===================
   RESPONSIVE DESIGN
   =================== */
@media (max-width: 1024px) {
    .hero-content {
        grid-template-columns: 1fr;
        gap: var(--spacing-lg);
        text-align: center;
    }
    
    .hero-image img {
        margin: 0 auto;
        max-width: 320px;
    }
    
    .intro {
        margin-left: auto;
        margin-right: auto;
    }
    
    .hero-buttons {
        justify-content: center;
    }
}

@media (max-width: 768px) {
    :root {
        --spacing-xl: 3rem;
    }
    
    .section-title {
        font-size: 2.25rem;
    }
    
    .hero-text h1 {
        font-size: 2.75rem;
    }
    
    .tagline {
        font-size: 1.25rem;
    }
    
    .hero-buttons {
        flex-direction: column;
    }
    
    .btn {
        width: 100%;
    }
}

@media (max-width: 480px) {
    .section-title {
        font-size: 2rem;
    }
    
    .hero-text h1 {
        font-size: 2.25rem;
    }
    
    .hero-image img {
        max-width: 260px;
    }
}

/* ===================
   DARK MODE
   =================== */
@media (prefers-color-scheme: dark) {
    :root {
        --text-color: #f1f5f9;
        --text-light: #cbd5e1;
        --text-muted: #94a3b8;
        --background: #0f172a;
        --background-alt: #1e293b;
        --background-card: #1e293b;
        --border-color: #334155;
    }
    
    body::before {
        background: 
            radial-gradient(circle at 20% 50%, rgba(79, 70, 229, 0.06) 0%, transparent 50%),
            radial-gradient(circle at 80% 80%, rgba(6, 182, 212, 0.06) 0%, transparent 50%);
    }
    
    .navbar {
        background: rgba(15, 23, 42, 0.95);
    }
    
    .nav-menu {
        background: rgba(30, 41, 59, 0.98);
    }
}

/* ===================
   ACCESSIBILITY
   =================== */
@media (prefers-reduced-motion: reduce) {
    *,
    *::before,
    *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
}

*:focus-visible {
    outline: 2px solid var(--primary-color);
    outline-offset: 2px;
}

::selection {
    background: var(--primary-color);
    color: white;
}

/* Scroll Reveal Animation */
.scroll-reveal {
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.6s ease-out, transform 0.6s ease-out;
}

.scroll-reveal.revealed {
    opacity: 1;
    transform: translateY(0);
}

/* Ripple Effect */
.ripple-effect {
    position: absolute;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.6);
    transform: scale(0);
    animation: ripple 0.6s ease-out;
    pointer-events: none;
}

@keyframes ripple {
    to {
        transform: scale(4);
        opacity: 0;
    }
}

/* Social Section */
.social-section {
    margin-top: var(--spacing-xl);
    padding-top: var(--spacing-lg);
    border-top: 1px solid var(--border-color);
}

.social-section h2 {
    font-size: 2rem;
    font-weight: 700;
    text-align: center;
    margin-bottom: var(--spacing-md);
    color: var(--text-color);
}
