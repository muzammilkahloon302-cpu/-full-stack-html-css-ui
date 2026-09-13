# -full-stack-html-css-ui
A clean, responsive multi-section website built with HTML and CSS, featuring a navbar, hero section, services, contact form, and professional UI styling.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>TechNova | Digital Solutions</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- ================= NAVBAR ================= -->

    <header>
        <nav class="navbar">

            <div class="logo">
                Tech<span>Nova</span>
            </div>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

        </nav>
    </header>


    <main>

        <!-- ================= HERO ================= -->

        <section id="home" class="hero">

            <div class="hero-content">

                <p class="tagline">DIGITAL SOLUTIONS FOR THE FUTURE</p>

                <h1>
                    Build Something
                    <span>Amazing</span>
                </h1>

                <p>
                    We create modern, responsive and user-friendly
                    digital experiences that help businesses grow.
                </p>

                <div class="hero-buttons">
                    <a href="#services" class="btn primary-btn">
                        Explore Services
                    </a>

                    <a href="#contact" class="btn secondary-btn">
                        Contact Us
                    </a>
                </div>

            </div>

        </section>


        <!-- ================= SERVICES ================= -->

        <section id="services" class="services">

            <div class="section-heading">

                <p>WHAT WE DO</p>

                <h2>Our Services</h2>

                <span>
                    Professional solutions designed for modern businesses.
                </span>

            </div>


            <div class="service-container">

                <!-- Service 1 -->

                <div class="service-card">

                    <div class="service-icon">
                        &lt;/&gt;
                    </div>

                    <h3>Web Development</h3>

                    <p>
                        We build responsive and modern websites
                        using clean and efficient technologies.
                    </p>

                    <a href="#contact">Learn More →</a>

                </div>


                <!-- Service 2 -->

                <div class="service-card">

                    <div class="service-icon">
                        ✦
                    </div>

                    <h3>UI/UX Design</h3>

                    <p>
                        Clean and intuitive interfaces designed
                        to provide an excellent user experience.
                    </p>

                    <a href="#contact">Learn More →</a>

                </div>


                <!-- Service 3 -->

                <div class="service-card">

                    <div class="service-icon">
                        ☁
                    </div>

                    <h3>Cloud Solutions</h3>

                    <p>
                        Scalable and reliable cloud solutions
                        for modern applications and businesses.
                    </p>

                    <a href="#contact">Learn More →</a>

                </div>

            </div>

        </section>


        <!-- ================= CONTACT ================= -->

        <section id="contact" class="contact">

            <div class="contact-wrapper">

                <div class="contact-info">

                    <p class="contact-label">GET IN TOUCH</p>

                    <h2>
                        Let's Build Something
                        <span>Great Together.</span>
                    </h2>

                    <p>
                        Have a project idea or want to learn more
                        about our services? Send us a message and
                        let's discuss your requirements.
                    </p>

                    <div class="contact-details">

                        <div>
                            <strong>Email</strong>
                            <p>hello@technova.com</p>
                        </div>

                        <div>
                            <strong>Phone</strong>
                            <p>+92 300 1234567</p>
                        </div>

                    </div>

                </div>


                <!-- Contact Form -->

                <form class="contact-form">

                    <label for="name">Your Name</label>

                    <input
                        type="text"
                        id="name"
                        placeholder="Enter your name"
                    >


                    <label for="email">Email Address</label>

                    <input
                        type="email"
                        id="email"
                        placeholder="Enter your email"
                    >


                    <label for="message">Message</label>

                    <textarea
                        id="message"
                        rows="5"
                        placeholder="Write your message..."
                    ></textarea>


                    <button type="submit">
                        Send Message
                    </button>

                </form>

            </div>

        </section>

    </main>


    <!-- ================= FOOTER ================= -->

    <footer>

        <div class="footer-content">

            <div class="logo">
                Tech<span>Nova</span>
            </div>

            <p>
                Creating digital experiences for the future.
            </p>

        </div>

        <p class="copyright">
            © 2026 TechNova. All Rights Reserved.
        </p>

    </footer>

</body>
</html>

/* =================================
   RESET & GLOBAL STYLES
================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #f8fafc;
    color: #172033;
    line-height: 1.6;
}

a {
    text-decoration: none;
}

ul {
    list-style: none;
}


/* =================================
   NAVBAR
================================= */

header {
    background: #ffffff;
    border-bottom: 1px solid #e5e7eb;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.navbar {
    max-width: 1150px;
    margin: auto;

    padding: 18px 25px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 25px;
    font-weight: 800;
    color: #172033;
}

.logo span {
    color: #2563eb;
}

.nav-links {
    display: flex;
    gap: 35px;
}

.nav-links a {
    color: #475569;
    font-size: 15px;
    font-weight: 600;

    transition: 0.3s;
}

.nav-links a:hover {
    color: #2563eb;
}


/* =================================
   HERO SECTION
================================= */

.hero {
    min-height: 650px;

    display: flex;
    justify-content: center;
    align-items: center;

    text-align: center;

    padding: 80px 25px;

    background:
        radial-gradient(
            circle at top right,
            #dbeafe,
            transparent 35%
        ),
        #f8fafc;
}

.hero-content {
    max-width: 850px;
}

.tagline {
    color: #2563eb;
    font-size: 13px;
    font-weight: 800;
    letter-spacing: 2px;

    margin-bottom: 20px;
}

.hero h1 {
    font-size: 62px;
    line-height: 1.1;
    margin-bottom: 25px;
}

.hero h1 span {
    color: #2563eb;
}

.hero-content > p:not(.tagline) {
    max-width: 650px;
    margin: auto;

    color: #64748b;
    font-size: 18px;
}

