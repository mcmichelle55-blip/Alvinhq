#   
<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Alvin Profile HQ | Premium Digital Assets</title>  
    <style>  
        /* BASE STYLES & THEME */  
        :root {  
            --hq-cyan: #00d4ff;  
            --hq-dark: #0b0e11;  
            --hq-card: #1e2329;  
            --hq-nav: #161a1e;  
            --white: #ffffff;  
            --gray: #888888;  
        }  
  
        body {  
            margin: 0;  
            padding: 0;  
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;  
            background-color: var(--hq-dark);  
            color: var(--white);  
            scroll-behavior: smooth;  
        }  
  
        /* NAVIGATION */  
        nav {  
            display: flex;  
            justify-content: space-between;  
            align-items: center;  
            padding: 15px 5%;  
            background: var(--hq-nav);  
            position: sticky;  
            top: 0;  
            z-index: 1000;  
            border-bottom: 1px solid #333;  
        }  
  
        .logo img {  
            height: 50px; /* Adjust based on your logo shape */  
            display: block;  
        }  
  
        nav ul {  
            display: flex;  
            list-style: none;  
            gap: 25px;  
            margin: 0;  
        }  
  
        nav ul li a {  
            color: var(--white);  
            text-decoration: none;  
            font-weight: 600;  
            font-size: 0.9rem;  
            transition: 0.3s;  
        }  
  
        nav ul li a:hover {  
            color: var(--hq-cyan);  
        }  
  
        /* HERO SECTION */  
        header {  
            height: 85vh;  
            width: 100%;  
            display: flex;  
            flex-direction: column;  
            justify-content: flex-end;  
            align-items: center;  
            /* Update 'image_0.png' to your actual banner filename */  
            background: linear-gradient(rgba(0,0,0,0.2), rgba(0,0,0,0.9)),   
                        url('image_0.png') no-repeat center center;  
            background-size: cover;  
            text-align: center;  
            padding-bottom: 60px;  
            box-sizing: border-box;  
        }  
  
        .btn-hero {  
            padding: 18px 45px;  
            background-color: var(--hq-cyan);  
            color: #000;  
            text-decoration: none;  
            font-weight: 800;  
            font-size: 1.1rem;  
            border-radius: 8px;  
            transition: 0.3s;  
            text-transform: uppercase;  
            box-shadow: 0 0 15px rgba(0, 212, 255, 0.4);  
        }  
  
        .btn-hero:hover {  
            background-color: var(--white);  
            box-shadow: 0 0 25px rgba(0, 212, 255, 0.7);  
            transform: scale(1.05);  
        }  
  
        /* GALLERY & SERVICES */  
        .section-padding {  
            padding: 80px 5%;  
            text-align: center;  
        }  
  
        .gallery-grid {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));  
            gap: 30px;  
            max-width: 1200px;  
            margin: 40px auto;  
        }  
  
        .service-card {  
            background: var(--hq-card);  
            border-radius: 15px;  
            overflow: hidden;  
            border: 1px solid #333;  
            transition: 0.3s;  
            text-align: left;  
        }  
  
        .service-card:hover {  
            transform: translateY(-10px);  
            border-color: var(--hq-cyan);  
        }  
  
        .service-img {  
            width: 100%;  
            height: 200px;  
            background: #2b3139;  
            display: flex;  
            align-items: center;  
            justify-content: center;  
            color: #444;  
            font-weight: bold;  
        }  
  
        .service-info {  
            padding: 25px;  
        }  
  
        .service-info h3 {  
            margin: 0 0 10px 0;  
            color: var(--hq-cyan);  
        }  
  
        .price-tag {  
            font-size: 1.4rem;  
            font-weight: bold;  
            margin: 15px 0;  
        }  
  
        .buy-btn {  
            display: block;  
            width: 100%;  
            padding: 12px;  
            background-color: var(--hq-cyan);  
            color: #000;  
            text-align: center;  
            text-decoration: none;  
            font-weight: bold;  
            border-radius: 6px;  
            transition: 0.3s;  
        }  
  
        .buy-btn:hover {  
            background-color: var(--white);  
        }  
  
        /* TRUST & FOOTER */  
        .trust-bar {  
            background: var(--hq-nav);  
            padding: 40px 5%;  
            border-top: 1px solid #333;  
        }  
  
        .badge-container {  
            display: flex;  
            justify-content: center;  
            gap: 15px;  
            flex-wrap: wrap;  
            margin-top: 20px;  
        }  
  
        .badge {  
            border: 1px solid var(--hq-cyan);  
            padding: 8px 20px;  
            border-radius: 30px;  
            font-size: 0.8rem;  
            color: var(--hq-cyan);  
            text-transform: uppercase;  
        }  
  
        /* FLOATING WHATSAPP */  
        .whatsapp-float {  
            position: fixed;  
            bottom: 30px;  
            right: 30px;  
            background-color: #25d366;  
            color: white;  
            padding: 15px 25px;  
            border-radius: 50px;  
            text-decoration: none;  
            font-weight: bold;  
            box-shadow: 0 5px 15px rgba(0,0,0,0.4);  
            z-index: 1000;  
            display: flex;  
            align-items: center;  
            gap: 10px;  
            transition: 0.3s;  
        }  
  
        .whatsapp-float:hover {  
            transform: scale(1.1);  
            background-color: #1ebe57;  
        }  
  
        footer {  
            padding: 30px;  
            font-size: 0.8rem;  
            color: var(--gray);  
            border-top: 1px solid #222;  
        }  
  
        /* MOBILE ADJUSTMENTS */  
        @media (max-width: 768px) {  
            header { height: 60vh; }  
            nav { padding: 15px 20px; }  
            nav ul { display: none; } /* Simplified for mobile */  
        }  
    </style>  
