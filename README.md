# Ex.07 Restaurant Website
## Date:10.12.2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
home.html
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Winged Majesty</title>
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Roboto:wght@300;400;500&family=Gloock&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: 'Roboto', sans-serif;
                margin: 0;
                padding: 0;
                background-color: #f8f8f8;
                color: #333;
            }
            .header {
                display: flex;
                justify-content: space-between;
                padding: 20px;
                background-color:black;
                color: white;
                align-items: center;
            }
            .logo h1 {
                margin: 0;
                font-family: 'Poppins', sans-serif;
                font-size: 20px;
            }
            .logo img {
                height: 40px;
                width: auto;
                margin-left: 10px;
            }
            .search-bar input {
                padding: 10px;
                width: 550px;
                border-radius: 20px;
                border: 2px solid #ccc;
                margin-left: 200px;
                font-size: 1.1em;
            }
            .search-bar button {
                padding: 10px;
                background-color: #f1c40f;
                border: none;
                cursor: pointer;
                border-radius: 5px;
                font-size: 1.1em;
                
            }
            .account span {
                margin: 0 8px;
                cursor: pointer;
                font-size: 20px;
            }
            .nav-container {
                background-color: #34495e;
                color: white;
                border-bottom: 3px solid #f1c40f;
            }
            .nav-menu ul {
                display: flex;
                justify-content: center;
                list-style: none;
                padding: 10px 0;
                margin: 0;
            }
            .nav-menu ul li {
                margin: 0 20px;
                cursor: pointer;
            }
            .nav-menu a {
                text-decoration: none;
                color: white;
                font-size: 1.2em;
            }
            .nav-menu ul li::after {
                content: "";
                display: block;
                width: 100%;
                height: 2px;
                background-color: #f1c40f;
                transform: scaleX(0);
               
            }
            .nav-menu ul li:hover::after {
                transform: scaleX(1);
            }
            .hero {
                text-align: center;
                padding: 50px 0;
                position: relative;
                background-color: #ecf0f1;
            }
            .banner video {
                width: 100%;
                height: auto;
                max-height: 500px;
                object-fit: cover;
            }
            .hero h2 {
                font-family: 'Gloock', sans-serif;
                font-size: 3em;
                color: #2c3e50;
                margin-top: 20px;
                text-transform: uppercase;
            }
            .cta-box {
                display: flex;
                justify-content: center;
                margin-top: 40px;
            }
            .cta-box .box {
                width: 300px;
                margin: 0 15px;
                background-color: #fff;
                padding: 30px;
                border-radius: 10px;
                text-align: center;
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
                border-top: 5px solid #f1c40f;
            }
            .cta-box img {
                width: 100%;
                border-radius: 10px;
                margin-bottom: 20px;
            }
            .cta-box h3 {
                font-family: 'Poppins', sans-serif;
                color: #2c3e50;
                margin-bottom: 15px;
            }
            .cta-box p {
                font-size: 1em;
                color: #7f8c8d;
            }
            footer {
                background-color: #2c3e50;
                color: white;
                padding: 20px 0;
                text-align: center;
            }
            footer a {
                color: #f1c40f;
                text-decoration: none;
                margin: 0 10px;
            }
            footer a:hover {
                text-decoration: underline;
            }
        </style>
    </head>
    <body>
        <header class="header">
            <div class="logo">
                <img src="logo.png" alt="logo">   
                <h1>Winged Majesty</h1>
                
            </div>
            <div class="search-bar">
                <input type="text" placeholder="Crown your appetite. Search now...">
                <button>Search</button>
            </div>
            <div class="account">
                <span><a href="signin.html">Hello Royalty, Sign in</a></span>
                <span><a href="orders.html">Orders</a></span>
                <span><a href="cart.html">Cart</a></span>
            </div>
        </header>
        <div class="nav-container">
            <nav class="nav-menu">
                <ul>
                   <li><a href="home.html">HOME</a></li> 
                   <li><a href="menu.html">MENU BOOK</a></li> 
                   <li><a href="admin.html">ADMINISTRATION</a></li> 
                   <li><a href="contact.html">CONTACT US</a></li> 
                </ul>
            </nav>
        </div>
        <main>
            <section class="hero">
                <div class="banner">
                    <video autoplay loop muted>
                        <source src="hero.mp4" type="video/mp4">
                    </video>
                </div>
                <h2>Comfort Your Crave</h2>
                <p>Soar to new heights of flavor and elegance with Winged Majesty where every bite is a royal experience.</p>
            </section>
            <section class="cta-box">
                <div class="box">
                    <img src="menu.png" alt="Our Menu">
                    <h3>OUR MENU</h3>
                    <p>Embark on a culinary journey through a menu designed to captivate and satisfy every royal appetite. From bold flavors to timeless classics, each dish is a masterpiece – thoughtfully curated to deliver an unforgettable dining experience, where every bite feels like a taste of royalty.</p>
                    <a href="menu.html">Discover More</a>
                </div>
                <div class="box">
                    <img src="table.png" alt="Book a Table">
                    <h3>BOOK A TABLE</h3>
                    <p>Reserve your seat at the royal table and experience dining like never before. Whether it's an intimate dinner or a grand celebration, let us create an unforgettable experience just for you. Book now and make your moment at Winged Majesty truly special.</p>
                    <a href="booking.html">Book Now</a>
                </div>
                <div class="box">
                    <img src="hours.png" alt="Opening Hours">
                    <h3>OPENING HOURS</h3>
                    <p>Our doors are always open to welcome you into a world of exquisite flavors. Whether it’s a midday craving or an evening indulgence, Winged Majesty is ready to serve you with passion and perfection – come join us during our royal hours and experience dining at its finest.</p>
                    <a href="hours.html">See Schedule</a>
                </div>
            </section>
            <footer>
                <p>Joseph C 2024 | <a href="privacy.html">Privacy Policy</a> | <a href="terms.html">Terms & Conditions</a></p>
            </footer>
    </body>
