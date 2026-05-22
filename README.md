# queens-of-chnages
a simple web page using html and css



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Queens Of Change Foundation</title>
    <style>
        /* --- SIMPLE LIGHT STYLES --- */
        
        /* Color Palette */
        :root {
            --bg-light: #fff5f7;      /* Very light pink/white */
            --bg-white: #ffffff;
            --text-dark: #444444;
            --text-light: #666666;
            --accent: #e91e63;       /* Soft pink */
            --accent-light: #fce4ec;
            --border: #f0f0f0;
        }

        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* --- HEADER --- */
        header {
            background-color: var(--bg-white);
            padding: 1rem 2rem;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--accent);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1100px;
            margin: 0 auto;
        }

        nav ul {
            display: flex;
            gap: 1.5rem;
            list-style: none;
        }

        nav a {
            color: var(--text-light);
            font-size: 0.95rem;
        }

        nav a:hover {
            color: var(--accent);
        }

        /* --- HERO SECTION --- */
        .hero {
            background-color: var(--bg-white);
            padding: 4rem 2rem;
            text-align: center;
        }

        .hero h1 {
            font-size: 2.5rem;
            color: var(--accent);
            margin-bottom: 0.5rem;
        }

        .tagline {
            font-size: 1.2rem;
            color: var(--text-light);
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 12px 30px;
            border-radius: 25px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            background-color: #c2185b;
            transform: scale(1.05);
        }

        /* --- ABOUT SECTION --- */
        .about {
            padding: 4rem 2rem;
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .about h2 {
            color: var(--accent);
            margin-bottom: 1rem;
        }

        .about p {
            color: var(--text-light);
            margin-bottom: 1.5rem;
        }

        /* --- IMAGE SECTION --- */
        .image-section {
            padding: 2rem;
            text-align: center;
            background-color: var(--bg-white);
        }

        .image-section img {
            max-width: 100%;
            width: 100%;
            max-height: 400px;
            object-fit: cover;
            border-radius: 10px;
        }

        /* --- FOOTER --- */
        footer {
            background-color: var(--bg-white);
            padding: 2rem;
            text-align: center;
            border-top: 1px solid var(--border);
        }

        footer p {
            color: var(--text-light);
            font-size: 0.9rem;
        }

        /* --- MOBILE RESPONSIVE --- */
        @media (max-width: 600px) {
            .hero h1 {
                font-size: 1.8rem;
            }
            
            nav ul {
                display: none;
            }
            
            .logo {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <nav>
            <div class="logo">Queens Of Change</div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero">
        <h1>Queens Of Change Foundation</h1>
        <p class="tagline">Empowering Women. Building Communities. Creating Change.</p>
        <a href="#contact" class="btn">Volunteer With Us</a>
    </section>

    <!-- ABOUT SECTION -->
    <section class="about" id="about">
        <h2>Who We Are</h2>
        <p>
            Queens Of Change is a non-profit organization dedicated to uplifting women 
            in under-resourced communities. We believe every woman deserves the 
            opportunity to succeed.
        </p>
        <p>
            Through mentorship, education, and community support, we help women 
            transform their lives and build a better future for themselves and their families.
        </p>
    </section>

    <!-- IMAGE SECTION -->
    <section class="image-section">
        <!-- Using a free placeholder image -->
        <img src="https://images.unsplash.com/photo-1529070538774-1843cb3265df?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" 
             alt="Community of women working together">
    </section>

    <!-- CONTACT / BUTTON SECTION -->
    <section class="about" id="contact">
        <h2>Get Involved</h2>
        <p>Join us in making a difference. Whether you want to volunteer, donate, or simply spread the word, your support matters.</p>
        <br>
        <a href="mailto:hello@queensofchange.org" class="btn">Donate Now</a>
    </section>

    <!-- FOOTER -->
    <footer>
        <p><strong>Queens Of Change Foundation</strong></p>
        <p>Making the world a better place, one woman at a time.</p>
        <br>
        <p>&copy; 2024 Queens Of Change. All rights reserved.</p>
    </footer>

</body>
</html>