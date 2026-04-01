<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SilverGlow - Premium Silver Jewelry Worldwide</title>
    <meta name="description" content="Buy authentic silver jewelry online. Worldwide shipping. High-quality necklaces, rings, earrings & more.">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Arial', sans-serif; line-height: 1.6; color: #333; }
        header { background: linear-gradient(135deg, #c0c0c0, #a9a9a9); padding: 1rem 0; position: fixed; width: 100%; top: 0; z-index: 1000; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        nav { display: flex; justify-content: space-between; align-items: center; max-width: 1200px; margin: 0 auto; padding: 0 2rem; }
        .logo { font-size: 1.8rem; font-weight: bold; color: #fff; text-shadow: 1px 1px 2px rgba(0,0,0,0.3); }
        .nav-links { display: flex; list-style: none; gap: 2rem; }
        .nav-links a { color: #fff; text-decoration: none; font-weight: 500; transition: color 0.3s; }
        .nav-links a:hover { color: #ffd700; }
        .cart-icon { font-size: 1.5rem; color: #fff; cursor: pointer; position: relative; }
        #cart-count { position: absolute; top: -8px; right: -8px; background: #ffd700; color: #333; border-radius: 50%; width: 20px; height: 20px; display: flex; align-items: center; justify-content: center; font-size: 0.8rem; font-weight: bold; }
        .hero { background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1524592094714-0f25c5025c32?ixlib=rb-4.0.3&auto=format&fit=crop&w=2070&q=80') center/cover; height: 100vh; display: flex; align-items: center; justify-content: center; text-align: center; color: #fff; margin-top: 80px; }
        .hero h1 { font-size: 3.5rem; margin-bottom: 1rem; text-shadow: 2px 2px 4px rgba(0,0,0,0.5); }
        .hero p { font-size: 1.3rem; margin-bottom: 2rem; }
        .btn { background: #ffd700; color: #333; padding: 1rem 2rem; text-decoration: none; border-radius: 50px; font-weight: bold; transition: transform 0.3s, box-shadow 0.3s; display: inline-block; }
        .btn:hover { transform: translateY(-3px); box-shadow: 0 10px 20px rgba(255,215,0,0.3); }
        section { padding: 5rem 2rem; max-width: 1200px; margin: 0 auto; }
        h2 { text-align: center; font-size: 2.5rem; margin-bottom: 3rem; color: #555; }
        .products-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 2rem; }
        .product-card { background: #fff; border-radius: 15px; overflow: hidden; box-shadow: 0 10px 30px rgba(0,0,0,0.1); transition: transform 0.3s; }
        .product-card:hover { transform: translateY(-10px); }
        .product-img { width: 100%; height: 250px; object-fit: cover; }
        .product-info { padding: 1.5rem; text-align: center; }
        .product-info h3 { font-size: 1.4rem; margin-bottom: 0.5rem; }
        .price { font-size: 1.8rem; color: #ffd700; font-weight: bold; margin-bottom: 1rem; }
        .add-to-cart { background: #4CAF50; color: white; border: none; padding: 0.8rem 1.5rem; border-radius: 25px; cursor: pointer; font-weight: bold; transition: background 0.3s; }
        .add-to-cart:hover { background: #45a049; }
        #cart-modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.8); z-index: 2000; }
        .modal-content { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); background: #fff; padding: 2rem; border-radius: 15px; max-width: 500px; width: 90%; max-height: 80vh; overflow-y: auto; }
        .close { float: right; font-size: 2rem; cursor: pointer; color: #aaa; }
        .cart-item { display: flex; justify-content: space-between; align-items: center; padding: 1rem 0; border-bottom: 1px solid #eee; }
        .checkout-btn { background: #ffd700; color: #333; border: none; padding: 1rem 2rem; border-radius: 25px; font-weight: bold; cursor: pointer; width: 100%; margin-top: 1rem; }
        .features { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; text-align: center; }
        .feature { padding: 2rem; background: linear-gradient(135deg, #f0f0f0, #e0e0e0); border-radius: 15px; }
        .feature i { font-size: 3rem; color: #c0c0c0; margin-bottom: 1rem; }
        footer { background: #333; color: #fff; text-align: center; padding: 2rem; }
        @media (max-width: 768px) { .nav-links { display: none; } .hero h1 { font-size: 2.5rem; } }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">SilverGlow</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="cart-icon" onclick="toggleCart()">
                <i class="fas fa-shopping-cart"></i>
                <span id="cart-count">0</span>
            </div>
        </nav>
    </header>

    <section id="home" class="hero">
        <div>
            <h1>Premium Silver Jewelry</h1>
            <p>Authentic, Handcrafted Pieces Delivered Worldwide</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>
    </section>

    <section id="products">
        <h2>Featured Collection</h2>
        <div class="products-grid">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1586720818042-1e3daea1c6d2?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Silver Necklace" class="product-img">
                <div class="product-info">
                    <h3>Elegant Silver Necklace</h3>
                    <div class="price">$49.99</div>
                    <button class="add-to-cart" onclick="addToCart('Elegant Silver Necklace', 49.99)">Add to Cart</button>
                </div>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1610992816510-1c685531e9d8?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Silver Ring" class="product-img">
                <div class="product-info">
                    <h3>Classic Silver Ring</h3>
                    <div class="price">$29.99</div>
                    <button class="add-to-cart" onclick="addToCart('Classic Silver Ring', 29.99)">Add to Cart</button>
                </div>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1587563871167-2b3ef2c9f1c2?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Silver Earrings" class="product-img">
                <div class="product-info">
                    <h3>Dainty Silver Earrings</h3>
                    <div class="price">$39.99</div>
                    <button class="add-to-cart" onclick="addToCart('Dainty Silver Earrings', 39.99)">Add to Cart</button>
                </div>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1578662996442-48f60103fc96?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Silver Bracelet" class="product-img">
                <div class="product-info">
                    <h3>Statement Silver Bracelet</h3>
                    <div class="price">$59.99</div>
                    <button class="add-to-cart" onclick="addToCart('Statement Silver Bracelet', 59.99)">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="features" class="features">
        <h2 style="grid-column: 1 / -1;">Why Choose SilverGlow?</h2>
        <div class="feature">
            <i class="fas fa-shipping-fast"></i>
            <h3>Worldwide Shipping</h3>
            <p>Fast & secure delivery to 200+ countries.</p>
        </div>
        <div class="feature">
            <i class="fas fa-shield-alt"></i>
            <h3>100% Authentic</h3>
            <p>925 Sterling Silver, hallmarked & certified.</p>
        </div>
        <div class="feature">
            <i class="fas fa-undo"></i>
            <h3>30-Day Returns</h3>
            <p>Hassle-free returns & exchanges.</p>
        </div>
        <div class="feature">
            <i class="fas fa-credit-card"></i>
            <h3>Secure Payments</h3>
            <p>PayPal, Cards, Crypto accepted.</p>
        </div>
    </section>

    <section id="about">
        <h2>About SilverGlow</h2>
        <p style="text-align: center; font-size: 1.2rem; max-width: 800px; margin: 0 auto;">
            Founded in 2023, SilverGlow brings exquisite handcrafted silver jewelry from artisan workshops to your doorstep. 
            We source the finest 925 sterling silver for timeless pieces that shine worldwide. Join thousands of satisfied customers!
        </p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p style="text-align: center; font-size: 1.2rem;">Ready to glow? Email us at <a href="mailto:hello@silverglow.com">hello@silverglow.com</a> or DM on Instagram @silverglowjewels</p>
    </section>

    <div id="cart-modal">
        <div class="modal-content">
            <span class="close" onclick="toggleCart()">&times;</span>
            <h2>Shopping Cart</h2>
            <div id="cart-items"></div>
            <div id="cart-total" style="font-weight: bold; font-size: 1.2rem; margin: 1rem 0;"></div>
            <button class="checkout-btn" onclick="checkout()">Proceed to Checkout</button>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 SilverGlow. All rights reserved. | Worldwide Shipping | Secure Shopping</p>
    </footer>

    <script>
        let cart = [];

        function addToCart(name, price) {
            cart.push({ name, price });
            updateCartCount();
            alert(`${name} added to cart!`);
        }

        function updateCartCount() {
            document.getElementById('cart-count').textContent = cart.length;
        }

        function toggleCart() {
            const modal = document.getElementById('cart-modal');
            modal.style.display = modal.style.display === 'block' ? 'none' : 'block';
            if (modal.style.display === 'block') renderCart();
        }

        function renderCart() {
            const itemsDiv = document.getElementById('cart-items');
            const totalDiv = document.getElementById('cart-total');
            if (cart.length === 0) {
                itemsDiv.innerHTML = '<p>Your cart is empty.</p>';
                totalDiv.textContent = '';
                return;
            }
            itemsDiv.innerHTML = cart.map((item, index) => `
                <div class="cart-item">
                    <span>${item.name}</span>
                    <span>$${item.price.toFixed(2)} <button onclick="removeFromCart(${index})" style="background:red;color:white;border:none;border-radius:50%;width:25px;height:25px;cursor:pointer;">&times;</button></span>
                </div>
            `).join('');
            const total = cart.reduce((sum, item) => sum + item.price, 0);
            totalDiv.textContent = `Total: $${total.toFixed(2)}`;
        }

        function removeFromCart(index) {
            cart.splice(index, 1);
            updateCartCount();
            renderCart();
        }

        function checkout() {
            if (cart.length === 0) return alert('Cart is empty!');
            alert('Thanks for your order! (Demo - Integrate real payment gateway next.)');
            cart = [];
            updateCartCount();
            toggleCart();
        }

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
            });
        });

        // Close modal on outside click
        window.onclick = function(event) {
            const modal = document.getElementById('cart-modal');
            if (event.target === modal) toggleCart();
        }
    </script>
</body>
</html>
