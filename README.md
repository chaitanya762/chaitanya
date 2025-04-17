# chaitanya
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Botanic Marketing Limited - B2B Plant & Chocolate Solutions</title>
    <style>
        /* Reset and base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        
        a {
            text-decoration: none;
            color: #39338E; /* Updated to match logo color */
        }
        
        /* Header */
        header {
            background-color: #fff;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #E84142; /* Changed to match the red accent in logo */
        }
        
        .customer-type {
            background-color: #39338E; /* Updated to match logo color */
            padding: 8px 0;
        }
        
        .customer-links {
            display: flex;
            justify-content: center;
        }
        
        .customer-links a {
            color: white;
            margin: 0 15px;
            font-weight: 500;
            padding: 5px 15px;
            border-radius: 4px;
            transition: background-color 0.3s;
        }
        
        .customer-links a:hover,
        .customer-links a.active {
            background-color: #2D2878; /* Darker shade of the purple in logo */
        }
        
        /* Hero section */
        .hero {
            background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('/api/placeholder/1200/600');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            align-items: center;
            color: white;
            margin-top: 90px;
        }
        
        .hero-content {
            max-width: 800px;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 18px;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: #39338E; /* Updated to match logo color */
            color: white;
            padding: 12px 25px;
            border-radius: 5px;
            font-weight: 500;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2D2878; /* Darker shade of the purple in logo */
        }
        
        /* Features section */
        .features {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            font-size: 36px;
            color: #39338E; /* Updated to match logo color */
        }
        
        .features-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .feature-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
        }
        
        .feature-img {
            height: 200px;
            background-color: #F2F0FF; /* Light purple background */
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .feature-content {
            padding: 25px;
        }
        
        .feature-content h3 {
            color: #39338E; /* Updated to match logo color */
            margin-bottom: 15px;
            font-size: 22px;
        }
        
        /* B2B Services */
        .b2b-services {
            padding: 80px 0;
        }
        
        .service-card {
            display: flex;
            margin-bottom: 40px;
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .service-img {
            flex: 0 0 40%;
            background-color: #F2F0FF; /* Light purple background */
            min-height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .service-content {
            flex: 0 0 60%;
            padding: 40px;
        }
        
        .service-content h3 {
            font-size: 24px;
            color: #39338E; /* Updated to match logo color */
            margin-bottom: 15px;
        }
        
        .service-content ul {
            margin: 20px 0;
            padding-left: 20px;
        }
        
        .service-content li {
            margin-bottom: 10px;
        }
        
        /* Pricing */
        .pricing {
            padding: 80px 0;
            background-color: #F2F0FF; /* Light purple background */
        }
        
        .pricing-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .pricing-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        
        .pricing-card:hover {
            transform: translateY(-10px);
        }
        
        .pricing-header {
            background-color: #39338E; /* Updated to match logo color */
            color: white;
            padding: 20px;
        }
        
        .pricing-header h3 {
            font-size: 24px;
            margin-bottom: 10px;
        }
        
        .pricing-price {
            font-size: 36px;
            font-weight: bold;
        }
        
        .pricing-price span {
            font-size: 16px;
            font-weight: normal;
        }
        
        .pricing-features {
            padding: 30px;
        }
        
        .pricing-features ul {
            list-style: none;
            margin-bottom: 25px;
        }
        
        .pricing-features li {
            margin-bottom: 15px;
            padding-bottom: 15px;
            border-bottom: 1px solid #f0f0f0;
        }
        
        .pricing-features li:last-child {
            border-bottom: none;
        }
        
        /* Case Studies */
        .case-studies {
            padding: 80px 0;
        }
        
        .case-study {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        /* Products Section */
        .products {
            padding: 80px 0;
        }
        
        .category-title {
            font-size: 28px;
            color: #39338E;
            margin: 40px 0 20px;
            text-align: center;
        }
        
        .products-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 25px;
        }
        
        .product-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .product-img {
            height: 200px;
            background-color: #f5f5f5;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }
        
        .product-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .product-content {
            padding: 20px;
        }
        
        .product-content h3 {
            font-size: 18px;
            margin-bottom: 10px;
            color: #39338E;
        }
        
        .product-content p {
            color: #777;
            margin-bottom: 15px;
        }
        
        .product-price {
            font-size: 20px;
            font-weight: bold;
            color: #E84142;
            margin-bottom: 15px;
        }
        
        .add-to-cart {
            display: inline-block;
            background-color: #39338E;
            color: white;
            padding: 8px 15px;
            border-radius: 4px;
            font-size: 14px;
            transition: background-color 0.3s;
        }
        
        .add-to-cart:hover {
            background-color: #2D2878;
        }
        
        .category-section {
            margin-bottom: 60px;
        }
        
        /* Footer */
        footer {
            background-color: #39338E; /* Updated to match logo color */
            color: white;
            padding: 60px 0 20px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .footer-col h4 {
            font-size: 18px;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h4::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 2px;
            background-color: #E84142; /* Red accent from logo */
        }
        
        .footer-col ul {
            list-style: none;
        }
        
        .footer-col ul li {
            margin-bottom: 12px;
        }
        
        .footer-col ul li a {
            color: #f0f0f0;
            transition: color 0.3s;
        }
        
        .footer-col ul li a:hover {
            color: #E84142; /* Red accent from logo */
            padding-left: 5px;
        }
        
        .social-links {
            display: flex;
            margin-top: 20px;
        }
        
        .social-links a {
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            margin-right: 10px;
            border-radius: 50%;
            text-align: center;
            line-height: 40px;
            color: white;
            transition: all 0.3s;
        }
        
        .social-links a:hover {
            background-color: #E84142; /* Red accent from logo */
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .contact-info {
            margin-bottom: 15px;
        }
        
        .contact-info p {
            margin-bottom: 8px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="nav-container">
                <div class="logo">
                    <img src="/api/placeholder/150/50" alt="Botanic Marketing Limited Logo">
                </div>
                <nav>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#products">Products</a></li>
                        <li><a href="#pricing">Pricing</a></li>
                        <li><a href="#case-studies">Case Studies</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
        <div class="customer-type">
            <div class="container">
                <div class="customer-links">
                    <a href="#" class="active">Corporate</a>
                    <a href="#">Hospitality</a>
                    <a href="#">Retail</a>
                    <a href="#">Healthcare</a>
                </div>
            </div>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>Professional Plant & Chocolate Solutions for Business</h1>
                <p>Enhance your workplace environment with our premium plant installations and artisan chocolate selections for corporate gifts and events.</p>
                <a href="#contact" class="btn">Get a Quote</a>
            </div>
        </div>
    </section>

    <section id="features" class="features">
        <div class="container">
            <h2 class="section-title">Why Choose Us</h2>
            <div class="features-container">
                <div class="feature-card">
                    <div class="feature-img">
                        <!-- Feature image would go here -->
                    </div>
                    <div class="feature-content">
                        <h3>Expertise & Experience</h3>
                        <p>With over 20 years in the industry, we offer unmatched expertise in plant selection, installation, and maintenance for commercial spaces.</p>
                    </div>
                </div>
                <div class="feature-card">
                    <div class="feature-img">
                        <!-- Feature image would go here -->
                    </div>
                    <div class="feature-content">
                        <h3>Sustainable Solutions</h3>
                        <p>Our eco-friendly approach ensures minimal environmental impact while maximizing the benefits of greenery in your space.</p>
                    </div>
                </div>
                <div class="feature-card">
                    <div class="feature-img">
                        <!-- Feature image would go here -->
                    </div>
                    <div class="feature-content">
                        <h3>Premium Products</h3>
                        <p>From plants to chocolates, we provide only the highest quality products for your business needs and special occasions.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="services" class="b2b-services">
        <div class="container">
            <h2 class="section-title">Our B2B Services</h2>
            <div class="service-card">
                <div class="service-img">
                    <!-- Service image would go here -->
                </div>
                <div class="service-content">
                    <h3>Plant Installation & Design</h3>
                    <p>Transform your commercial space with professionally designed plant installations that improve air quality and create a welcoming atmosphere.</p>
                    <ul>
                        <li>Custom planting schemes for offices, hotels, and retail spaces</li>
                        <li>Seasonal displays and plant rotations</li>
                        <li>Green walls and vertical gardens</li>
                        <li>Plant containers and displays that match your brand aesthetic</li>
                    </ul>
                    <a href="#contact" class="btn">Learn More</a>
                </div>
            </div>
            <div class="service-card">
                <div class="service-img">
                    <!-- Service image would go here -->
                </div>
                <div class="service-content">
                    <h3>Maintenance Programs</h3>
                    <p>Keep your plants healthy and vibrant with our comprehensive maintenance services, designed to fit your schedule and budget.</p>
                    <ul>
                        <li>Regular watering and feeding</li>
                        <li>Pruning and plant health monitoring</li>
                        <li>Pest prevention and treatment</li>
                        <li>Plant replacement guarantees</li>
                    </ul>
                    <a href="#contact" class="btn">Learn More</a>
                </div>
            </div>
        </div>
    </section>

    <section id="products" class="products">
        <div class="container">
            <h2 class="section-title">Our Chocolate Collection</h2>
            <p style="text-align: center; margin-bottom: 40px;">Discover our premium chocolate range, perfect for corporate gifts, events, and special occasions.</p>
            
            <!-- Category 1: RETRO JELLIES -->
            <div class="category-section">
                <h3 class="category-title">RETRO JELLIES</h3>
                <div class="products-container">
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Retro Jellies - Classic Mix">
                        </div>
                        <div class="product-content">
                            <h3>Classic Mix</h3>
                            <p>Nostalgic chocolate-covered jellies with classic flavors.</p>
                            <div class="product-price">€1.25</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Retro Jellies - Fruit Selection">
                        </div>
                        <div class="product-content">
                            <h3>Fruit Selection</h3>
                            <p>Chocolate-coated fruit jellies with retro appeal.</p>
                            <div class="product-price">€1.45</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Retro Jellies - Berry Blast">
                        </div>
                        <div class="product-content">
                            <h3>Berry Blast</h3>
                            <p>Mixed berry jellies with a luxurious chocolate coating.</p>
                            <div class="product-price">€1.50</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Retro Jellies - Rainbow Mix">
                        </div>
                        <div class="product-content">
                            <h3>Rainbow Mix</h3>
                            <p>Colorful assortment of chocolate-dipped jelly treats.</p>
                            <div class="product-price">€1.35</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Category 2: EMMA'S JELLIES -->
            <div class="category-section">
                <h3 class="category-title">EMMA'S JELLIES</h3>
                <div class="products-container">
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Emma's Jellies - Premium Selection">
                        </div>
                        <div class="product-content">
                            <h3>Premium Selection</h3>
                            <p>Handcrafted chocolate jellies with gourmet flavors.</p>
                            <div class="product-price">€1.75</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Emma's Jellies - Citrus Delight">
                        </div>
                        <div class="product-content">
                            <h3>Citrus Delight</h3>
                            <p>Zesty orange and lemon jellies enrobed in fine chocolate.</p>
                            <div class="product-price">€1.65</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Emma's Jellies - Signature Mix">
                        </div>
                        <div class="product-content">
                            <h3>Signature Mix</h3>
                            <p>Emma's specially curated jelly and chocolate collection.</p>
                            <div class="product-price">€1.85</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Emma's Jellies - Luxury Assortment">
                        </div>
                        <div class="product-content">
                            <h3>Luxury Assortment</h3>
                            <p>Premium jellies with dark, milk, and white chocolate.</p>
                            <div class="product-price">€1.95</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Category 3: SUPER NATURE -->
            <div class="category-section">
                <h3 class="category-title">SUPER NATURE</h3>
                <div class="products-container">
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Super Nature - Organic Blend">
                        </div>
                        <div class="product-content">
                            <h3>Organic Blend</h3>
                            <p>Natural chocolate with organic fruit-flavored centers.</p>
                            <div class="product-price">€1.80</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Super Nature - Superfood Mix">
                        </div>
                        <div class="product-content">
                            <h3>Superfood Mix</h3>
                            <p>Chocolate with berry and antioxidant-rich fillings.</p>
                            <div class="product-price">€1.90</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Super Nature - Plant Based">
                        </div>
                        <div class="product-content">
                            <h3>Plant Based</h3>
                            <p>Vegan chocolate with all-natural fruit jelly centers.</p>
                            <div class="product-price">€1.85</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Super Nature - Pure Cocoa">
                        </div>
                        <div class="product-content">
                            <h3>Pure Cocoa</h3>
                            <p>High cocoa content chocolate with natural ingredients.</p>
                            <div class="product-price">€1.70</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Category 4: SCREAMER BIG LICK -->
            <div class="category-section">
                <h3 class="category-title">SCREAMER BIG LICK</h3>
                <div class="products-container">
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Big Lick - Original">
                        </div>
                        <div class="product-content">
                            <h3>Original</h3>
                            <p>Bold chocolate lollipops with intensely flavored centers.</p>
                            <div class="product-price">€1.50</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Big Lick - Sour Blast">
                        </div>
                        <div class="product-content">
                            <h3>Sour Blast</h3>
                            <p>Chocolate-coated lollipops with explosive sour centers.</p>
                            <div class="product-price">€1.60</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Big Lick - Extreme Fizz">
                        </div>
                        <div class="product-content">
                            <h3>Extreme Fizz</h3>
                            <p>Chocolate lollipops with fizzy, popping centers.</p>
                            <div class="product-price">€1.70</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Big Lick - Chili Heat">
                        </div>
                        <div class="product-content">
                            <h3>Chili Heat</h3>
                            <p>Spicy chocolate lollipops with a fiery kick.</p>
                            <div class="product-price">€1.65</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Category 5: SCREAMER CORE -->
            <div class="category-section">
                <h3 class="category-title">SCREAMER CORE</h3>
                <div class="products-container">
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Core - Liquid Center">
                        </div>
                        <div class="product-content">
                            <h3>Liquid Center</h3>
                            <p>Chocolate shells with explosive liquid filling.</p>
                            <div class="product-price">€1.40</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Core - Double Trouble">
                        </div>
                        <div class="product-content">
                            <h3>Double Trouble</h3>
                            <p>Dual-flavored chocolate with contrasting centers.</p>
                            <div class="product-price">€1.55</div>
                            <a href="#" class="add-to-cart">Add to Cart</a>
                        </div>
                    </div>
                    <div class="product-card">
                        <div class="product-img">
                            <img src="/api/placeholder/300/300" alt="Screamer Core - Mystery Mix">
                        </div>
                        <div class="product-content">
                            <h3>Mystery Mix</h3>
                            <p>Surprise-centered chocolates with random fillings.</p>
                            <div class="product-price">€1.45</div>
                            <a href="#" class="add-to-cart">Add to
