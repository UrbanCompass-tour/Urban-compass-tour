<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Urban Compass Tour LLC</title>
    <link rel="stylesheet" href="./css/travel.css">
    <style>
        /* Include the cleaned up and corrected CSS here (already in your original file) */
    


/* RESET & BASE STYLES */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', sans-serif;
    line-height: 1.6;
    background-color: #f8f9fa;
    color: #333;
}

a {
    text-decoration: none;
}

/* HEADER */
.header {
    background-color: #fff;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 999;
    padding: 1rem 2rem;
}

.header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
    font-weight: bold;
    color:rgba(59, 107, 221, 0.879);
    font-size: 1.5rem;
}

.nav {
    display: flex;
    gap: 1.5rem;
}

.nav-links {
    color: #333;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav-links:hover {
    color: #ff6347;
}

.contact-button {
    background-color: #ff6347;
    color: #fff;
    padding: 0.6rem 1rem;
    border-radius: 5px;
    transition: background 0.3s ease;
}

.contact-button:hover {
    background-color: #e5533f;
}

.menu-button {
    display: none;
    background: none;
    border: none;
    cursor: pointer;
}

.menu-icon {
    width: 30px;
}

/* MAIN SECTION */
.main-section {
    display: flex;
    flex-wrap: wrap;
    padding: 4rem 2rem;
    align-items: center;
    justify-content: space-between;
    gap: 2rem;
    background: linear-gradient(135deg, #FF6347, #1E90FF);
    border-radius: 10px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

.content-left {
    flex: 1;
    animation: slideInLeft 1.2s ease;
}

.section-label {
    color: #ff6347;
    font-weight: 600;
    margin-bottom: 0.5rem;
}

.section-title {
    font-size: 2.8rem;
    font-weight: bold;
    margin-bottom: 1rem;
}

.section-description {
    font-size: 1.1rem;
    max-width: 600px;
    margin-bottom: 2rem;
}

.button-group a {
    padding: 0.8rem 1.5rem;
    margin-right: 1rem;
    background-color: #ff6347;
    color: #fff;
    border-radius: 5px;
    transition: transform 0.3s ease;
}

.button-group a:hover {
    transform: scale(1.05);
}

.content-right {
    flex: 1;
    display: flex;
    justify-content: center;
    animation: slideInRight 1.2s ease;
}

.section-image {
    max-width: 100%;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}

/* ANIMATIONS */
@keyframes slideInLeft {
    0% {
        opacity: 0;
        transform: translateX(-50%);
    }
    100% {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes slideInRight {
    0% {
        opacity: 0;
        transform: translateX(100%);
    }
    100% {
        opacity: 1;
        transform: translateX(0);
    }
}

/* GALLERY STYLES */
.image-gallery {
    padding: 4rem 2rem;
    background-color: #f9f9f9;
    text-align: center;
}

.gallery-title {
    font-size: 2rem;
    margin-bottom: 2rem;
    color: #333;
}

.gallery-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 2rem;
}

.gallery-item {
    flex: 1;
    max-width: 300px;
    transform: scale(1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    opacity: 0;
    transform: translateY(50px);
}

.gallery-item img {
    width: 100%;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.gallery-item h3 {
    margin-top: 1rem;
    color: #555;
}

/* Hover Zoom Effect */
.gallery-item:hover img {
    transform: scale(1.05);
}

/* Scroll Animation */
.gallery-item.visible {
    opacity: 1;
    transform: translateY(0);
    transition: all 0.6s ease-in-out;
}

/* Base Styles */
.site-footer {
    background-color: #1a1a1a;
    color: #fff;
    padding: 40px 20px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.footer-container {
    display: flex;
    flex-direction: column;
    gap: 30px;
}

.footer-column {
    flex: 1;
}

.footer-logo {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 10px;
}

.footer-description,
.footer-heading,
.footer-links,
.footer-column p {
    font-size: 14px;
    line-height: 1.6;
}

.footer-links {
    list-style: none;
    padding: 0;
}

.footer-links li {
    margin-bottom: 8px;
}

.footer-links a {
    color: #fff;
    text-decoration: none;
}

.footer-links a:hover {
    text-decoration: underline;
}

.map-responsive {
    overflow: hidden;
    padding-top: 56.25%;
    position: relative;
    height: 0;
}

.map-responsive iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
}

.footer-bottom {
    border-top: 1px solid #444;
    margin-top: 30px;
    padding-top: 20px;
    text-align: center;
}

.footer-social a {
    margin: 0 10px;
    color: #fff;
    text-decoration: none;
}

.footer-social a:hover {
    text-decoration: underline;
}

/* Large Screens */
@media (min-width: 768px) {
    .footer-container {
        flex-direction: row;
        justify-content: space-between;
    }

    .footer-column {
        margin-right: 20px;
    }

    .footer-column:last-child {
        margin-right: 0;
    }

    .footer-bottom {
        display: flex;
        justify-content: space-between;
        align-items: center;
        text-align: left;
        padding: 20px;
    }
}

 .map-responsive {
  position: relative;
  
  overflow: hidden;
  padding-bottom: 56.25%; /* 16:9 ratio */
  height: 0;
  margin-top: 1rem;
}

.map-responsive iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
@media only screen and (min-width: 480px) and (max-width: 767px) {
  .site-footer {
    padding: 20px;
    text-align: center;
  }

  .footer-container {
    flex-direction: column;
    align-items: center;
  }

  .footer-column {
    width: 100%;
    margin-bottom: 20px;
  }

  .footer-logo {
    font-size: 1.8rem;
  }

  .footer-heading {
    font-size: 1.2rem;
    margin-bottom: 10px;
  }

  .footer-links li {
    margin: 5px 0;
  }

  .map-responsive iframe {
    width: 100%;
    height: 300px;
  }

  .footer-social {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin-top: 15px;
  }

  .footer-copy {
    font-size: 0.9rem;
    margin-top: 10px;
  }
}


@media (max-width: 768px) {
  .nav {
    display: none !important; /* Ensures it hides unless .show is applied */
  }
}
@media (max-width: 768px) {
  .logo {
    flex-direction: column;
    align-items: flex-start;
    font-size: 1.2rem;
  }

  .logo img {
    width: 60px;
  }
}


/* MEDIA QUERIES */
@media (max-width: 768px) {
    .main-section {
        flex-direction: column;
        text-align: center;
    }

    .nav {
        display: none;
        flex-direction: column;
        width: 100%;
        margin-top: 1rem;
        background-color: #fff;
        padding: 1rem;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .nav.show {
        display: flex;
    }

    .menu-button {
        display: block;
    }

    .button-group a {
        display: block;
        margin: 0.5rem auto;
        width: 70%;
    }

    .section-title {
        font-size: 2rem;
    }

   .gallery-grid {
  padding: 0 1rem;
}

.gallery-item img {
  width: 100%;
  height: auto;
}


    .footer-container {
        flex-direction: column;
        text-align: center;
    }

    .footer-column {
        text-align: center;
    }

    /* Ensure the hero image is responsive */
    .content-right img {
        max-width: 100%;
    }
}

@media (max-width: 480px) {
 
    
  .main-section {
    padding: 2rem 1rem;
  }

  .section-title {
    font-size: 1.6rem;
  }

  .section-description {
    font-size: 0.95rem;
  }

  .button-group a {
    width: 100%;
    margin: 0.5rem 0;
  }


    .section-description {
        font-size: 1rem;
    }

    .gallery-item {
        max-width: 90%;
    }

    .footer-copy {
        font-size: 0.8rem;
    }
} 
    
   


/* I will keep it minimal here for clarity. Assume it includes the previously posted correct styles. */
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="header-content">
            <a href="#" class="logo">
                <img src="./logo.logo.com.png" alt="Urban Compass Logo" width="80">
                <div>
                    Muhammad Hazik Riyan<br>
                    Urban Compass Tour LLC
                </div>
            </a>
            <nav class="nav" id="navMenu">
                <a href="#home" class="nav-links">Home</a>
                <a href="#gallery" class="nav-links">Gallery</a>
                <a href="#tours" class="nav-links">Tours</a>
                <a href="#about" class="nav-links">About</a>
            </nav>
            <a href="#contact" class="contact-button">Contact Us</a>
            <button class="menu-button" id="menuToggle">
                <img src="https://img.icons8.com/ios-filled/50/000000/menu--v1.png" alt="Menu" class="menu-icon">
            </button>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="main-section" id="home">
        <div class="content-left">
            <p class="section-label">Discover the World with Us</p>
            <h1 class="section-title">Your Journey Begins Here</h1>
            <p class="section-description">
                Explore breathtaking destinations with our expert travel guidance.
                Whether you seek adventure, relaxation, or cultural experiences, we make it easy.
            </p>
            <div class="button-group">
                <a href="#start">Start Tour</a>
                <a href="#tours">Take Tour</a>
            </div>
        </div>
        <div class="content-right">
            <img src="./GqRKuOEW0AAPzDv.jpg" alt="Travel destination" class="section-image">
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="image-gallery" id="gallery">
        <h2 class="gallery-title">Owner of Travel and Tour</h2>
        <div class="gallery-grid">
            <div class="gallery-item animate">
                <img src="./w.jpg" alt="Owner Photo 1">
            </div>
            <div class="gallery-item animate">
                <img src="./Ha.jpg" alt="Owner Photo 2">
            </div>
            <div class="gallery-item animate">
                <img src="./h.jpg" alt="Owner Photo 3">
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="site-footer" id="contact">
        <div class="footer-container">
            <div class="footer-column">
                <h2 class="footer-logo">Travel & Tour</h2>
                <p class="footer-description">
                    Explore the world with guided tours and unforgettable experiences.
                </p>
            </div>
            <div class="footer-column">
                <h3 class="footer-heading">Quick Links</h3>
                <ul class="footer-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#tours">Tours</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
            <div class="footer-column">
                <h3 class="footer-heading">Contact Us</h3>
                <p><strong>Email:</strong> urbancompasstour@gmail.com</p>
                <p><strong>Phone:</strong> +971 564897862</p>
                <p><strong>Address:</strong> Building 11, Office 14, Persia Cluster, Al Qusais, Dubai, UAE</p>
                <p><strong>Office Hours:</strong> Mon–Fri (Open), Sat–Sun (Closed)</p>
                <div class="map-responsive">
                   <center>
                     <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d28863.873830493478!2d55.36192306708753!3d25.271115970427807!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3e5f5c35d410acf3%3A0xe8aff9f4de65bf11!2sAl%20Qusais%20-%20Dubai%20-%20United%20Arab%20Emirates!5e0!3m2!1sen!2s!4v1747185695412!5m2!1sen!2s" width="800" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                   </center>
</div>

                
            </div>
             <!-- Scripts -->
    <script>
        const menuToggle = document.getElementById('menuToggle');
        const navMenu = document.getElementById('navMenu');

        menuToggle.addEventListener('click', () => {
            navMenu.classList.toggle('show');
        });

        const animatedItems = document.querySelectorAll('.gallery-item');
        const showOnScroll = () => {
            animatedItems.forEach(item => {
                const rect = item.getBoundingClientRect();
                if (rect.top < window.innerHeight - 100) {
                    item.classList.add('visible');
                }
            });
        };
        window.addEventListener('scroll', showOnScroll);
        window.addEventListener('load', showOnScroll);
    </script>
        </div>
        <div class="footer-bottom">
            <div class="footer-social">
                <a href="https://maps.app.goo.gl/5qzTgzxYpbcyVxrd6">View Location</a>
                <a href="#">Instagram</a>
                <a href="#">Twitter</a>
            </div>
            <p class="footer-copy">&copy; 2025 Urban Compass Tour LLC. All rights reserved.</p>
        </div>
    </footer>

   
</body>
</html>
