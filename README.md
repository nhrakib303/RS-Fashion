<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Buy authentic Punjabi dresses online. Traditional handcrafted designs with premium fabrics.">
    <title>Traditional Punjabi - Online Store</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;700&family=Shadows+Into+Light&display=swap" rel="stylesheet">
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Baloo 2', cursive;
            background-color: #f9f3e9;
            color: #333;
            line-height: 1.6;
        }
        
        header {
            background-color: #e31837; /* Punjabi Red */
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        
        nav {
            background-color: #d42e2e;
            padding: 15px;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            flex-wrap: wrap;
        }
        
        nav ul li {
            margin: 0 20px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #f4c430; /* Golden */
        }
        
        .hero {
            background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1595341595379-cf1cd0fb7fb3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            height: 70vh;
            min-height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
        }
        
        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 5px rgba(0,0,0,0.5);
        }
        
        .btn {
            display: inline-block;
            background-color: #f4c430; /* Golden */
            color: #000;
            padding: 12px 25px;
            border-radius: 50px;
            text-decoration: none;
            margin-top: 20px;
            font-weight: bold;
            transition: transform 0.3s, background-color 0.3s;
        }
        
        .btn:hover {
            transform: scale(1.05);
            background-color: #e31837;
            color: white;
        }
        
        .products {
            padding: 80px 20px;
            text-align: center;
        }
        
        .section-title {
            font-size: 2.5rem;
            margin-bottom: 15px;
            color: #e31837;
            position: relative;
            display: inline-block;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            width: 50%;
            height: 3px;
            background-color: #f4c430;
            bottom: -10px;
            left: 25%;
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }
        
        .product-card {
            background-color: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            position: relative;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        
        .product-img {
            height: 300px;
            background-size: cover;
            background-position: center;
        }
        
        .product-info {
            padding: 25px;
            text-align: left;
        }
        
        .product-info h3 {
            margin-bottom: 10px;
            font-size: 1.4rem;
            color: #333;
        }
        
        .product-info p {
            color: #666;
            margin-bottom: 15px;
        }
        
        .price {
            font-weight: bold;
            color: #e31837;
            font-size: 1.3rem;
            margin: 15px 0;
            display: block;
        }
        
        .discount {
            text-decoration: line-through;
            color: #999;
            font-size: 1rem;
            margin-left: 10px;
        }
        
        .rating {
            color: #f4c430;
            margin: 10px 0;
        }
        
        /* New: Cart Icon */
        .cart-icon {
            position: fixed;
            top: 20px;
            right: 30px;
            background-color: #f4c430;
            color: #000;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            cursor: pointer;
            z-index: 101;
            box-shadow: 0 3px 10px rgba(0,0,0,0.2);
        }
        
        .cart-count {
            position: absolute;
            top: -5px;
            right: -5px;
            background-color: #e31837;
            color: white;
            width: 25px;
            height: 25px;
            border-radius: 50%;
            font-size: 0.8rem;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 50px 0;
            margin-top: 80px;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .footer-section {
            flex: 1;
            min-width: 250px;
            margin: 20px;
            text-align: left;
        }
        
        .footer-section h3 {
            margin-bottom: 20px;
            font-size: 1.3rem;
            color: #f4c430;
        }
        
        .social-icons a {
            color: white;
            margin-right: 15px;
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-icons a:hover {
            color: #f4c430;
        }
        
        .copyright {
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid #444;
        }
        
        @media (max-width: 768px) {
            nav ul li {
                margin: 10px 15px;
            }
            
            .hero-content h1 {
                font-size: 2.5rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .cart-icon {
                width: 40px;
                height: 40px;
                font-size: 1.2rem;
                top: 15px;
                right: 20px;
            }
        }
        
        @media (max-width: 480px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 8px 0;
            }
            
            .hero {
                height: 60vh;
            }
            
            .hero-content h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Cart Icon (Would need JavaScript for functionality) -->
    <div class="cart-icon">
        <i class="fas fa-shopping-cart"></i>
        <span class="cart-count">0</span>
    </div>
    
    <header>
        <h1>Traditional Punjabi</h1>
        <p>Authentic Punjabi Dresses Online</p>
    </header>
    
    <nav>
        <ul>
            <li><a href="#"><i class="fas fa-home"></i> Home</a></li>
            <li><a href="#"><i class="fas fa-store"></i> Shop</a></li>
            <li><a href="#"><i class="fas fa-info-circle"></i> About Us</a></li>
            <li><a href="#"><i class="fas fa-phone"></i> Contact</a></li>
        </ul>
    </nav>
    
    <section class="hero">
        <div class="hero-content">
            <h1>Beautiful Punjabi Collection</h1>
            <p>Handcrafted with traditional designs and premium fabrics</p>
            <a href="#" class="btn">Shop Now</a>
        </div>
    </section>
    
    <main class="products">
        <h2 class="section-title">Our Featured Products</h2>
        <p>Discover our latest Punjabi dress collection</p>
        
        <div class="product-grid">
            <article class="product-card">
                <figure class="product-img"
