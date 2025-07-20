# Responsive-Design-Implementation

Project Overview:
This project is a responsive web design prototype created using Figma. It showcases a clean, modern UI layout suitable for websites.

Purpose:
The goal of this design was to:-
- Practice UI/UX skills using Figma
- Create a responsive layout adaptable to different screen sizes
- Focus on visual hierarchy, alignment, typography, and color usage

Design Principles Used:
- Responsive layout structure
- Consistent spacing and alignment
- Balanced color palette
- Modern and readable typography

Link- https://www.figma.com/design/ZXX4iBa0At4oOxYrhKFtL7/Untitled?t=zkAHJGCnayZpWGM0-1

HTML Code-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Pixel Beauty</title>
  <link rel="stylesheet" href="style.css"/>
</head>
<body>

  <header class="navbar">
    <div class="logo">
      <span class="pink">pixel</span><span class="black">Beauty</span>
    </div>
    <nav class="nav-links">
      <a href="#">Home</a> |
      <a href="#">About Us</a> |
      <a href="#">Shop</a> |
      <a href="#">Contact Us</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Glow Naturally with Pixel Beauty</h1>
    <p>
      Skincare that loves you back. Discover our range of clean, cruelty-free beauty products made with gentle, effective ingredients.
    </p>
    <button class="shop-btn">Shop Now</button>
  </section>

</body>
</html>

CSS Code-
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background-color: #f8e9f4;
  color: #000;
}

/* Navbar */
.navbar {
  background-color: #f9cbe3;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  flex-wrap: wrap;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
}

.pink {
  color: #d843d8;
  font-style: italic;
}

.black {
  color: #000;
}

.nav-links {
  font-size: 1rem;
  text-align: right;
}

.nav-links a {
  text-decoration: none;
  color: black;
  margin: 0 0.4rem;
}

/* Hero Section - Full Screen Background Image */
.hero {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;

  height: 100vh;
  padding: 2rem;

  background-image: url('https://raketcontent.com/small_1000003418_090cca8218.jpg');
  background-size: cover;              
  background-position: center center;  
  background-repeat: no-repeat;
  background-color: #f8e9f4;
}

.hero h1 {
  font-size: 2.5rem;
  color: #d843d8;
  margin-bottom: 1rem;
  font-weight: bold;
}

.hero p {
  font-size: 1.1rem;
  max-width: 600px;
  margin-bottom: 2rem;
  color: #000;
}

.shop-btn {
  padding: 0.8rem 1.5rem;
  background-color: #e8d7df;
  border: none;
  font-weight: bold;
  cursor: pointer;
  font-size: 1rem;
  box-shadow: 2px 2px 6px rgba(0,0,0,0.2);
  transition: 0.3s;
}

.shop-btn:hover {
  background-color: #dcbfd2;
}

/* Responsive Design */
@media screen and (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  .nav-links {
    margin-top: 1rem;
    text-align: left;
  }

  .hero h1 {
    font-size: 2rem;
  }

  .hero p {
    font-size: 1rem;
  }

  .shop-btn {
    font-size: 0.95rem;
  }
}
