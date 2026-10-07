/* ---------- Global Styles ---------- */

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.6;
    background-color: #f4f7fb;
    color: #1f2937;
}


/* ---------- Header ---------- */

.site-header {
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    color: white;
    padding: 1.5rem 5%;
}

.header-container {
    max-width: 1100px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    gap: 1rem;
}

.logo-link {
    display: flex;
    align-items: center;
}

.logo {
    width: 60px;
    height: 60px;
    object-fit: contain;
}

.header-content h1 {
    font-size: 2rem;
    margin-bottom: 0.2rem;
}

.header-content p {
    color: #bfdbfe;
}


/* ---------- Navigation ---------- */

nav {
    max-width: 1100px;
    margin: 1.5rem auto 0;
}

.nav-list {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
}

.nav-list a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    padding: 0.5rem 0.8rem;
    border-radius: 6px;
    transition: background-color 0.3s ease;
}

.nav-list a:hover,
.nav-list a:focus {
    background-color: #2563eb;
}


/* ---------- General Sections ---------- */

.section {
    padding: 5rem 5%;
}

.section-container {
    max-width: 1100px;
    margin: 0 auto;
}

.section h2 {
    text-align: center;
    color: #0f172a;
    font-size: 2rem;
    margin-bottom: 2.5rem;
}


/* ---------- About Section ---------- */

.about-section {
    background-color: white;
}

.about-section .section-container {
    display: flex;
    align-items: center;
    gap: 4rem;
}

.about-image {
    flex: 1;
    text-align: center;
}

.about-image img {
    width: 250px;
    height: 250px;
    object-fit: cover;
    border-radius: 50%;
    border: 6px solid #2563eb;
    box-shadow: 0 10px 30px rgba(15, 23, 42, 0.15);
}

.about-content {
    flex: 2;
}

.about-content h2 {
    text-align: left;
    margin-bottom: 1rem;
}

.about-content p {
    margin-bottom: 1rem;
}


/* ---------- Skills Section ---------- */

.skills-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.5rem;
}

.skill-card {
    background-color: white;
    padding: 1.5rem;
    border-radius: 10px;
    border-top: 4px solid #2563eb;
    box-shadow: 0 5px 15px rgba(15, 23, 42, 0.08);
    transition: transform 0.3s ease;
}

.skill-card:hover {
    transform: translateY(-5px);
}

.skill-card dt {
    font-weight: bold;
    font-size: 1.1rem;
    color: #1d4ed8;
    margin-bottom: 0.5rem;
}

.skill-card dd {
    color: #4b5563;
}


/* ---------- Projects Section ---------- */

.projects-section {
    background-color: white;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
}

.project-card {
    background-color: #f8fafc;
    padding: 2rem;
    border-radius: 12px;
    border: 1px solid #e2e8f0;
    box-shadow: 0 5px 15px rgba(15, 23, 42, 0.08);
    display: flex;
    flex-direction: column;
}

.project-card h3 {
    color: #1d4ed8;
    margin-bottom: 1rem;
}

.project-card p {
    flex-grow: 1;
    margin-bottom: 1.5rem;
}

.project-card a {
    color: #1d4ed8;
    font-weight: bold;
    text-decoration: none;
}

.project-card a:hover,
.project-card a:focus {
    text-decoration: underline;
}


/* ---------- Contact Form ---------- */

.contact-form {
    max-width: 700px;
    margin: 0 auto;
    background-color: white;
    padding: 2rem;
    border-radius: 12px;
    box-shadow: 0 5px 20px rgba(15, 23, 42, 0.08);
}

.form-group {
    margin-bottom: 1.5rem;
}

.form-group label {
    display: block;
    font-weight: bold;
    margin-bottom: 0.5rem;
}

.form-group input,
.form-group textarea {
    width: 100%;
    padding: 0.8rem;
    border: 1px solid #cbd5e1;
    border-radius: 6px;
    font: inherit;
}

.form-group input:focus,
.form-group textarea:focus {
    outline: 2px solid #2563eb;
    border-color: #2563eb;
}

.contact-form button {
    border: none;
    background-color: #2563eb;
    color: white;
    padding: 0.8rem 1.5rem;
    border-radius: 6px;
    font-size: 1rem;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.contact-form button:hover {
    background-color: #1d4ed8;
}


/* ---------- Footer ---------- */

.site-footer {
    background-color: #0f172a;
    color: white;
    text-align: center;
    padding: 2rem;
}


/* =========================================
   Responsive Design
   ========================================= */


/* ---------- Tablet ---------- */

@media (max-width: 900px) {

    .skills-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .projects-grid {
        grid-template-columns: 1fr 1fr;
    }

    .about-section .section-container {
        gap: 2rem;
    }
}


/* ---------- Mobile ---------- */

@media (max-width: 600px) {

    .site-header {
        padding: 1.2rem 4%;
    }

    .header-container {
        flex-direction: column;
        text-align: center;
    }

    .header-content h1 {
        font-size: 1.6rem;
    }

    .nav-list {
        flex-direction: column;
        align-items: center;
        gap: 0.5rem;
    }

    .section {
        padding: 3rem 5%;
    }

    .about-section .section-container {
        flex-direction: column;
        text-align: center;
    }

    .about-content h2 {
        text-align: center;
    }

    .about-image img {
        width: 190px;
        height: 190px;
    }

    .skills-grid {
        grid-template-columns: 1fr;
    }

    .projects-grid {
        grid-template-columns: 1fr;
    }

    .contact-form {
        padding: 1.5rem;
    }
}