</head>  
<body>  
  
    <nav>  
        <div class="logo">  
            <img src="logo.png" alt="Alvin Profile HQ">  
        </div>  
        <ul>  
            <li><a href="#">HOME</a></li>  
            <li><a href="#services">INVENTORY</a></li>  
            <li><a href="#trust">SECURITY</a></li>  
        </ul>  
    </nav>  
  
    <header>  
        <a href="https://wa.me/2347044190741" class="btn-hero">VIEW HQ INVENTORY</a>  
    </header>  
  
    <section id="services" class="section-padding">  
        <h2 style="font-size: 2.5rem; margin-bottom: 5px;">PREMIUM ASSETS</h2>  
        <p style="color: var(--gray); margin-bottom: 40px;">Selected High-Tier CODM Accounts & Professional Branding</p>  
  
        <div class="gallery-grid">  
            <div class="service-card">  
                <div class="service-img">MYTHIC ACCOUNT</div>  
                <div class="service-info">  
                    <h3>Mythic Bundle #01</h3>  
                    <p>Fully stacked with rare skins, maxed mythic weapons, and full access.</p>  
                    <div class="price-tag">DM for Price</div>  
                    <a href="https://wa.me/2347044190741" class="buy-btn">BUY NOW</a>  
                </div>  
            </div>  
  
            <div class="service-card">  
                <div class="service-img">CUSTOM BRANDING</div>  
                <div class="service-info">  
                    <h3>HQ Branding Pack</h3>  
                    <p>Custom 4D sales banners, logos, and social media flyers for sellers.</p>  
                    <div class="price-tag">From $20</div>  
                    <a href="https://wa.me/2347044190741" class="buy-btn">ORDER DESIGN</a>  
                </div>  
            </div>  
  
            <div class="service-card">  
                <div class="service-img">LEGENDARY ACC</div>  
                <div class="service-info">  
                    <h3>Ranked Specialist</h3>  
                    <p>Legendary Multi/BR rank with rare character skins and emotes.</p>  
                    <div class="price-tag">Secure Deal</div>  
                    <a href="https://wa.me/2347044190741" class="buy-btn">BUY NOW</a>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <section id="trust" class="trust-bar">  
        <div style="text-align: center;">  
            <h2 style="margin-bottom: 10px;">WHY CHOOSE HQ?</h2>  
            <div class="badge-container">  
                <span class="badge">Verified Seller</span>  
                <span class="badge">100% Secure Transfer</span>  
                <span class="badge">Instant Delivery</span>  
                <span class="badge">Crypto / Bank / Cards</span>  
            </div>  
        </div>  
    </section>  
  
    <footer style="text-align: center;">  
        <p>&copy; 2026 ALVIN PROFILE HQ. All Rights Reserved.</p>  
    </footer>  
  
    <a href="https://wa.me/2347044190741" class="whatsapp-float">  
        <span>Chat with Alvin HQ</span>  
    </a>  
  
</body>  
</html>  
