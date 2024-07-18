# Ecommerce-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-Commerce Website</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="products.html">Products</a></li>
                <li><a href="cart.html">Cart</a></li>
                <li><a href="checkout.html">Checkout</a></li>
            </ul>
        </nav>
        <h1>Welcome to Our E-Commerce Store!</h1>
    </header>
    <main>
        <section>
            <h2>Featured Products</h2>
            <div class="product">
                <img src="images/product1.jpg" alt="Product 1">
                <h3>Product Title 1</h3>
                <p>$10.00</p>
                <button>Add to Cart</button>
            </div>
            <div class="product">
                <img src="images/product2.jpg" alt="Product 2">
                <h3>Product Title 2</h3>
                <p>$20.00</p>
                <button>Add to Cart</button>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 E-Commerce Store. All rights reserved.</p>
    </footer>
    <script src="js/scripts.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Products</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="products.html">Products</a></li>
                <li><a href="cart.html">Cart</a></li>
                <li><a href="checkout.html">Checkout</a></li>
            </ul>
        </nav>
        <h1>Our Products</h1>
    </header>
    <main>
        <section>
            <div class="product">
                <img src="images/product1.jpg" alt="Product 1">
                <h3>Product Title 1</h3>
                <p>$10.00</p>
                <button>Add to Cart</button>
            </div>
            <div class="product">
                <img src="images/product2.jpg" alt="Product 2">
                <h3>Product Title 2</h3>
                <p>$20.00</p>
                <button>Add to Cart</button>
            </div>
            <!-- Add more products as needed -->
        </section>
    </main>
    <footer>
        <p>&copy; 2024 E-Commerce Store. All rights reserved.</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shopping Cart</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="products.html">Products</a></li>
                <li><a href="cart.html">Cart</a></li>
                <li><a href="checkout.html">Checkout</a></li>
            </ul>
        </nav>
        <h1>Shopping Cart</h1>
    </header>
    <main>
        <section>
            <h2>Your Cart</h2>
            <div class="cart-item">
                <img src="images/product1.jpg" alt="Product 1">
                <h3>Product Title 1</h3>
                <p>$10.00</p>
                <input type="number" value="1" min="1">
                <button>Remove</button>
            </div>
            <!-- Add more cart items as needed -->
            <div class="total">
                <h3>Total: $10.00</h3>
                <button><a href="checkout.html">Proceed to Checkout</a></button>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 E-Commerce Store. All rights reserved.</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Checkout</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="products.html">Products</a></li>
                <li><a href="cart.html">Cart</a></li>
                <li><a href="checkout.html">Checkout</a></li>
            </ul>
        </nav>
        <h1>Checkout</h1>
    </header>
    <main>
        <section>
            <h2>Billing Information</h2>
            <form action="submit_order.php" method="post">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                <label for="address">Address:</label>
                <input type="text" id="address" name="address" required>
                <label for="city">City:</label>
                <input type="text" id="city" name="city" required>
                <label for="state">State:</label>
                <input type="text" id="state" name="state" required>
                <label for="zip">Zip Code:</label>
                <input type="text" id="zip" name="zip" required>
                <button type="submit">Place Order</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 E-Commerce Store. All rights reserved.</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 20px;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

.product, .cart-item {
    margin: 20px 0;
    border: 1px solid #ccc;
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.product img, .cart-item img {
    max-width: 100px;
    height: auto;
}

.total {
    margin-top: 20px;
    text-align: right;
}

form {
    display: flex;
    flex-direction: column;
}

form label {
    margin: 10px 0 5px;
}

form input {
    padding: 10px;
    margin-bottom: 10px;
}

form button {
    padding: 10px;
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
}

form button a {
    color: white;
    text-decoration
