<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description"
          content="Elegant women's clothing boutique offering stylish ethnic wear, western wear, sarees and accessories.">

    <title>Elegance Boutique | Women's Clothing</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
          rel="stylesheet">

    <style>
        * {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #fff8fb;
            color: #292929;
        }

        .navbar {
            box-shadow: 0 3px 12px rgba(0,0,0,.10);
        }

        .navbar-brand,
        .section-title,
        .custom-card h4 {
            color: #9b3f65 !important;
        }

        .nav-link {
            font-weight: 600;
            transition: .3s;
        }

        .nav-link:hover {
            color: #9b3f65 !important;
        }

        .hero {
            min-height: 620px;
            display: flex;
            align-items: center;
            color: white;

            background:
                linear-gradient(
                    rgba(75,25,45,.65),
                    rgba(75,25,45,.65)
                ),
                url("https://images.unsplash.com/photo-1496747611176-843222e1e57c?auto=format&fit=crop&w=1600&q=80")
                center/cover;
        }

        .hero h1 {
            font-size: clamp(40px, 6vw, 68px);
            font-weight: 700;
        }

        .hero p {
            font-size: 19px;
            max-width: 750px;
        }

        .btn-main {
            background: #e8a0b8;
            color: #222;
            border: none;
            font-weight: bold;
            padding: 12px 27px;
            border-radius: 25px;
            transition: .3s;
        }

        .btn-main:hover {
            background: #f5c4d4;
            color: #222;
            transform: translateY(-3px);
        }

        section {
            padding: 70px 0;
        }

        .section-title {
            font-weight: bold;
            margin-bottom: 12px;
        }

        .section-subtitle {
            color: #666;
            margin-bottom: 35px;
        }

        .custom-card {
            background: white;
            border: none;
            border-radius: 15px;
            padding: 25px;
            height: 100%;
            box-shadow: 0 5px 20px rgba(0,0,0,.08);
            transition: .3s;
        }

        .custom-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 10px 25px rgba(0,0,0,.13);
        }

        .about-box {
            background: white;
            border-radius: 18px;
            padding: 30px;
            box-shadow: 0 5px 20px rgba(0,0,0,.08);
        }

        .product-card {
            overflow: hidden;
            padding: 0;
        }

        .product-card img {
            width: 100%;
            height: 260px;
            object-fit: cover;
            transition: .4s;
        }

        .product-card:hover img {
            transform: scale(1.04);
        }

        .product-content {
            padding: 22px;
        }

        .price {
            color: #b13e69;
            font-size: 21px;
            font-weight: bold;
        }

        .tag {
            display: inline-block;
            background: #fbe4ed;
            color: #9b3f65;
            padding: 8px 14px;
            border-radius: 20px;
            margin: 5px 4px 5px 0;
            font-size: 14px;
            font-weight: 600;
        }

        .ad-box {
            background:
                linear-gradient(
                    rgba(75,25,45,.70),
                    rgba(75,25,45,.70)
                ),
                url("https://images.unsplash.com/photo-1483985988355-763728e1935b?auto=format&fit=crop&w=1500&q=80")
                center/cover;

            color: white;
            padding: 70px 30px;
            border-radius: 20px;
            text-align: center;
        }

        .ad-box h2 {
            font-size: clamp(30px, 5vw, 48px);
            font-weight: bold;
        }

        .offer-badge {
            display: inline-block;
            background: #e8a0b8;
            color: #222;
            padding: 10px 18px;
            border-radius: 25px;
            font-weight: bold;
        }

        .social-card {
            border-left: 5px solid #9b3f65;
        }

        .email-section {
            background: #f9edf2;
        }

        .email-wrapper {
            max-width: 850px;
            margin: auto;
        }

        .email-subject {
            background: white;
            padding: 15px 20px;
            border-radius: 8px 8px 0 0;
            border: 1px solid #ddd;
        }

        .email-card {
            background: white;
            border: 1px solid #ddd;
            overflow: hidden;
            box-shadow: 0 5px 18px rgba(0,0,0,.08);
        }

        .email-banner {
            position: relative;
        }

        .email-banner img {
            width: 100%;
            height: 280px;
            object-fit: cover;
        }

        .email-banner-text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%,-50%);
            width: 90%;
            text-align: center;
            color: white;
            text-shadow: 1px 2px 5px rgba(0,0,0,.7);
        }

        .email-banner-text h2 {
            font-size: clamp(28px,5vw,45px);
            font-weight: bold;
        }

        .email-offer {
            position: absolute;
            right: 25px;
            top: 20px;
            background: #e8a0b8;
            color: #222;
            width: 75px;
            height: 75px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            font-weight: bold;
            font-size: 13px;
        }

        .email-content {
            padding: 30px;
        }

        .email-button {
            display: inline-block;
            background: #9b3f65;
            color: white;
            padding: 12px 25px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
        }

        .contact-box {
            background: #fbe4ed;
            border-radius: 18px;
            padding: 30px;
        }

        footer {
            background: #4d2435;
            color: white;
            text-align: center;
            padding: 30px 15px;
        }

        @media(max-width:576px) {

            .hero {
                min-height: 550px;
            }

            .hero p {
                font-size: 16px;
            }

            section {
                padding: 50px 0;
            }

            .email-banner img {
                height: 230px;
            }

            .email-offer {
                width: 62px;
                height: 62px;
                font-size: 11px;
                right: 15px;
                top: 15px;
            }

            .email-content {
                padding: 22px;
            }
        }
    </style>