</html>
```
admin.html
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Administration - Winged Majesty</title>
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Roboto:wght@300;400;500&family=Gloock&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: 'Roboto', sans-serif;
                margin: 0;
                padding: 0;
                background-color: #f8f8f8;
                color: #333;
            }
            .header {
                display: flex;
                justify-content: space-between;
                padding: 20px;
                background-color: black;
                color: white;
                align-items: center;
            }
            .logo h1 {
                margin: 0;
                font-family: 'Poppins', sans-serif;
                font-size: 20px;
            }
            .logo img {
                height: 40px;
                width: auto;
                margin-left: 10px;
            }
            .nav-container {
                background-color: #34495e;
                color: white;
                border-bottom: 3px solid #f1c40f;
            }
            .nav-menu ul {
                display: flex;
                justify-content: center;
                list-style: none;
                padding: 10px 0;
                margin: 0;
            }
            .nav-menu ul li {
                margin: 0 20px;
                cursor: pointer;
            }
            .nav-menu a {
                text-decoration: none;
                color: white;
                font-size: 1.2em;
            }
            .menu-section {
                padding: 50px 0;
                text-align: center;
                background-color: #ecf0f1;
            }
            .admin-container {
                display: grid;
                grid-template-columns: repeat(3, 1fr);
                gap: 30px;
                padding: 50px;
            }
            .admin-member {
                background-color: #fff;
                padding: 20px;
                text-align: center;
                border-radius: 10px;
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            }
            .admin-member img {
                width: 150px;
                height: 150px;
                border-radius: 50%;
                object-fit: cover;
                margin-bottom: 20px;
            }
            .admin-member {
                background-color: #fff;
                padding: 20px;
                text-align: center;
                border-radius: 10px;
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
                border: 3px solid #f1c40f;  /* Adding a yellow border */
            }
            .admin-member h3 {
                font-family: 'Poppins', sans-serif;
                color: #2c3e50;
                margin-bottom: 10px;
            }
            .admin-member p {
                font-size: 1.1em;
                color: #7f8c8d;
            }
            footer {
                background-color: #2c3e50;
                color: white;
                padding: 20px 0;
                text-align: center;
            }
            footer a {
                color: #f1c40f;
                text-decoration: none;
                margin: 0 10px;
            }
            footer a:hover {
                text-decoration: underline;
            }
        </style>
    </head>
    <body>
        <header class="header">
            <div class="logo">
                <img src="logo.png" alt="logo">   
                <h1>Winged Majesty</h1>
            </div>
        </header>
        <div class="nav-container">
            <nav class="nav-menu">
                <ul>
                    <li><a href="home.html">HOME</a></li> 
                    <li><a href="menu.html">MENU BOOK</a></li> 
                    <li><a href="admin.html">ADMINISTRATION</a></li> 
                    <li><a href="contact.html">CONTACT US</a></li> 
                </ul>
            </nav>
        </div>
        <main>
            <section class="menu-section">
                <h2>Our Esteemed Administration Team</h2>
                <div class="admin-container">
                    <div class="admin-member">
                        <img src="ceo.png" alt="Person 1">
                        <h3>Joseph</h3>
                        <p>CEO & Founder</p>
                    </div>
                   
                    <div class="admin-member">
                        <img src="man.png" alt="Person 2">
                        <h3>Jack Daniel</h3>
                        <p>Restaurant Manager</p>
                    </div>
                    
                    <div class="admin-member">
                        <img src="assis.png" alt="Person 3">
                        <h3>Samuel Green</h3>
                        <p>Assistant Manager</p>
                    </div>
                    
                    <div class="admin-member">
                        <img src="chef.png" alt="Person 4">
                        <h3>Emily Clark</h3>
                        <p>Head Chef</p>
                    </div>
                   
                    <div class="admin-member">
                        <img src="head.png" alt="Person 5">
                        <h3>Michael Johnson</h3>
                        <p>Sous Chef</p>
                    </div>
                    
                    <div class="admin-member">
                        <img src="fin.png" alt="Person 6">
                        <h3>Alice Brown</h3>
                        <p>Financial Controller</p>
                    </div>
                </div>
            </section>
        </main>
        <footer>
            <p>Joseph C 2024 | <a href="privacy.html">Privacy Policy</a> | <a href="terms.html">Terms & Conditions</a></p>
        </footer>
    </body>
</html>
```
menu.html
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Menu - Winged Majesty</title>
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Roboto:wght@300;400;500&family=Gloock&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: 'Roboto', sans-serif;
                margin: 0;
                padding: 0;
                background-color: #f8f8f8;
                color: #333;
            }
            .header {
                display: flex;
                justify-content: space-between;
                padding: 20px;
                background-color: black;
                color: white;
                align-items: center;
            }
            .logo h1 {
                margin: 0;
                font-family: 'Poppins', sans-serif;
                font-size: 20px;
            }
            .logo img {
                height: 40px;
                width: auto;
                margin-left: 10px;
            }
            .search-bar input {
                padding: 10px;
                width: 550px;
                border-radius: 20px;
                border: 2px solid #ccc;
                margin-left: 200px;
                font-size: 1.1em;
            }
            .search-bar button {
                padding: 10px;
                background-color: #f1c40f;
                border: none;
                cursor: pointer;
                border-radius: 5px;
                font-size: 1.1em;
            }
            .account span {
                margin: 0 8px;
                cursor: pointer;
                font-size: 20px;
            }
            .nav-container {
                background-color: #34495e;
                color: white;
                border-bottom: 3px solid #f1c40f;
            }
            .nav-menu ul {
                display: flex;
                justify-content: center;
                list-style: none;
                padding: 10px 0;
                margin: 0;
            }
            .nav-menu ul li {
                margin: 0 20px;
                cursor: pointer;
            }
            .nav-menu a {
                text-decoration: none;
                color: white;
                font-size: 1.2em;
            }
            .nav-menu ul li::after {
                content: "";
                display: block;
                width: 100%;
                height: 2px;
                background-color: #f1c40f;
                transform: scaleX(0);
            }
            .nav-menu ul li:hover::after {
                transform: scaleX(1);
            }
            .menu-section {
                padding: 50px 0;
                text-align: center;
                background-color: #ecf0f1;
            }
            .menu-category {
                display: flex;
                justify-content: center;
                flex-wrap: wrap;
                gap: 20px;
            }
            .menu-item {
                width: 300px;
                margin: 15px;
                background-color: #fff;
                padding: 20px;
                border-radius: 10px;
                text-align: center;
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
                border-top: 5px solid #f1c40f;
            }
            .menu-item img {
                width: 100%;
                border-radius: 10px;
                margin-bottom: 20px;
            }
            .menu-item h3 {
                font-family: 'Poppins', sans-serif;
                color: #2c3e50;
                margin-bottom: 10px;
            }
            .menu-item p {
                font-size: 1.1em;
                color: #7f8c8d;
            }
            footer {
                background-color: #2c3e50;
                color: white;
                padding: 20px 0;
                text-align: center;
            }
            footer a {
                color: #f1c40f;
                text-decoration: none;
                margin: 0 10px;
            }
            footer a:hover {
                text-decoration: underline;
            }
        </style>
    </head>
    <body>
        <header class="header">
            <div class="logo">
                <img src="logo.png" alt="logo">   
                <h1>Winged Majesty</h1>
            </div>
            <div class="search-bar">
                <input type="text" placeholder="Search your favorite meal...">
                <button>Search</button>
            </div>
            <div class="account">
                <span><a href="signin.html">Hello Royalty, Sign in</a></span>
                <span><a href="orders.html">Orders</a></span>
                <span><a href="cart.html">Cart</a></span>
            </div>
        </header>
        <div class="nav-container">
            <nav class="nav-menu">
                <ul>
                    <li><a href="home.html">HOME</a></li> 
                    <li><a href="menu.html">MENU BOOK</a></li> 
                    <li><a href="admin.html">ADMINISTRATION</a></li> 
                    <li><a href="contact.html">CONTACT US</a></li> 
                </ul>
            </nav>
        </div>
        <main>
            <section class="menu-section">
                <h2>Our Exquisite Menu</h2>
                <p>Indulge in a variety of royal delicacies crafted to perfection. Select your favorites from our carefully curated menu.</p>

                <div class="menu-category">
                    <div class="menu-item">
                        <img src="burrito.png" alt="Dish 1">
                        <h3>BURRITO</h3>
                        <p>A golden tortilla wrapped around tender grilled meat or veggies, smoky beans, cilantro-lime rice, creamy guacamole, tangy salsa, and a dollop of sour cream. A bold, flavorful feast fit for the skies!</p>
                    </div>
                    <div class="menu-item">
                        <img src="burrito bowl.png" alt="Dish 2">
                        <h3>BURRITO BOWL</h3>
                        <p>A vibrant bowl of cilantro-lime rice, smoky beans, tender grilled meat or veggies, topped with creamy guacamole, tangy salsa, shredded cheese, and sour cream. A deconstructed delight soaring with flavor!</p>
                    </div>
                    <div class="menu-item">
                        <img src="lifestyle bowl.png" alt="Dish 3">
                        <h3>LIFESTYLE BOWL</h3>
                        <p>A wholesome blend of fresh greens, cilantro-lime rice, smoky beans, and your choice of lean grilled protein, topped with guacamole and salsa. A light, flavorful creation made for those on the go!</p>
                    </div>
                    <div class="menu-item">
                        <img src="quesadilla.png" alt="Dish 4">
                        <h3>QUESADILLA</h3>
                        <p>A golden, crispy tortilla filled with melted cheese, your choice of grilled meat or veggies, and topped with creamy guacamole and tangy salsa. A perfect balance of crunch and flavor, soaring with every bite!</p>
                    </div>
                    <div class="menu-item">
                        <img src="order.png" alt="Dish 5">
                        <h3>SALAD</h3>
                        <p>A fresh mix of crisp greens, vibrant veggies, and your choice of grilled protein, drizzled with tangy dressing and topped with creamy guacamole. Light, refreshing, and packed with flavor—perfect for every journey!</p>
                    </div>
                    <div class="menu-item">
                        <img src="three-tacos.png" alt="Dish 6">
                        <h3>TACOS</h3>
                        <p>Soft, warm tortillas filled with your choice of grilled meat or veggies, topped with fresh salsa, creamy guacamole, and a sprinkle of cheese. A burst of flavor in every bite, ready to take flight!</p>
                    </div>
                    <div class="menu-item">
                        <img src="kid meal.png" alt="Dish 7">
                        <h3>KID'S MEAL</h3>
                        <p>A fun, kid-friendly plate featuring a choice of soft taco, mini quesadilla, or crispy chicken tenders, paired with rice, beans, and a side of sweet salsa. Simple, tasty, and perfect for little adventurers!</p>
                    </div>
                    <div class="menu-item">
                        <img src="chips.png" alt="Dish 8">
                        <h3>CHIPS & SIDES</h3>
                        <p>Crispy tortilla chips served with a side of creamy guacamole, tangy salsa, or zesty queso. Perfect for dipping and snacking on your flight of flavor!</p>
                    </div>
                    <div class="menu-item">
                        <img src="drinks.png" alt="Dish 9">
                        <h3>DRINKS</h3>
                        <p>A refreshing selection of ice-cold beverages, from fizzy sodas to tangy lemonades, and chilled teas. The perfect companion to your flavorful journey!</p>
                    </div>
                </div>
            </section>
        </main>
        <footer>
            <p>Joseph C 2024 | <a href="privacy.html">Privacy Policy</a> | <a href="terms.html">Terms & Conditions</a></p>
        </footer>
    </body>
