# Ex02 Commercial Website
## Date: 11.03.2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">BrandName</div>
            <div class="nav-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#services">Services</a>
                <a href="#testimonials">Testimonials</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <div class="hero-text">
                <h1>Elevate Your Business</h1>
                <p>Discover our innovative solutions and take your business to the next level with our expert services.</p>
                <a href="#contact" class="cta-button">Get Started</a>
            </div>
            <div class="hero-image">
                <img src="https://images.pexels.com/photos/3184416/pexels-photo-3184416.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="Business Image">
            </div>
        </div>
    </section>

    <section class="about" id="about">
        <div class="about-content">
            <div class="about-text">
                <h2>About Us</h2>
                <p>At BrandName, we're passionate about helping businesses thrive. With years of experience and a dedicated team, we provide tailored solutions that drive success. Our mission is to empower our clients with innovative strategies and exceptional service.</p>
            </div>
            <div class="about-image">
                <img src="https://images.pexels.com/photos/933964/pexels-photo-933964.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="About Image">
            </div>
        </div>
    </section>

    <section class="services" id="services">
        <div class="services-container">
            <h2>Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <h3>Consulting</h3>
                    <p>Expert guidance to optimize your business operations and strategy.</p>
                </div>
                <div class="service-card">
                    <h3>Development</h3>
                    <p>Custom software and web solutions to meet your unique needs.</p>
                </div>
                <div class="service-card">
                    <h3>Marketing</h3>
                    <p>Effective digital marketing campaigns to boost your brand.</p>
                </div>
                <div class="service-card">
                    <h3>Support</h3>
                    <p>24/7 support to ensure your business runs smoothly.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="testimonials" id="testimonials">
        <div class="testimonials-container">
            <h2>What Our Clients Say</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p>"BrandName transformed our business with their innovative solutions. Highly recommended!"</p>
                    <p class="author">Jane Doe, CEO</p>
                </div>
                <div class="testimonial-card">
                    <p>"Their team is professional, responsive, and truly cares about our success."</p>
                    <p class="author">John Smith, Founder</p>
                </div>
                <div class="testimonial-card">
                    <p>"The best investment we made for our business growth!"</p>
                    <p class="author">Emily Brown, Marketing Director</p>
                </div>
            </div>
        </div>
    </section>

    <section class="contact" id="contact">
        <div class="contact-container">
            <div class="contact-info">
                <h2>Contact Us</h2>
                <p>Email: info@brandname.com</p>
                <p>Phone: (123) 456-7890</p>
                <p>Address: 123 Business Ave, City, Country</p>
            </div>
            <div class="contact-form">
                <h2>Send a Message</h2>
                <form>
                    <input type="text" placeholder="Your Name" required>
                    <input type="email" placeholder="Your Email" required>
                    <textarea placeholder="Your Message" required></textarea>
                    <button type="submit">Send</button>
                </form>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-content">
            <div class="footer-text">
                <p>© 2025 BrandName. All rights reserved.</p>
            </div>
            <div class="footer-links">
                <a href="#privacy">Privacy Policy</a>
                <a href="#terms">Terms of Service</a>
                <a href="#contact">Contact Us</a>
            </div>
        </div>
    </footer>
