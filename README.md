# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Layout</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <nav class="navbar">
      <div class="logo">MyWebsite</div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="content">
    <section id="home" class="hero">
      <h1>Welcome to MyWebsite</h1>
      <p>Your one-stop solution for awesome designs.</p>
    </section>

    <section id="about" class="about">
      <h2>About Us</h2>
      <p>We create beautiful, responsive designs tailored to your needs.</p>
    </section>

    <section id="services" class="services">
      <h2>Our Services</h2>
      <div class="service-items">
        <div class="service">Web Design</div>
        <div class="service">Development</div>
        <div class="service">SEO Optimization</div>
      </div>
    </section>

    <section id="contact" class="contact">
      <h2>Contact Us</h2>
      <p>Email us at contact@mywebsite.com</p>
    </section>
  </main>

  <footer class="footer">
    <p>&copy; 2025 MyWebsite. All rights reserved.</p>
  </footer>
</body>
</html>



/* General Styles */
body {
  margin: 0;
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

h1, h2 {
  margin-bottom: 10px;
}

p {
  margin: 0 0 10px;
}

a {
  text-decoration: none;
  color: #333;
}

ul {
  list-style: none;
  padding: 0;
}

/* Header & Navigation Bar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: #fff;
}

.navbar .logo {
  font-size: 1.5rem;
}

.nav-links {
  display: flex;
  gap: 20px;
}

.nav-links li {
  padding: 5px 10px;
}

.nav-links a {
  color: #fff;
}

.nav-links a:hover {
  text-decoration: underline;
}

/* Main Content */
.hero {
  text-align: center;
  padding: 50px;
  background-color: #f4f4f4;
}

.about, .services, .contact {
  padding: 20px;
  text-align: center;
}

.service-items {
  display: flex;
  justify-content: center;
  gap: 15px;
}

.service {
  background-color: #ddd;
  padding: 20px;
  border-radius: 5px;
  flex: 1;
  text-align: center;
}

/* Footer */
.footer {
  text-align: center;
  padding: 10px;
  background-color: #333;
  color: #fff;
}

/* Responsive Design */
@media (max-width: 768px) {
  .nav-links {
    flex-direction: column;
    gap: 10px;
  }

  .service-items {
    flex-direction: column;
  }
}

@media (max-width: 480px) {
  .hero {
    padding: 20px;
  }

  .service {
    padding: 10px;
  }
}