</head>

<body>

<!-- NAVBAR -->

<nav class="navbar navbar-expand-lg bg-white sticky-top">

    <div class="container">

        <a class="navbar-brand" href="#">
            👗 Elegance Boutique
        </a>

        <button class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarMenu">

            <span class="navbar-toggler-icon"></span>

        </button>

        <div class="collapse navbar-collapse" id="navbarMenu">

            <ul class="navbar-nav ms-auto">

                <li class="nav-item">
                    <a class="nav-link" href="#home">Home</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#about">About</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#products">Collection</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#audience">Audience</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#seo">SEO</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#social">Social Media</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#advertisement">Advertisement</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#email">Email</a>
                </li>

            </ul>

        </div>
    </div>
</nav>


<!-- HERO -->

<header class="hero" id="home">

    <div class="container">

        <div class="col-lg-8">

            <p class="fw-bold">
                DIGITAL MARKETING PROJECT
            </p>

            <h1>
                Style That Speaks for You
            </h1>

            <p class="mt-3">
                Discover elegant, stylish and affordable women's
                clothing designed to make every occasion special.
            </p>

            <p>
                Explore ethnic wear, western outfits, sarees,
                dresses and fashionable accessories.
            </p>

            <a href="#products"
               class="btn btn-main mt-3">
                Explore Collection
            </a>

        </div>

    </div>

</header>


<!-- ABOUT -->

<section id="about">

    <div class="container">

        <h2 class="section-title text-center">
            1. Boutique Profile
        </h2>

        <p class="section-subtitle text-center">
            About our women's clothing boutique
        </p>

        <div class="about-box mb-4">

            <h3 class="section-title">
                About Elegance Boutique
            </h3>

            <p>
                Elegance Boutique is a women's clothing boutique
                offering fashionable, comfortable and affordable
                clothing for modern women.
            </p>

            <p>
                Our collection includes ethnic wear, western wear,
                sarees, dresses and stylish accessories suitable
                for everyday wear and special occasions.
            </p>

        </div>


        <div class="row g-4">

            <div class="col-md-4">
                <div class="custom-card">
                    <h4>Business Name</h4>
                    <p>Elegance Boutique</p>
                </div>
            </div>

            <div class="col-md-4">
                <div class="custom-card">
                    <h4>Business Type</h4>
                    <p>Women's Clothing Boutique</p>
                </div>
            </div>

            <div class="col-md-4">
                <div class="custom-card">
                    <h4>Location</h4>
                    <p>Nagpur, Maharashtra, India</p>
                </div>
            </div>

            <div class="col-md-4">
                <div class="custom-card">
                    <h4>Contact</h4>
                    <p>+91 98765 43210</p>
                </div>
            </div>

            <div class="col-md-4">
                <div class="custom-card">
                    <h4>Email</h4>
                    <p>eleganceboutique@example.com</p>
                </div>
            </div>

            <div class="col-md-4">
                <div class="custom-card">
                    <h4>Shopping</h4>
                    <p>Offline & Online Orders</p>
                </div>
            </div>

        </div>


        <div class="about-box mt-4">

            <h3 class="section-title">
                Our USP
            </h3>

            <ul>

                <li>Trendy and stylish clothing</li>

                <li>Affordable prices</li>

                <li>Quality fabrics</li>

                <li>New collections regularly</li>

                <li>Personalized customer service</li>

                <li>Online ordering facility</li>

            </ul>

        </div>

    </div>

