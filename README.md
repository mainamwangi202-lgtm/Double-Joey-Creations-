# Double-Joey-Creations-
It's the home for those that own their stories
https://github.com/mainamwangi202-lgtm/Double-Joey-Creations-.git
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Double Joey Creations — Night Luxury</title>
  <meta name="description" content="Double Joey Creations | Shoes, Clothing & Jewelry — Urban Luxe Collection" />
  <link rel="stylesheet" href="styles.css" />
  <link rel="icon" href="images/favicon.png" />
</head>
<body>
  <header class="site-header">
    <div class="topbar">
      <button id="menuBtn" class="icon-btn">☰</button>
      <div class="logo">DOUBLE JOEY CREATIONS</div>
      <div class="icons">
        <button id="searchBtn" class="icon-btn">🔍</button>
        <button id="cartBtn" class="icon-btn">🛒 <span id="cartCount">0</span></button>
      </div>
    </div>
  </header>

  <main id="main">
    <!-- HERO -->
    <section class="hero">
      <div class="hero-image" style="background-image:url('images/hero-night.jpg')"></div>
      <div class="hero-overlay">
        <h1 class="hero-title">Where Elegance Meets Everyday Style</h1>
        <p class="hero-sub">Shoes, Clothing & Jewelry crafted for expression</p>
        <div class="hero-ctas">
          <a href="#shop" class="btn btn-gold">Shop Men</a>
          <a href="#shop" class="btn btn-rose">Shop Women</a>
        </div>
      </div>
    </section>

    <!-- CATEGORIES -->
    <section class="categories" id="shop">
      <div class="category" data-cat="shoes">
        <img src="images/cat-shoes.jpg" alt="Shoes" />
        <div class="cat-label">Shoes</div>
      </div>
      <div class="category" data-cat="clothing">
        <img src="images/cat-clothing.jpg" alt="Clothing" />
        <div class="cat-label">Clothing</div>
      </div>
      <div class="category" data-cat="jewelry">
        <img src="images/cat-jewelry.jpg" alt="Jewelry" />
        <div class="cat-label">Jewelry</div>
      </div>
    </section>

    <!-- FEATURED -->
    <section class="featured">
      <h2>Urban Luxe Collection</h2>
      <p class="muted">Designed for those who own their story.</p>
      <div class="product-grid" id="productGrid"></div>
    </section>

    <!-- ABOUT -->
    <section class="about">
      <div class="about-img" style="background-image:url('images/about-studio.jpg')"></div>
      <div class="about-text">
        <h3>Crafted for Those Who Dare to Be Distinct</h3>
        <p>At Double Joey Creations, every stitch, shine, and silhouette tells a story of ambition and authenticity. We blend urban edge with couture sensibility — designed for both men and women who make fashion a statement.</p>
        <a href="#contact" class="btn btn-outline">Learn Our Story</a>
      </div>
    </section>

    <!-- TESTIMONIALS -->
    <section class="testimonials">
      <h4>What our customers say</h4>
      <div class="test-grid">
        <blockquote>“Exceptional craftsmanship and effortless style — I’ve never felt more confident.” <cite>— Sophia A.</cite></blockquote>
        <blockquote>“The jewelry is exquisite. It’s become my everyday luxury.” <cite>— Miriam O.</cite></blockquote>
      </div>
    </section>

    <!-- NEWSLETTER -->
    <section class="newsletter">
      <h5>Join the Double Joey Family</h5>
      <p class="muted">Receive new drops, exclusive offers, and style edits.</p>
      <form id="newsletterForm" class="newsletter-form">
        <input id="newsletterEmail" type="email" placeholder="Your email address" required />
        <button class="btn btn-rose" type="submit">Subscribe</button>
      </form>
      <div id="newsletterMsg" class="muted small"></div>
    </section>

    <!-- FOOTER -->
    <footer class="site-footer" id="contact">
      <div class="footer-col">
        <div class="logo small">DOUBLE JOEY CREATIONS</div>
        <p class="muted">© <span id="year"></span> Double Joey Creations</p>
      </div>
      <div class="footer-col">
        <h6>Contact</h6>
        <p class="muted">info@doublejoeycreations.com<br/>+1 (555) 123-4567</p>
      </div>
      <div class="footer-col">
        <h6>Follow</h6>
        <div class="socials">
          <a href="#" class="social">Instagram</a>
          <a href="#" class="social">TikTok</a>
          <a href="#" class="social">Facebook</a>
        </div>
      </div>
    </footer>
  </main>

  <!-- PRODUCT MODAL -->
  <div id="productModal" class="modal hidden">
    <div class="modal-content">
      <button id="closeModal" class="close">×</button>
      <div class="modal-grid">
        <div class="modal-img" id="modalImg"></div>
        <div class="modal-info">
          <h3 id="modalTitle"></h3>
          <p id="modalPrice" class="price"></p>
          <p id="modalDesc"></p>
          <label for="sizeSelect">Size</label>
          <select id="sizeSelect"></select>
          <label for="qty">Quantity</label>
          <input id="qty" type="number" min="1" value="1" />
          <div class="modal-actions">
            <button id="addToCart" class="btn btn-gold">Add to Cart</button>
            <a href="checkout.html" id="buyNow" class="btn btn-rose">Buy Now</a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- CART SLIDEOUT -->
  <div id="cartSlide" class="cart hidden">
    <div class="cart-header"><h4>Your Cart</h4><button id="closeCart" class="close">×</button></div>
    <div id="cartItems" class="cart-items"></div>
    <div class="cart-footer">
      <div class="cart-total">Total: <span id="cartTotal">$0.00</span></div>
      <a href="checkout.html" class="btn btn-gold">Checkout</a>
    </div>
  </div>

  <script src="app.js"></script>
</body>
</html>
