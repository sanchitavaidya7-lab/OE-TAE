<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Elegance Boutique | Women's Fashion</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
}

body {
    background: #fffaf7;
    color: #342323;
}

header {
    background: #fff;
    padding: 20px 8%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0 2px 12px #00000010;
    position: sticky;
    top: 0;
    z-index: 10;
}

.logo {
    font-size: 27px;
    color: #a94f6b;
    font-weight: bold;
    letter-spacing: 1px;
}

nav a {
    text-decoration: none;
    color: #342323;
    margin-left: 22px;
    font-size: 15px;
}

nav a:hover {
    color: #b94f72;
}

.hero {
    min-height: 520px;
    display: flex;
    align-items: center;
    padding: 60px 8%;
    background: linear-gradient(90deg, #f6dce2, #fff4ee);
    gap: 30px;
}

.hero-text {
    flex: 1;
}

.hero-text h1 {
    font-family: Georgia, serif;
    font-size: clamp(38px, 5vw, 65px);
    line-height: 1.15;
    color: #71384c;
}

.hero-text p {
    margin: 20px 0;
    font-size: 17px;
    line-height: 1.7;
}

.btn {
    display: inline-block;
    padding: 13px 27px;
    background: #a94f6b;
    color: white;
    text-decoration: none;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 15px;
}

.btn:hover {
    background: #78354d;
}

.hero img {
    width: 46%;
    max-height: 430px;
    object-fit: cover;
    border-radius: 160px 160px 8px 8px;
}

.section {
    padding: 65px 8%;
    text-align: center;
}

.section h2 {
    font-family: Georgia, serif;
    color: #71384c;
    font-size: 36px;
    margin-bottom: 12px;
}

.subtitle {
    color: #777;
    margin-bottom: 35px;
}

.products {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
}

.product {
    background: white;
    padding-bottom: 22px;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 20px #0000000c;
    transition: transform 0.3s;
}

.product:hover {
    transform: translateY(-6px);
}

.product img {
    width: 100%;
    height: 300px;
    object-fit: cover;
}

.product h3 {
    margin: 18px 0 8px;
}

.price {
    color: #a94f6b;
    font-size: 19px;
    font-weight: bold;
    margin-bottom: 15px;
}

.about {
    background: #f7e7e8;
    padding: 55px 12%;
    text-align: center;
    line-height: 1.8;
}

.about h2 {
    font-family: Georgia, serif;
    color: #71384c;
    margin-bottom: 15px;
    font-size: 34px;
}

.contact {
    text-align: center;
    padding: 55px 20px;
}

.contact p {
    margin: 12px 0 22px;
}

footer {
    background: #482d37;
    color: white;
    text-align: center;
    padding: 22px;
}

@media (max-width: 750px) {
    header {
        padding: 18px 5%;
        flex-direction: column;
        gap: 15px;
    }

    nav a {
        margin: 0 7px;
        font-size: 13px;
    }

    .hero {
        flex-direction: column;
        text-align: center;
        padding: 45px 6%;
    }

    .hero img {
        width: 100%;
        max-height: 350px;
    }

    .products {
        grid-template-columns: repeat(2, 1fr);
        gap: 12px;
    }

    .product img {
        height: 210px;
    }

    .section {
        padding: 45px 5%;
    }
}

@media (max-width: 420px) {
    .products {
        grid-template-columns: 1fr;
    }

    .product img {
        height: 300px;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">✿ Elegance Boutique</div>
    <nav>
        <a href="#home">Home</a>
        <a href="#collection">Collection</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero" id="home">
    <div class="hero-text">
        <h1>Style That Makes You Shine</h1>
        <p>
            Discover beautiful ethnic wear, elegant dresses,
            and timeless fashion made for every woman.
        </p>
        <a href="#collection" class="btn">Explore Collection</a>
    </div>

    <img
      src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=900&q=85"
      alt="Elegant women's fashion">
</section>

<section class="section" id="collection">
    <h2>Our Collection</h2>
    <p class="subtitle">Find your perfect style, made for you.</p>

    <div class="products">

        <div class="product">
            <img src="https://images.unsplash.com/photo-1610030469983-98e550d6193c?auto=format&fit=crop&w=700&q=80"
                 alt="Traditional ethnic fashion">
            <h3>Ethnic Wear</h3>
            <p class="price">₹1,499</p>
            <button class="btn" onclick="order('Ethnic Wear')">
                Enquire Now
            </button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1595777457583-95e059d581b8?auto=format&fit=crop&w=700&q=80"
                 alt="Elegant women's dress">
            <h3>Party Dresses</h3>
            <p class="price">₹1,999</p>
            <button class="btn" onclick="order('Party Dresses')">
                Enquire Now
            </button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?auto=format&fit=crop&w=700&q=80"
                 alt="Fashion handbag">
            <h3>Fashion Accessories</h3>
            <p class="price">₹799</p>
            <button class="btn" onclick="order('Fashion Accessories')">
                Enquire Now
            </button>
        </div>

    </div>
</section>

<section class="about" id="about">
    <h2>About Our Boutique</h2>
    <p>
        Welcome to Elegance Boutique, where fashion meets confidence.
        We bring you handpicked styles, beautiful designs, and
        fashionable outfits to make every occasion special.
    </p>
</section>

<section class="contact" id="contact">
    <h2>Let's Connect 💗</h2>
    <p>Have a question about our collection? Contact us today.</p>
    <a href="https://wa.me/91XXXXXXXXXX" class="btn">
        Chat on WhatsApp
    </a>
</section>

<footer>
    <p>© 2026 Elegance Boutique | Fashion With Love ✿</p>
</footer>

<script>
function order(product) {
    const phone = "91XXXXXXXXXX";
    const message = "Hi! I am interested in " + product +
                    " from Elegance Boutique.";
    const url = "https://wa.me/" + phone +
                "?text=" + encodeURIComponent(message);

    window.open(url, "_blank");
}
</script>

</body>
</html>