</body>
</html>
```


style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

header {
    background-color: #2c3e50;
    color: white;
    padding: 1rem;
    position: sticky;
    top: 0;
    z-index: 100;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
}

.nav-links {
    display: flex;
    gap: 2rem;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-size: 1rem;
}

.nav-links a:hover {
    color: #3498db;
}

.hero {
    background-color: #f1f1f1;
    padding: 4rem 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
}

.hero-content {
    max-width: 1200px;
    display: flex;
    gap: 2rem;
    align-items: center;
}

.hero-text {
    flex: 1;
}

.hero-text h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.hero-text p {
    font-size: 1.1rem;
    margin-bottom: 1.5rem;
    color: #555;
}

.cta-button {
    background-color: #3498db;
    color: white;
    padding: 0.8rem 1.5rem;
    text-decoration: none;
    border-radius: 5px;
    display: inline-block;
}

.cta-button:hover {
    background-color: #2980b9;
}

.hero-image {
    flex: 1;
}

.hero-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

.about {
    padding: 4rem 1rem;
    background-color: #fff;
    display: flex;
    justify-content: center;
}

.about-content {
    max-width: 1200px;
    display: flex;
    gap: 2rem;
    align-items: center;
}

.about-text {
    flex: 1;
}

.about-text h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
}

.about-text p {
    font-size: 1rem;
    color: #555;
    line-height: 1.6;
}

.about-image {
    flex: 1;
}

.about-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

.services {
    padding: 4rem 1rem;
    background-color: #f9f9f9;
    display: flex;
    justify-content: center;
}

.services-container {
    max-width: 1200px;
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

.services-container h2 {
    font-size: 2rem;
    text-align: center;
    margin-bottom: 2rem;
}

.services-grid {
    display: flex;
    gap: 2rem;
    flex-wrap: wrap;
}

.service-card {
    flex: 1;
    min-width: 250px;
    padding: 1.5rem;
    border: 1px solid #ddd;
    border-radius: 10px;
    text-align: center;
    background-color: white;
}

.service-card h3 {
    margin-bottom: 1rem;
}

.service-card p {
    color: #555;
}

.testimonials {
    padding: 4rem 1rem;
    background-color: #fff;
    display: flex;
    justify-content: center;
}

.testimonials-container {
    max-width: 1200px;
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

.testimonials-container h2 {
    font-size: 2rem;
    text-align: center;
    margin-bottom: 2rem;
}

.testimonial-grid {
    display: flex;
    gap: 2rem;
    flex-wrap: wrap;
}

.testimonial-card {
    flex: 1;
    min-width: 250px;
    padding: 1.5rem;
    border: 1px solid #ddd;
    border-radius: 10px;
    background-color: #f9f9f9;
}

.testimonial-card p {
    font-style: italic;
    color: #555;
    margin-bottom: 1rem;
}

.testimonial-card .author {
    font-weight: bold;
    color: #333;
}

.contact {
    padding: 4rem 1rem;
    background-color: #f1f1f1;
    display: flex;
    justify-content: center;
}

.contact-container {
    max-width: 1200px;
    display: flex;
    gap: 2rem;
    flex-wrap: wrap;
}

.contact-info {
    flex: 1;
    min-width: 250px;
}

.contact-info h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
}

.contact-info p {
    color: #555;
    margin-bottom: 1rem;
}

.contact-form {
    flex: 1;
    min-width: 250px;
}

.contact-form h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
}

.contact-form form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.contact-form input,
.contact-form textarea {
    padding: 0.8rem;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 1rem;
}

.contact-form textarea {
    resize: vertical;
    min-height: 100px;
}

.contact-form button {
    background-color: #3498db;
    color: white;
    padding: 0.8rem;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
}

.contact-form button:hover {
    background-color: #2980b9;
}

footer {
    background-color: #2c3e50;
    color: white;
    padding: 2rem 1rem;
    margin-top: auto;
}

.footer-content {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
}

.footer-links a {
    color: white;
    text-decoration: none;
    margin-left: 1rem;
}

.footer-links a:hover {
    color: #3498db;
}

@media (max-width: 768px) {
    .hero-content,
    .about-content,
    .contact-container {
        flex-direction: column;
        text-align: center;
    }

    .nav-links {
        flex-direction: column;
        gap: 1rem;
    }

    .services-grid,
    .testimonial-grid {
        flex-direction: column;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }

    .footer-links {
        margin-top: 1rem;
    }
}
```


## OUTPUT
Home
![Screenshot 2025-04-25 183423](https://github.com/user-attachments/assets/393bd5d9-ef30-4433-86bc-115bc05abfa6)

About
![Screenshot 2025-04-25 183429](https://github.com/user-attachments/assets/d2be0d81-cde0-458c-9b13-7872f098c908)

Services
![Screenshot 2025-04-25 183443](https://github.com/user-attachments/assets/d6d15fc5-4d19-4181-a3bb-7dabfb3e0624)

Review
![Screenshot 2025-04-25 183452](https://github.com/user-attachments/assets/fb345812-ea40-4e08-90ad-d029eb816a2a)

Contact
![Screenshot 2025-04-25 183459](https://github.com/user-attachments/assets/067b7d53-9c4d-4034-9524-97ec8206d4eb)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