</section>


<!-- PRODUCTS -->

<section id="products" class="bg-light">

    <div class="container">

        <h2 class="section-title text-center">
            2. Latest Collection
        </h2>

        <p class="section-subtitle text-center">
            Fashionable outfits for every occasion
        </p>


        <div class="row g-4">


            <!-- PRODUCT 1 -->

            <div class="col-md-4">

                <div class="custom-card product-card">

                    <img
                        src="https://images.unsplash.com/photo-1610030469983-98e550d6193c?auto=format&fit=crop&w=900&q=80"
                        alt="Traditional Saree">

                    <div class="product-content">

                        <h4>
                            Designer Saree
                        </h4>

                        <p>
                            Elegant sarees perfect for festivals,
                            weddings and special occasions.
                        </p>

                        <p class="price">
                            ₹1,499 onwards
                        </p>

                        <button
                            class="btn btn-main"
                            onclick="showMessage('Designer Saree')">

                            Shop Now

                        </button>

                    </div>

                </div>

            </div>


            <!-- PRODUCT 2 -->

            <div class="col-md-4">

                <div class="custom-card product-card">

                    <img
                        src="https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?auto=format&fit=crop&w=900&q=80"
                        alt="Women's Dress">

                    <div class="product-content">

                        <h4>
                            Stylish Dresses
                        </h4>

                        <p>
                            Comfortable and trendy dresses
                            for casual and party wear.
                        </p>

                        <p class="price">
                            ₹899 onwards
                        </p>

                        <button
                            class="btn btn-main"
                            onclick="showMessage('Stylish Dress')">

                            Shop Now

                        </button>

                    </div>

                </div>

            </div>


            <!-- PRODUCT 3 -->

            <div class="col-md-4">

                <div class="custom-card product-card">

                    <img
                        src="https://images.unsplash.com/photo-1583391733956-6c78276477e2?auto=format&fit=crop&w=900&q=80"
                        alt="Ethnic Wear">

                    <div class="product-content">

                        <h4>
                            Ethnic Wear
                        </h4>

                        <p>
                            Beautiful ethnic outfits for festivals,
                            celebrations and family occasions.
                        </p>

                        <p class="price">
                            ₹1,199 onwards
                        </p>

                        <button
                            class="btn btn-main"
                            onclick="showMessage('Ethnic Wear')">

                            Shop Now

                        </button>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- TARGET AUDIENCE -->

<section id="audience">

    <div class="container">

        <h2 class="section-title text-center">
            3. Target Audience
        </h2>

        <p class="section-subtitle text-center">
            Customers who are most likely to purchase our products
        </p>


        <div class="row g-4">


            <div class="col-md-4">

                <div class="custom-card text-center">

                    <h4>👩 College Students</h4>

                    <p>
                        Age: 18–25
                    </p>

                    <p>
                        Interested in trendy, affordable and
                        comfortable outfits.
                    </p>

                    <span class="tag">
                        Instagram
                    </span>

                    <span class="tag">
                        Reels
                    </span>

                </div>

            </div>


            <div class="col-md-4">

                <div class="custom-card text-center">

                    <h4>👩‍💼 Working Women</h4>

                    <p>
                        Age: 22–40
                    </p>

                    <p>
                        Looking for stylish office wear,
                        casual wear and party outfits.
                    </p>

                    <span class="tag">
                        Facebook
                    </span>

                    <span class="tag">
                        Instagram
                    </span>

                </div>

            </div>


            <div class="col-md-4">

                <div class="custom-card text-center">

                    <h4>👩‍👩‍👧 Fashion Buyers</h4>

                    <p>
                        Age: 25–50
                    </p>

                    <p>
                        Interested in sarees, ethnic wear,
                        festive collections and accessories.
                    </p>

                    <span class="tag">
                        WhatsApp
                    </span>

                    <span class="tag">
                        Online Shopping
                    </span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- SEO -->