</html>
```
contact.html
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Contact Us - Winged Majesty</title>
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Roboto:wght@300;400;500&family=Gloock&display=swap" rel="stylesheet">
        <style>
            html, body {
                height: 100%;
                margin: 0;
                padding: 0;
                font-family: 'Roboto', sans-serif;
                background-color: #f8f8f8;
                color: #333;
            }
            body {
                display: flex;
                flex-direction: column;
            }
            main {
                flex: 1; 
                padding: 50px 20px;
                text-align: center;
                background-color: #ecf0f1;
            }
            .header {
                display: flex;
                justify-content: space-between;
                padding: 20px;
                background-color: black;
                color: white;
                align-items: center;
            }
            .logo h1 {
                margin: 0;
                font-family: 'Poppins', sans-serif;
                font-size: 20px;
            }
            .logo img {
                height: 40px;
                width: auto;
                margin-left: 10px;
            }
            .nav-container {
                background-color: #34495e;
                color: white;
                border-bottom: 3px solid #f1c40f;
            }
            .nav-menu ul {
                display: flex;
                justify-content: center;
                list-style: none;
                padding: 10px 0;
                margin: 0;
            }
            .nav-menu ul li {
                margin: 0 20px;
                cursor: pointer;
            }
            .nav-menu a {
                text-decoration: none;
                color: white;
                font-size: 1.2em;
            }
            .contact-section h2 {
                font-family: 'Poppins', sans-serif;
                color: #2c3e50;
                margin-bottom: 20px;
            }
            .contact-text {
                font-size: 1.2em;
                color: #7f8c8d;
                margin-bottom: 30px;
                line-height: 1.6;
            }
            .contact-info {
                font-size: 1.2em;
                color: #2c3e50;
                margin-bottom: 20px;
            }
            footer {
                background-color: #2c3e50;
                color: white;
                padding: 20px 0;
                text-align: center;
            }
            footer a {
                color: #f1c40f;
                text-decoration: none;
                margin: 0 10px;
            }
            footer a:hover {
                text-decoration: underline;
            }
        </style>
    </head>
    <body>
        <header class="header">
            <div class="logo">
                <img src="logo.png" alt="logo">   
                <h1>Winged Majesty</h1>
            </div>
        </header>
        <div class="nav-container">
            <nav class="nav-menu">
                <ul>
                    <li><a href="home.html">HOME</a></li> 
                    <li><a href="menu.html">MENU BOOK</a></li> 
                    <li><a href="admin.html">ADMINISTRATION</a></li> 
                    <li><a href="contact.html">CONTACT US</a></li> 
                </ul>
            </nav>
        </div>
        <main>
            <section class="contact-section">
                <h2>Get In Touch with Winged Majesty</h2>
                <p class="contact-text">
                    At Winged Majesty, we believe in delivering an unforgettable experience, whether you're enjoying our delicious meals or connecting with our dedicated team. Our commitment to excellence and personalized service makes us more than just a place to eat – it's a journey. We are here to listen, help, and create memorable moments together. Your feedback, questions, or simply a hello, are always welcome!
                </p>
                <div class="contact-info">
                    <p><strong>Phone:</strong> +91 98745 10125</p>
                    <p><strong>Email:</strong> user@wingedmajesty.com</p>
                    <p><strong>Contact address:</strong>456 Pegasus Street, Block B, 3rd Floor
                        Silver Horizon Towers, Adyar
                        Chennai, Tamil Nadu 600020
                        India</p>
                </div>
            </section>
        </main>
        <footer>
            <p>Joseph C 2024 | <a href="privacy.html">Privacy Policy</a> | <a href="terms.html">Terms & Conditions</a></p>
        </footer>
    </body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2024-12-10 141152-1.png>)
![alt text](<Screenshot 2024-12-10 141204-1.png>)
![alt text](<Screenshot 2024-12-10 141934-1.png>)
![alt text](<Screenshot 2024-12-10 143519-1.png>)
![alt text](<Screenshot 2024-12-10 143532-1.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
