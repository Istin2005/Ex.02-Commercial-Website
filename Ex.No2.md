# Ex02 Commercial Website
## Date:3-10-2025

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

## index.html
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brew Haven</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Navigation Bar -->
    <header>
        <nav class="navbar">
            <div class="logo">☕ Brew Haven</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#specials">Chef's Specials</a></li>
                <li><a href="#order">Order Online</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-text">
            <h1>Welcome to Brew Haven ❤️</h1>
            <p>Freshly brewed coffee & delightful treats every day!</p>
            <a href="#menu" class="btn explore-btn">🌟 Explore Menu 🌟</a>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="menu">
        <h2>Our Menu</h2>
        <div class="menu-grid">
            <div class="card">
                <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93" alt="Cappuccino">
                <h3>Cappuccino</h3>
                <p>Rich espresso with steamed milk foam.</p>
                <span>₹150</span>
            </div>
            <div class="card">
                <img src="https://media.istockphoto.com/id/147987270/photo/fresh-baked-croissants.jpg?s=612x612&w=0&k=20&c=7fEdqVxlvRK80hpGGEMGyw-_Cpi1ipb1D2rTim5yTuI= " alt="Croissant">
                <h3>Butter Croissant</h3>
                <p>Flaky and buttery, baked fresh daily.</p>
                <span>₹80</span>
            </div>
            <div class="card">
                <img src="https://encrypted-tbn3.gstatic.com/shopping?q=tbn:ANd9GcSO9mEacSFgIkZpWC3cu1OK_lgHTb_2sA2x05xORymWCLD4jxv30G_eyjhLPnMk3nVnK16pXtxR0cWP364G24HGd9FshwPk" alt="Cake">
                <h3>Chocolate Cake</h3>
                <p>Decadent and moist, a chocoholic’s dream.</p>
                <span>₹200</span>
            </div>
        </div>
    </section>

    <!-- Chef's Specials -->
    <section id="specials" class="specials">
        <h2>Chef's Specials</h2>
        <div class="specials-grid">
            <div class="card">
                <img src="https://images.unsplash.com/photo-1551024601-bec78aea704b" alt="Fruit Tart">
                <h3>Fruit Tart</h3>
                <p>Fresh seasonal fruits with creamy custard.</p>
            </div>
            <div class="card">
                <img src="https://www.ambitiouskitchen.com/wp-content/uploads/2022/12/No-Knead-Honey-Sunflower-Seed-Artisan-Bread-5.jpg" alt="Artisan Bread">
                <h3>Artisan Bread</h3>
                <p>Handmade, crusty, and full of flavor.</p>
            </div>
        </div>
    </section>

    <!-- Order Online -->
    <section id="order" class="order">
        <h2>Order Online</h2>
        <p>Enjoy our delicious treats from the comfort of your home.</p>
        <a href="#" class="btn">Start Ordering</a>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2025 Brew Haven | Designed by Istin</p>
        <p>📍 123 Coffee Lane, chennai, India</p>
        <p>📞 +91 9876543210 </p>
        <div class="social-links">
            <a href="#">Facebook</a> | 
            <a href="#">Instagram</a> | 
            <a href="#">Twitter</a>
        </div>
    </footer>
</body>
</html>

```

## style.css
```
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    color: #333;
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #4b2e05;
    padding: 15px 30px;
}
.logo {
    font-family: 'Playfair Display', serif;
    font-size: 26px;
    color: #fff;
}
.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}
.nav-links a {
    text-decoration: none;
    color: white;
    font-weight: 500;
    transition: 0.3s;
}
.nav-links a:hover {
    color: #ffcc99;
}

/* Hero */
.hero {
    height: 100vh;
    background: url('https://images.unsplash.com/photo-1509042239860-f550ce710b93') center/cover no-repeat;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}
.hero::before {
    content: "";
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(0, 0, 0, 0.45);
}
.hero-text {
    position: relative;
    z-index: 2;
    color: white;
    padding: 20px;
}
.hero-text h1 {
    font-size: 3.2rem;
    font-family: 'Playfair Display', serif;
    color: #f6e1b3;
    margin-bottom: 10px;
}
.hero-text p {
    font-size: 1.2rem;
    margin-bottom: 20px;
}
.explore-btn {
    background: linear-gradient(45deg, #ff7e5f, #feb47b);
    color: white;
    font-size: 1.2rem;
    font-weight: bold;
    padding: 15px 35px;
    border-radius: 50px;
    text-decoration: none;
    transition: all 0.3s ease;
}
.explore-btn:hover {
    transform: scale(1.1);
}

/* Cards */
.menu, .specials, .order {
    padding: 60px 20px;
    text-align: center;
}
.menu-grid, .specials-grid {
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap;
}
.card {
    background: #fff8f0;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    width: 250px;
    transition: transform 0.3s;
}
.card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
}
.card:hover {
    transform: scale(1.05);
}

/* Order Section */
.order {
    background: #fff0e6;
}

/* Footer */
footer {
    background: #4b2e05;
    color: white;
    text-align: center;
    padding: 20px;
}
.social-links a {
    color: #ffb266;
    text-decoration: none;
}
.social-links a:hover {
    color: #ffd9b3;
}
```

## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2b7f1d24-922a-457c-adfe-302d877de9cf" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9a3ac6bb-fb3f-462f-a8e7-d75b5f1228a7" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/836ce0d4-b8f7-4205-b1c9-8085ec16f528" />




## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