<section id="seo" class="bg-light">

    <div class="container">

        <h2 class="section-title text-center">
            4. SEO Keywords
        </h2>

        <p class="section-subtitle text-center">
            Keywords used to promote the boutique online
        </p>


        <div class="about-box">

            <h4>
                Short-Tail Keywords
            </h4>

            <div class="mb-4">

                <span class="tag">Women's Clothing</span>

                <span class="tag">Ladies Wear</span>

                <span class="tag">Fashion Boutique</span>

                <span class="tag">Sarees</span>

                <span class="tag">Ethnic Wear</span>

                <span class="tag">Dresses</span>

            </div>


            <h4>
                Long-Tail Keywords
            </h4>

            <div class="mb-4">

                <span class="tag">
                    Best women's clothing boutique
                </span>

                <span class="tag">
                    Affordable ladies wear online
                </span>

                <span class="tag">
                    Designer sarees in Nagpur
                </span>

                <span class="tag">
                    Trendy dresses for women
                </span>

                <span class="tag">
                    Ethnic wear for women
                </span>

            </div>


            <h4>
                SEO Strategy
            </h4>

            <ul>

                <li>
                    Use keywords in product titles.
                </li>

                <li>
                    Add keywords to product descriptions.
                </li>

                <li>
                    Use location-based keywords.
                </li>

                <li>
                    Upload high-quality product images.
                </li>

                <li>
                    Collect genuine customer reviews.
                </li>

                <li>
                    Regularly update the website.
                </li>

            </ul>

        </div>

    </div>

</section>


<!-- SOCIAL MEDIA -->

<section id="social">

    <div class="container">

        <h2 class="section-title text-center">
            5. Social Media Marketing
        </h2>

        <p class="section-subtitle text-center">
            Promoting the boutique through social media
        </p>


        <div class="row g-4">


            <div class="col-md-4">

                <div class="custom-card social-card">

                    <h4>
                        Instagram
                    </h4>

                    <p>
                        Upload product photos, fashion Reels,
                        new arrivals, styling ideas and offers.
                    </p>

                    <strong>
                        Sample Post:
                    </strong>

                    <p>
                        "New season, new style! ✨
                        Discover our latest women's collection."
                    </p>

                    <span class="tag">
                        #EleganceBoutique
                    </span>

                    <span class="tag">
                        #WomensFashion
                    </span>

                </div>

            </div>


            <div class="col-md-4">

                <div class="custom-card social-card">

                    <h4>
                        Facebook
                    </h4>

                    <p>
                        Share new collections, discounts,
                        customer reviews and festive offers.
                    </p>

                    <strong>
                        Sample Post:
                    </strong>

                    <p>
                        "Upgrade your wardrobe with our
                        latest collection. Shop your style today!"
                    </p>

                    <span class="tag">
                        #Fashion
                    </span>

                    <span class="tag">
                        #Boutique
                    </span>

                </div>

            </div>


            <div class="col-md-4">

                <div class="custom-card social-card">

                    <h4>
                        WhatsApp
                    </h4>

                    <p>
                        Send new collection photos,
                        catalogues, offers and order updates.
                    </p>

                    <strong>
                        Sample Message:
                    </strong>

                    <p>
                        "Hello! Our new women's collection
                        has arrived. Contact us for prices
                        and availability."
                    </p>

                    <span class="tag">
                        Direct Enquiry
                    </span>

                </div>

            </div>

        </div>


        <div class="about-box mt-4">

            <h4 class="section-title">
                Weekly Content Plan
            </h4>

            <div class="row">

                <div class="col-md-3">
                    <strong>Monday</strong>
                    <p>New Arrival</p>
                </div>

                <div class="col-md-3">
                    <strong>Wednesday</strong>
                    <p>Fashion Reel</p>
                </div>

                <div class="col-md-3">
                    <strong>Friday</strong>
                    <p>Special Offer</p>
                </div>

                <div class="col-md-3">
                    <strong>Sunday</strong>
                    <p>Customer Review</p>
                </div>

            </div>

        </div>

    </div>

</section>


<!-- ADVERTISEMENT -->

