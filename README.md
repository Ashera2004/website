# Ex.07 Restaurant Website
# Date: 3/05/2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
home.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shahi Darbaar - Authentic Indian Cuisine</title>
    <style>
        
        :root {
            --turmeric: #e6b325;      
            --paprika: #a83232;       
            --cardamom: #536455;      
            --cinnamon: #8b4513;      
            --cream: #f8f0e3;        
            --black-pepper: #2a2a2a;  
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background-color: var(--cream);
            color: var(--black-pepper);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--cream);
            padding: 20px 0;
            text-align: center;
        }

        .logo {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .logo img {
            width: 100px;
            height: auto;
            margin-right: 15px;
        }

        .logo h1 {
            color: var(--cardamom);
            font-size: 2.5rem;
            letter-spacing: 2px;
            font-weight: bold;
        }

        /* Navigation */
        nav {
            background-color: var(--black-pepper);
            padding: 15px 0;
        }

        nav ul {
            display: flex;
            justify-content: space-around;
            list-style-type: none;
            max-width: 960px;
            margin: 0 auto;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            padding: 10px 15px;
            transition: all 0.3s ease;
        }

        nav a:hover {
            color: var(--turmeric);
        }

        /* Hero Banner */
        .hero {
            color: white;
            text-align: left;
            padding: 100px 20px;
            position: relative;
        }

        .hero img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
        }

        .hero-content {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--turmeric);
        }

        .hero p {
            font-size: 1.1rem;
            margin-bottom: 30px;
        }

        /* Features Section */
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin: 50px 0;
        }

        .feature-box {
            flex-basis: 30%;
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            margin-bottom: 30px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .feature-box img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .feature-content {
            padding: 20px;
        }

        .feature-content h3 {
            color: var(--paprika);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }

        .feature-content p {
            margin-bottom: 15px;
            color: var(--black-pepper);
        }

        .hours-list {
            list-style: none;
        }

        .hours-list li {
            margin-bottom: 5px;
        }

        .cta-button {
            display: inline-block;
            background-color: var(--paprika);
            color: white;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 4px;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }

        .cta-button:hover {
            background-color: var(--cinnamon);
        }

        /* Footer */
        footer {
            background-color: var(--cardamom);
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 50px;
        }

        .footer-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .logo-small {
            width: 50px;
            height: auto;
            margin-bottom: 10px;
        }

        .divider {
            height: 2px;
            background-color: var(--turmeric);
            margin: 40px 0;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">
                <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo">
                <h1>SHAHI DARBAAR</h1>
            </div>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact-us.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <section class="hero">
            <img src="\static\background.jpg" alt="Hero Background">
            <div class="hero-content">
                <h2>30% Off This Weekend</h2>
                <p>Experience the royal flavors of India with our weekend special offer. Indulge in authentic dishes prepared with traditional spices and techniques handed down through generations. Our chefs create each dish with passion and precision to bring you the true taste of Indian royalty.</p>
            </div>
        </section>

        <div class="container">
            <div class="features">
                <div class="feature-box">
                    <img src="\static\new_menu_items.jpg" alt="New Menu Items">
                    <div class="feature-content">
                        <h3>Our New Menu</h3>
                        <p>Experience our newly curated menu featuring authentic dishes from across the Indian subcontinent. Every dish is carefully prepared using traditional methods and the finest spices to bring you the royal flavors of India.</p>
                        <a href="menu.html" class="cta-button">See our new menu</a>
                    </div>
                </div>

                <div class="feature-box">
                    <img src="\static\book_table.jpg" alt="Book a Table">
                    <div class="feature-content">
                        <h3>Book a table</h3>
                        <p>Reserve your royal dining experience at Shahi Darbaar. Our elegant ambiance combined with exceptional service ensures a memorable meal for you and your loved ones. Book in advance to secure your preferred time and seating.</p>
                        <a href="contact-us.html" class="cta-button">Book your table now</a>

                    </div>
                </div>

                <div class="feature-box">
                    <img src="\static\opening_hour.jpg" alt="Opening Hours">
                    <div class="feature-content">
                        <h3>Opening Hours</h3>
                        <p>We welcome you to experience our royal hospitality during these hours:</p>
                        <ul class="hours-list">
                            <li>Mon - Sun: 9am - 8pm</li>
                            
                        </ul>
                    </div>
                </div>
            </div>

            <div class="divider"></div>
        </div>
    </main>

    <footer>
        <div class="footer-content">
            <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo" class="logo-small">
            <p>Designed and Developed by A S Siddarth (2122204040316)</p>
        </div>
    </footer>
</body>
</html>

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu - Shahi Darbaar</title>
    <style>
        
        :root {
            --turmeric: #e6b325;      
            --paprika: #a83232;       
            --cardamom: #536455;      
            --cinnamon: #8b4513;      
            --cream: #f8f0e3;         
            --black-pepper: #2a2a2a;  
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background-color: var(--cream);
            color: var(--black-pepper);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--cream);
            padding: 20px 0;
            text-align: center;
        }

        .logo {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .logo img {
            width: 100px;
            height: auto;
            margin-right: 15px;
        }

        .logo h1 {
            color: var(--cardamom);
            font-size: 2.5rem;
            letter-spacing: 2px;
            font-weight: bold;
        }

        /* Navigation */
        nav {
            background-color: var(--black-pepper);
            padding: 15px 0;
        }

        nav ul {
            display: flex;
            justify-content: space-around;
            list-style-type: none;
            max-width: 960px;
            margin: 0 auto;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            padding: 10px 15px;
            transition: all 0.3s ease;
        }

        nav a:hover {
            color: var(--turmeric);
        }

        /* Page Title */
        .page-title {
            text-align: center;
            margin: 50px 0 30px;
            color: var(--paprika);
        }

        .page-title h2 {
            font-size: 3rem;
            position: relative;
            display: inline-block;
        }

        .page-title h2:after {
            content: '';
            position: absolute;
            width: 100px;
            height: 3px;
            background-color: var(--turmeric);
            left: 50%;
            bottom: -15px;
            transform: translateX(-50%);
        }

        /* Menu Categories */
        .menu-categories {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
        }

        .category-btn {
            background-color: var(--cardamom);
            color: white;
            border: none;
            padding: 10px 20px;
            margin: 0 10px;
            cursor: pointer;
            border-radius: 4px;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .category-btn:hover, .category-btn.active {
            background-color: var(--paprika);
        }

        /* Menu Items */
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            margin-bottom: 50px;
        }

        .menu-item {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .menu-item:hover {
            transform: translateY(-5px);
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .menu-item-content {
            padding: 20px;
        }

        .menu-item-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
            align-items: center;
        }

        .menu-item-title {
            color: var(--cinnamon);
            font-size: 1.3rem;
        }

        .menu-item-price {
            color: var(--paprika);
            font-weight: bold;
            font-size: 1.2rem;
        }

        .menu-item-desc {
            color: var(--black-pepper);
            margin-bottom: 15px;
        }

        .spice-level {
            display: flex;
            align-items: center;
        }

        .spice-level span {
            margin-right: 5px;
            color: var(--cinnamon);
            font-weight: bold;
        }

        .spice-icon {
            color: var(--paprika);
            font-size: 1.2rem;
            margin-right: 3px;
        }

        .dietary-info {
            display: flex;
            margin-top: 10px;
        }

        .dietary-tag {
            background-color: var(--cardamom);
            color: white;
            padding: 3px 8px;
            border-radius: 4px;
            font-size: 0.8rem;
            margin-right: 5px;
        }

        /* Footer */
        footer {
            background-color: var(--cardamom);
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 50px;
        }

        .footer-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .logo-small {
            width: 50px;
            height: auto;
            margin-bottom: 10px;
        }

        /* Hide filtered items */
        .menu-item.hidden {
            display: none;
        }

        /* No Results Message */
        .no-results {
            grid-column: 1 / -1;
            text-align: center;
            padding: 50px;
            font-size: 1.5rem;
            color: var(--paprika);
            display: none;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">
                <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo">
                <h1>SHAHI DARBAAR</h1>
            </div>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact-us.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <div class="container">
            <div class="page-title">
                <h2>Our Royal Menu</h2>
            </div>

            <div class="menu-categories">
                <button class="category-btn active" data-category="all">All</button>
                <button class="category-btn" data-category="appetizers">Appetizers</button>
                <button class="category-btn" data-category="main-course">Main Course</button>
                <button class="category-btn" data-category="breads">Breads</button>
                <button class="category-btn" data-category="desserts">Desserts</button>
            </div>

            <div class="menu-grid">
                <div class="no-results">No menu items found in this category.</div>

                <!-- Menu Item 1 -->
                <div class="menu-item" data-category="main-course">
                    <img src="\static\butter chicken.webp" alt="Butter Chicken">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Butter Chicken</h3>
                            <div class="menu-item-price">₹469</div>
                        </div>
                        <p class="menu-item-desc">Tender chicken pieces marinated in yogurt and spices, cooked in a creamy tomato sauce with butter.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 2 -->
                <div class="menu-item" data-category="main-course">
                    <img src="\static\chicken briyani.jpg" alt="Biryani">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Chicken Biryani</h3>
                            <div class="menu-item-price">₹370</div>
                        </div>
                        <p class="menu-item-desc">Fragrant basmati rice cooked with tender chicken pieces, saffron, and aromatic spices in the traditional dum style.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 3 -->
                <div class="menu-item" data-category="main-course">
                    <img src="\static\palak-paneer.jpg" alt="Palak Paneer">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Palak Paneer</h3>
                            <div class="menu-item-price">₹300</div>
                        </div>
                        <p class="menu-item-desc">Cubes of fresh cottage cheese cooked in a creamy spinach gravy flavored with cumin and garlic.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 4 -->
                <div class="menu-item" data-category="appetizers">
                    <img src="\static\chicken tikka.jpg" alt="Chicken Tikka">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Chicken Tikka</h3>
                            <div class="menu-item-price">₹190</div>
                        </div>
                        <p class="menu-item-desc">Boneless chicken chunks marinated in yogurt and spices, skewered and grilled in a tandoor oven.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 5 -->
                <div class="menu-item" data-category="main-course">
                    <img src="\static\Amritsari-Chole-Bhature.jpg" alt="Chole Bhature">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Chole Bhature</h3>
                            <div class="menu-item-price">₹225</div>
                        </div>
                        <p class="menu-item-desc">Spicy chickpea curry served with deep-fried leavened bread, a popular North Indian dish.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 6 -->
                <div class="menu-item" data-category="breads">
                    <img src="\static\garlic-naan.jpg" alt="Naan">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Garlic Naan</h3>
                            <div class="menu-item-price">₹85</div>
                        </div>
                        <p class="menu-item-desc">Leavened flatbread topped with garlic, baked in a tandoor oven until golden and fluffy.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">-</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 7 -->
                <div class="menu-item" data-category="main-course">
                    <img src="\static\Rogan-Josh.jpg" alt="Rogan Josh">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Rogan Ghosht</h3>
                            <div class="menu-item-price">₹485</div>
                        </div>
                        <p class="menu-item-desc">Traditional Kashmiri lamb curry cooked with Kashmiri red chillies, aromatic spices, and yogurt.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 8 -->
                <div class="menu-item" data-category="appetizers">
                    <img src="\static\samosa 1.jpg" alt="Samosa">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Vegetable Samosa</h3>
                            <div class="menu-item-price">₹40</div>
                        </div>
                        <p class="menu-item-desc">Crispy pastry filled with a spiced mixture of potatoes, peas, and herbs, deep-fried to perfection.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 9 -->
                <div class="menu-item" data-category="desserts">
                    <img src="\static\gulab-jamun.jpeg" alt="Gulab Jamun">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Gulab Jamun</h3>
                            <div class="menu-item-price">₹50</div>
                        </div>
                        <p class="menu-item-desc">Soft, spongy milk solids dumplings soaked in rose and cardamom flavored sugar syrup.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">-</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 10 -->
                <div class="menu-item" data-category="main-course">
                    <img src="\static\Best-Malai-Kofta.jpg" alt="Malai Kofta">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Malai Kofta</h3>
                            <div class="menu-item-price">₹390</div>
                        </div>
                        <p class="menu-item-desc">Soft cottage cheese and vegetable dumplings in a rich, creamy tomato gravy with cashews and spices.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 11 -->
                <div class="menu-item" data-category="appetizers">
                    <img src="\static\tandori chicken.jpg" alt="Tandoori Chicken">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Tandoori Chicken</h3>
                            <div class="menu-item-price">₹785</div>
                        </div>
                        <p class="menu-item-desc">Chicken marinated in yogurt and spices, grilled in a tandoor oven until charred and juicy.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">🌶️</span>
                            <span class="spice-icon">🌶️</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>

                <!-- Menu Item 12 -->
                <div class="menu-item" data-category="desserts">
                    <img src="\static\rasmalai.jpg" alt="Rasmalai">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Rasmalai</h3>
                            <div class="menu-item-price">₹200</div>
                        </div>
                        <p class="menu-item-desc">Soft cottage cheese dumplings soaked in sweetened, thickened milk flavored with cardamom and saffron.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">-</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                            <div class="dietary-tag">Gluten-Free</div>
                        </div>
                    </div>
                </div>
                
                <!-- Amritsari Kulcha -->
                <div class="menu-item" data-category="breads">
                    <img src="\static\amritsar kulcha.jpg" alt="Amritsari Kulcha">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Amritsari Kulcha</h3>
                            <div class="menu-item-price">₹215</div>
                        </div>
                        <p class="menu-item-desc">Stuffed bread with spiced mashed potatoes, onions, and herbs, cooked in a tandoor and brushed with butter.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">-</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

                <!-- Gobi Paratha -->
                <div class="menu-item" data-category="breads">
                    <img src="\static\gobi-paratha.jpg" alt="Gobi Paratha">
                    <div class="menu-item-content">
                        <div class="menu-item-header">
                            <h3 class="menu-item-title">Gobi Paratha</h3>
                            <div class="menu-item-price">₹129</div>
                        </div>
                        <p class="menu-item-desc">Whole wheat flatbread stuffed with spiced grated cauliflower, cooked on a griddle with ghee or butter.</p>
                        <div class="spice-level">
                            <span>Spice Level:</span>
                            <span class="spice-icon">-</span>
                        </div>
                        <div class="dietary-info">
                            <div class="dietary-tag">Vegetarian</div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </main>

    <footer>
        <div class="footer-content">
            <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo" class="logo-small">
            <p>Designed and Developed by A S Siddarth (212224040316)</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Get all category buttons and menu items
            const categoryButtons = document.querySelectorAll('.category-btn');
            const menuItems = document.querySelectorAll('.menu-item');
            const noResultsMessage = document.querySelector('.no-results');

            // Add click event to each category button
            categoryButtons.forEach(button => {
                button.addEventListener('click', function() {
                    // Remove active class from all buttons
                    categoryButtons.forEach(btn => btn.classList.remove('active'));
                    
                    // Add active class to clicked button
                    this.classList.add('active');
                    
                    // Get the category from data attribute
                    const category = this.getAttribute('data-category');
                    
                    // Filter menu items
                    filterMenuItems(category);
                });
            });

            // Function to filter menu items based on category
            function filterMenuItems(category) {
                let visibleCount = 0;
                
                menuItems.forEach(item => {
                    // Get the category of the item
                    const itemCategory = item.getAttribute('data-category');
                    
                    // Show all items if 'all' is selected or show only items matching the selected category
                    if (category === 'all' || itemCategory === category) {
                        item.classList.remove('hidden');
                        visibleCount++;
                    } else {
                        item.classList.add('hidden');
                    }
                });
                
                
                if (visibleCount === 0) {
                    noResultsMessage.style.display = 'block';
                } else {
                    noResultsMessage.style.display = 'none';
                }
            }
        });
    </script>
</body>
</html>

administration.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration - Shahi Darbaar</title>
    <style>
       
        :root {
            --turmeric: #e6b325;      
            --paprika: #a83232;       
            --cardamom: #536455;      
            --cinnamon: #8b4513;     
            --cream: #f8f0e3;         
            --black-pepper: #2a2a2a;  
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background-color: var(--cream);
            color: var(--black-pepper);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--cream);
            padding: 20px 0;
            text-align: center;
        }

        .logo {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .logo img {
            width: 100px;
            height: auto;
            margin-right: 15px;
        }

        .logo h1 {
            color: var(--cardamom);
            font-size: 2.5rem;
            letter-spacing: 2px;
            font-weight: bold;
        }

        /* Navigation */
        nav {
            background-color: var(--black-pepper);
            padding: 15px 0;
        }

        nav ul {
            display: flex;
            justify-content: space-around;
            list-style-type: none;
            max-width: 960px;
            margin: 0 auto;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            padding: 10px 15px;
            transition: all 0.3s ease;
        }

        nav a:hover {
            color: var(--turmeric);
        }

        /* Page Title */
        .page-title {
            text-align: center;
            margin: 50px 0 30px;
            color: var(--paprika);
        }

        .page-title h2 {
            font-size: 3rem;
            position: relative;
            display: inline-block;
        }

        .page-title h2:after {
            content: '';
            position: absolute;
            width: 100px;
            height: 3px;
            background-color: var(--turmeric);
            left: 50%;
            bottom: -15px;
            transform: translateX(-50%);
        }

        /* Team Section */
        .team-intro {
            text-align: center;
            max-width: 800px;
            margin: 0 auto 50px;
            color: var(--cardamom);
            font-size: 1.1rem;
        }

        .team-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            margin-bottom: 50px;
        }

        .team-member {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
            text-align: center;
        }

        .team-member:hover {
            transform: translateY(-5px);
        }

        .team-member img {
            width: 100%;
            height: 300px;
            object-fit: cover;
        }

        .team-member-content {
            padding: 20px;
        }

        .team-member-name {
            color: var(--cinnamon);
            font-size: 1.5rem;
            margin-bottom: 5px;
        }

        .team-member-title {
            color: var(--paprika);
            font-weight: bold;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }

        .team-member-bio {
            color: var(--black-pepper);
            margin-bottom: 15px;
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 10px;
        }

        .social-link {
            color: var(--cardamom);
            font-size: 1.2rem;
            transition: color 0.3s ease;
        }

        .social-link:hover {
            color: var(--paprika);
        }

        /* Mission Section */
        .mission-section {
            background-color: var(--cardamom);
            color: white;
            padding: 60px 0;
            margin: 30px 0;
        }

        .mission-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .mission-content h3 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: var(--turmeric);
        }

        .mission-content p {
            font-size: 1.1rem;
            margin-bottom: 20px;
        }

        /* Footer */
        footer {
            background-color: var(--cardamom);
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 50px;
        }

        .footer-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .logo-small {
            width: 50px;
            height: auto;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">
                <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo">
                <h1>SHAHI DARBAAR</h1>
            </div>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact-us.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <div class="container">
            <div class="page-title">
                <h2>Our Royal Team</h2>
            </div>

            <div class="team-intro">
                <p>At Shahi Darbaar, our team of culinary experts and hospitality professionals work diligently to bring you the authentic taste of royal Indian cuisine. Each member brings their passion and expertise to create an unforgettable dining experience.</p>
            </div>

            <div class="team-grid">
                <!-- Team Member 1 -->
                <div class="team-member">
                    <img src="\static\Rajesh Kumar.jpg" alt="Rajesh Kumar">
                    <div class="team-member-content">
                        <h3 class="team-member-name">Rajesh Kumar</h3>
                        <div class="team-member-title">Executive Chef</div>
                        <p class="team-member-bio">With over 20 years of experience in royal Indian kitchens, Chef Rajesh brings authentic flavors and traditional cooking techniques to Shahi Darbaar. His expertise in spice blending and tandoor cooking has earned him numerous culinary awards.</p>
                        
                    </div>
                </div>

                <!-- Team Member 2 -->
                <div class="team-member">
                    <img src="\static\priya singh.jpg" alt="Priya Singh">
                    <div class="team-member-content">
                        <h3 class="team-member-name">Priya Singh</h3>
                        <div class="team-member-title">Restaurant Manager</div>
                        <p class="team-member-bio">Priya ensures that every guest receives royal treatment at Shahi Darbaar. Her background in luxury hospitality and attention to detail creates a seamless dining experience from reservation to farewell.</p>
                        
                    </div>
                </div>

                <!-- Team Member 3 -->
                <div class="team-member">
                    <img src="\static\vikram joshi.jpg" alt="Vikram Joshi">
                    <div class="team-member-content">
                        <h3 class="team-member-name">Vikram Joshi</h3>
                        <div class="team-member-title">Pastry Chef</div>
                        <p class="team-member-bio">Specializing in traditional Indian sweets with a modern twist, Chef Vikram's desserts are the perfect ending to your royal feast. His unique creations blend authentic flavors with artistic presentation.</p>
                        
                    </div>
                </div>

                <!-- Team Member 4 -->
                <div class="team-member">
                    <img src="\static\ananya desai.jpg" alt="Ananya Desai">
                    <div class="team-member-content">
                        <h3 class="team-member-name">Ananya Desai</h3>
                        <div class="team-member-title">Marketing Director</div>
                        <p class="team-member-bio">Ananya brings Shahi Darbaar's royal experience to the digital world. Her creative campaigns and community engagement initiatives have made our restaurant a beloved culinary destination.</p>
                        
                    </div>
                </div>

                <!-- Team Member 5 -->
                <div class="team-member">
                    <img src="\static\arjun sharma.jpg" alt="Arjun Sharma">
                    <div class="team-member-content">
                        <h3 class="team-member-name">Arjun Sharma</h3>
                        <div class="team-member-title">Head Tandoor Chef</div>
                        <p class="team-member-bio">Master of the tandoor oven, Chef Arjun creates perfectly charred breads and succulent kebabs. His precision and timing bring out the authentic smoky flavors that define north Indian cuisine.</p>
                        
                    </div>
                </div>

                <!-- Team Member 6 -->
                <div class="team-member">
                    <img src="\static\meera kapoor.jpg" alt="Meera Kapoor">
                    <div class="team-member-content">
                        <h3 class="team-member-name">Meera Kapoor</h3>
                        <div class="team-member-title">Events Coordinator</div>
                        <p class="team-member-bio">From intimate family celebrations to grand corporate events, Meera ensures every special occasion at Shahi Darbaar exceeds expectations with her meticulous planning and creative touches.</p>
                        
                    </div>
                </div>
            </div>
        </div>

        <div class="mission-section">
            <div class="mission-content">
                <h3>Our Royal Mission</h3>
                <p>At Shahi Darbaar, we are committed to preserving and sharing the rich culinary heritage of royal Indian kitchens. Our mission is to transport our guests to the grand courts of Indian royalty through authentic flavors, elegant ambiance, and exceptional service.</p>
                <p>We source the finest ingredients, use traditional cooking methods, and honor time-tested recipes while incorporating contemporary sensibilities to create a dining experience that is both authentic and accessible.</p>
            </div>
        </div>
    </main>

    <footer>
        <div class="footer-content">
            <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo" class="logo-small">
            <p>Designed and Developed by A S Siddarth (212224040316)</p>
        </div>
    </footer>
</body>
</html>

contact-us.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us - Shahi Darbaar</title>
    <style>
        
        :root {
            --turmeric: #e6b325;      
            --paprika: #a83232;       
            --cardamom: #536455;      
            --cinnamon: #8b4513;      
            --cream: #f8f0e3;         
            --black-pepper: #2a2a2a;  
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background-color: var(--cream);
            color: var(--black-pepper);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--cream);
            padding: 20px 0;
            text-align: center;
        }

        .logo {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .logo img {
            width: 100px;
            height: auto;
            margin-right: 15px;
        }

        .logo h1 {
            color: var(--cardamom);
            font-size: 2.5rem;
            letter-spacing: 2px;
            font-weight: bold;
        }

        /* Navigation */
        nav {
            background-color: var(--black-pepper);
            padding: 15px 0;
        }

        nav ul {
            display: flex;
            justify-content: space-around;
            list-style-type: none;
            max-width: 960px;
            margin: 0 auto;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            padding: 10px 15px;
            transition: all 0.3s ease;
        }

        nav a:hover {
            color: var(--turmeric);
        }

        /* Page Title */
        .page-title {
            text-align: center;
            margin: 50px 0 30px;
            color: var(--paprika);
        }

        .page-title h2 {
            font-size: 3rem;
            position: relative;
            display: inline-block;
        }

        .page-title h2:after {
            content: '';
            position: absolute;
            width: 100px;
            height: 3px;
            background-color: var(--turmeric);
            left: 50%;
            bottom: -15px;
            transform: translateX(-50%);
        }

        /* Contact Section */
        .contact-section {
            display: flex;
            flex-wrap: wrap;
            margin: 50px 0;
            gap: 30px;
        }

        .contact-info {
            flex: 1;
            min-width: 300px;
            padding: 30px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .contact-info h3 {
            color: var(--cinnamon);
            font-size: 1.5rem;
            margin-bottom: 20px;
            border-bottom: 2px solid var(--turmeric);
            padding-bottom: 10px;
        }

        .contact-detail {
            display: flex;
            align-items: flex-start;
            margin-bottom: 20px;
        }

        .contact-icon {
            color: var(--paprika);
            font-size: 1.5rem;
            margin-right: 15px;
            min-width: 30px;
        }

        .contact-text h4 {
            color: var(--cardamom);
            margin-bottom: 5px;
        }

        .contact-text p, .contact-text a {
            color: var(--black-pepper);
            text-decoration: none;
        }

        .contact-text a:hover {
            color: var(--paprika);
        }

        .operating-hours {
            margin-top: 30px;
        }

        .operating-hours h4 {
            color: var(--cinnamon);
            margin-bottom: 15px;
        }

        .hours-list {
            list-style: none;
        }

        .hours-list li {
            margin-bottom: 5px;
            display: flex;
            justify-content: space-between;
        }

        .day {
            font-weight: bold;
            color: var(--cardamom);
        }

        /* Contact Form */
        .contact-form {
            flex: 1;
            min-width: 300px;
            padding: 30px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .contact-form h3 {
            color: var(--cinnamon);
            font-size: 1.5rem;
            margin-bottom: 20px;
            border-bottom: 2px solid var(--turmeric);
            padding-bottom: 10px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            color: var(--cardamom);
            margin-bottom: 8px;
            font-weight: bold;
        }

        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
            transition: border-color 0.3s ease;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--turmeric);
        }

        textarea.form-control {
            resize: vertical;
            min-height: 120px;
        }

        .submit-btn {
            background-color: var(--paprika);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 4px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .submit-btn:hover {
            background-color: var(--cinnamon);
        }

        /* Map Section */
        .map-section {
            margin: 50px 0;
        }

        .map-container {
            height: 400px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        /* Footer */
        footer {
            background-color: var(--cardamom);
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 50px;
        }

        .footer-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .logo-small {
            width: 50px;
            height: auto;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">
                <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo">
                <h1>SHAHI DARBAAR</h1>
            </div>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="home.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact-us.html">Contact Us</a></li>
        </ul>
    </nav>

    <main>
        <div class="container">
            <div class="page-title">
                <h2>Contact Us</h2>
            </div>

            <div class="contact-section">
                <div class="contact-info">
                    <h3>Reach Out To Us</h3>
                    
                    <div class="contact-detail">
                        <div class="contact-icon">📍</div>
                        <div class="contact-text">
                            <h4>Our Location</h4>
                            <p>64/B</p>
                            <p>CG Employees Colony</p>
                            <p>Mayuri Nagar, Miyapur</p>
                            <p>Hyderabad, Telangana 500049</p>
                        </div>
                    </div>
                    
                    <div class="contact-detail">
                        <div class="contact-icon">📞</div>
                        <div class="contact-text">
                            <h4>Phone</h4>
                            <p><a href="tel:+15551234567">+1 (555) 123-4567</a></p>
                            <p><a href="tel:+15559876543">+1 (555) 987-6543</a> (Reservations)</p>
                        </div>
                    </div>
                    
                    <div class="contact-detail">
                        <div class="contact-icon">📧</div>
                        <div class="contact-text">
                            <h4>Email</h4>
                            <p><a href="mailto:info@shahidarbaar.com">info@shahidarbaar.com</a></p>
                            <p><a href="mailto:reservations@shahidarbaar.com">reservations@shahidarbaar.com</a></p>
                        </div>
                    </div>
                    
                    <div class="contact-detail">
                        <div class="contact-icon">🌐</div>
                        <div class="contact-text">
                            <h4>Social Media</h4>
                            <p><a href="#">Facebook</a></p>
                            <p><a href="#">Instagram</a></p>
                            <p><a href="#">Twitter</a></p>
                        </div>
                    </div>
                    
                    <div class="operating-hours">
                        <h4>Operating Hours</h4>
                        <ul class="hours-list">
                            <li><span class="day">Monday - Sunday:</span> <span>9:00 AM - 08:00 PM</span></li>
                            
                        </ul>
                    </div>
                </div>
                
                <div class="contact-form">
                    <h3>Send Us a Message</h3>
                    <form>
                        <div class="form-group">
                            <label for="name">Your Name</label>
                            <input type="text" id="name" class="form-control" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="email">Email Address</label>
                            <input type="email" id="email" class="form-control" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" class="form-control">
                        </div>
                        
                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <input type="text" id="subject" class="form-control" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="message">Your Message</label>
                            <textarea id="message" class="form-control" required></textarea>
                        </div>
                        
                        <button type="submit" class="submit-btn">Send Message</button>
                    </form>
                </div>
            </div>
            
            <div class="map-section">
                <div class="map-container">
                    <img src="\static\map.png" alt="Map Location of Shahi Darbaar" style="width: 100%; height: 100%; object-fit: cover;">
                </div>
            </div>
        </div>
    </main>

    <footer>
        <div class="footer-content">
            <img src="\static\restaurent_logo.jpg" alt="Shahi Darbaar Logo" class="logo-small">
            <p>Designed and Developed by A S Siddarth (212224040316)</p>
        </div>
    </footer>
</body>
</html>
```
# OUTPUT:

![alt text](<Screenshot 2025-05-06 215631.png>)

![alt text](<Screenshot 2025-05-06 220107.png>)

![alt text](<Screenshot 2025-05-06 220118.png>)

![alt text](<Screenshot 2025-05-06 220126.png>)

![alt text](<Screenshot 2025-05-06 214926.png>)

![alt text](<Screenshot 2025-05-06 215357.png>)
# RESULT:

The program for designing software company website using HTML and CSS is completed successfully.