.hero-buttons {
    margin-top: 35px;

    display: flex;
    justify-content: center;
    gap: 15px;
}


/* =================================
   BUTTONS
================================= */

.btn {
    padding: 13px 27px;

    border-radius: 7px;

    font-weight: 700;

    transition: 0.3s;
}

.primary-btn {
    background: #2563eb;
    color: white;
}

.primary-btn:hover {
    background: #1d4ed8;
    transform: translateY(-3px);
}

.secondary-btn {
    border: 1px solid #cbd5e1;
    color: #334155;
    background: white;
}

.secondary-btn:hover {
    border-color: #2563eb;
    color: #2563eb;
    transform: translateY(-3px);
}


/* =================================
   SERVICES
================================= */

.services {
    padding: 100px 25px;

    background: white;
}

.section-heading {
    max-width: 700px;
    margin: auto;

    text-align: center;

    margin-bottom: 55px;
}

.section-heading p {
    color: #2563eb;

    font-size: 13px;
    font-weight: 800;

    letter-spacing: 2px;
}

.section-heading h2 {
    font-size: 40px;
    margin: 8px 0 12px;
}

.section-heading span {
    color: #64748b;
}


.service-container {
    max-width: 1100px;
    margin: auto;

    display: grid;
    grid-template-columns: repeat(3, 1fr);

    gap: 25px;
}

.service-card {
    padding: 35px;

    border: 1px solid #e5e7eb;
    border-radius: 12px;

    background: white;

    transition: 0.3s;
}

.service-card:hover {
    transform: translateY(-8px);

    border-color: #bfdbfe;

    box-shadow:
        0 15px 35px rgba(37, 99, 235, 0.12);
}

.service-icon {
    width: 55px;
    height: 55px;

    display: flex;
    justify-content: center;
    align-items: center;

    border-radius: 10px;

    background: #eff6ff;
    color: #2563eb;

    font-size: 22px;
    font-weight: bold;

    margin-bottom: 22px;
}

.service-card h3 {
    font-size: 21px;
    margin-bottom: 12px;
}

.service-card p {
    color: #64748b;
    margin-bottom: 20px;
}

.service-card a {
    color: #2563eb;
    font-weight: 700;

    transition: 0.3s;
}

.service-card a:hover {
    color: #1d4ed8;
}


/* =================================
   CONTACT
================================= */

.contact {
    padding: 100px 25px;

    background: #f1f5f9;
}

.contact-wrapper {
    max-width: 1100px;
    margin: auto;

    display: grid;

    grid-template-columns: 1fr 1fr;

    gap: 70px;
}

.contact-label {
    color: #2563eb;

    font-size: 13px;
    font-weight: 800;

    letter-spacing: 2px;
}

.contact-info h2 {
    font-size: 40px;
    line-height: 1.2;

    margin: 12px 0 20px;
}

.contact-info h2 span {
    color: #2563eb;
}

.contact-info > p {
    color: #64748b;
}

.contact-details {
    margin-top: 30px;
}

.contact-details div {
    margin-bottom: 18px;
}

.contact-details strong {
    color: #172033;
}

.contact-details p {
    color: #64748b;
}


/* =================================
   CONTACT FORM
================================= */

.contact-form {
    background: white;

    padding: 35px;

    border-radius: 12px;

    box-shadow:
        0 10px 30px rgba(0, 0, 0, 0.06);
}

.contact-form label {
    display: block;

    margin-bottom: 7px;

    font-size: 14px;
    font-weight: 600;
}

.contact-form input,
.contact-form textarea {
    width: 100%;

    padding: 13px;

    margin-bottom: 20px;

    border: 1px solid #cbd5e1;

    border-radius: 6px;

    font-family: inherit;

    outline: none;

    transition: 0.3s;
}

.contact-form input:focus,
.contact-form textarea:focus {
    border-color: #2563eb;

    box-shadow:
        0 0 0 3px #dbeafe;
}

.contact-form button {
    width: 100%;

    padding: 13px;

    border: none;
    border-radius: 7px;

    background: #2563eb;
    color: white;

    font-size: 15px;
    font-weight: 700;

    cursor: pointer;

    transition: 0.3s;
}

.contact-form button:hover {
    background: #1d4ed8;
    transform: translateY(-2px);
}


/* =================================
   FOOTER
================================= */

footer {
    background: #172033;
    color: #cbd5e1;

    padding: 35px 25px;

    text-align: center;
}

.footer-content {
    margin-bottom: 20px;
}

.footer-content .logo {
    color: white;
    margin-bottom: 8px;
}

.footer-content p {
    color: #94a3b8;
}

.copyright {
    padding-top: 20px;

    border-top: 1px solid #334155;

    color: #94a3b8;

    font-size: 13px;
}


/* =================================
   RESPONSIVE DESIGN
================================= */

@media (max-width: 800px) {

    .hero h1 {
        font-size: 45px;
    }

    .service-container {
        grid-template-columns: 1fr;
    }

    .contact-wrapper {
        grid-template-columns: 1fr;
        gap: 40px;
    }
}


@media (max-width: 600px) {

    .navbar {
        flex-direction: column;
        gap: 15px;
    }

    .nav-links {
        gap: 18px;
    }

    .hero {
        min-height: 600px;
    }

    .hero h1 {
        font-size: 36px;
    }

    .hero-buttons {
        flex-direction: column;
    }

    .btn {
        width: 100%;
    }

    .section-heading h2,
    .contact-info h2 {
        font-size: 32px;
    }

    .contact-form {
        padding: 25px;
    }
}