<section id="advertisement" class="bg-light">

    <div class="container">

        <h2 class="section-title text-center">
            6. Advertisement Design
        </h2>

        <p class="section-subtitle text-center">
            Sample online advertisement
        </p>


        <div class="ad-box">

            <span class="offer-badge">
                ✨ FESTIVE SALE
            </span>

            <p class="fw-bold mt-4">
                ELEGANCE BOUTIQUE
            </p>

            <h2>
                Your Style. Your Statement. 💕
            </h2>

            <p class="fs-5">
                Discover our latest collection of
                fashionable women's clothing.
            </p>

            <p>
                👗 Dresses
                &nbsp;&nbsp;
                🥻 Sarees
                &nbsp;&nbsp;
                ✨ Ethnic Wear
            </p>

            <button
                class="btn btn-main mt-3"
                onclick="showMessage('Festive Sale')">

                SHOP NOW

            </button>

            <p class="mt-4 mb-0">

                <strong>
                    Special Offer:
                </strong>

                Get up to 30% OFF on selected products.

            </p>

        </div>

    </div>

</section>


<!-- EMAIL MARKETING -->

<section id="email" class="email-section">

    <div class="container">

        <h2 class="section-title text-center">
            7. Email Marketing
        </h2>

        <p class="section-subtitle text-center">
            Sample promotional email campaign
        </p>


        <div class="email-wrapper">


            <div class="email-subject">

                <strong>
                    Subject:
                </strong>

                ✨ New Women's Collection – Up to 30% OFF!

            </div>


            <div class="email-card">


                <div class="email-banner">

                    <img
                        src="https://images.unsplash.com/photo-1496747611176-843222e1e57c?auto=format&fit=crop&w=1200&q=80"
                        alt="Women's Fashion">

                    <div class="email-banner-text">

                        <h2>
                            New Collection
                        </h2>

                        <p>
                            Stylish • Elegant • Affordable
                        </p>

                    </div>


                    <div class="email-offer">

                        UP TO
                        <br>
                        30%
                        <br>
                        OFF

                    </div>

                </div>


                <div class="email-content">

                    <h3 class="section-title">
                        Discover Our Latest Collection 💕
                    </h3>

                    <p>
                        Dear Customer,
                    </p>

                    <p>
                        Looking for stylish and affordable
                        women's clothing? Elegance Boutique
                        brings you our latest collection of
                        dresses, sarees, ethnic wear and
                        fashionable outfits.
                    </p>

                    <p>
                        Find your perfect style for every
                        occasion.
                    </p>


                    <strong>
                        Why Shop With Us?
                    </strong>

                    <ul class="mt-2">

                        <li>
                            Trendy designs
                        </li>

                        <li>
                            Quality fabrics
                        </li>

                        <li>
                            Affordable prices
                        </li>

                        <li>
                            New arrivals regularly
                        </li>

                        <li>
                            Easy ordering
                        </li>

                    </ul>


                    <div class="text-center my-4">

                        <span class="offer-badge">
                            🎉 UP TO 30% OFF
                        </span>

                        <p class="mt-3">
                            Limited-time offer on selected
                            products.
                        </p>

                    </div>


                    <div class="text-center">

                        <a href="#products"
                           class="email-button">

                            EXPLORE COLLECTION

                        </a>

                    </div>


                    <hr class="my-4">


                    <p>
                        Regards,
                        <br>

                        <strong>
                            Elegance Boutique
                        </strong>

                        <br>

                        📞 +91 98765 43210

                        <br>

                        📧 eleganceboutique@example.com

                        <br>

                        📍 Nagpur, Maharashtra

                    </p>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- CONTACT -->

<section>

    <div class="container">

        <div class="contact-box text-center">

            <h2 class="section-title">
                Find Your Perfect Style
            </h2>

            <p>
                Explore our latest women's clothing
                collection and choose your favourite outfit.
            </p>

            <p>

                📞 <strong>+91 98765 43210</strong>

                &nbsp;&nbsp;

                📧 <strong>
                    eleganceboutique@example.com
                </strong>

            </p>

            <button
                class="btn btn-main"
                onclick="showMessage('Elegance Boutique')">

                Contact Boutique

            </button>

        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    <strong>
        Digital Marketing Project
    </strong>

    <p class="mb-1">
        Promoting a Women's Clothing Boutique
    </p>

    <p class="mb-1">
        Elegance Boutique
    </p>

    <hr>

    <p class="mb-0">

        <strong>
            Created by: __________________
        </strong>

        <br>

        Roll No: __________________

    </p>

</footer>


<script
    src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js">
</script>


<script>

    function showMessage(item) {

        alert(
            "Thank you for your interest in " +
            item +
            "!\n\n" +
            "Please contact Elegance Boutique at " +
            "+91 98765 43210 for more details."
        );

    }

</script>

</body>
</html>
