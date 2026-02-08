# Project Responsive Web Design using Bootstrap
# Date:
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Online Store</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" />
  <style>
    .hero {
      background: url("{% static 'image.png' %}") center/cover no-repeat;
      background-size: auto;
      color: rgb(246, 5, 109);
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    .product-card:hover {
      transform: scale(1.03);
      transition: 0.3s;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }

    .offer-banner {
      background-color: #ffc107;
      color: #000;
      padding: 20px;
      text-align: center;
      font-size: 1.25rem;
      font-weight: bold;
    }
    footer {
      background-color: #343a40;
      color: #fff;
      padding: 20px 0;
      text-align: center;
    }
  </style>
</head>
<body>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container">
      <a class="navbar-brand">ZEBRONICS</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#products">Products</a></li>
        </ul>
      </div>
    </div>
  </nav>
  <section class="hero">
    <div class="container">
      <div class="content">
      <br><br><br><br><br><br><br><br><br><br><br>
      <h1>Welcome to Zebronics</h1>
      <p>Click shop now for amazing products!</p>
      <a href="#products" class="btn btn-warning mt-3">Shop Now</a>
      </div>
    </div>
  </section>
  <div class="offer-banner">
    !! Limited Time Offer: Get up to 50% off on selected items!
  </div>
  <section id="products" class="py-5">
    <div class="container">
      <h2 class="mb-4 text-center">Our Products</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card product-card">
            <img src="{% static 'lap.png' %}" class="card-img-top" alt="Product 1">
            <div class="card-body">
              <h5 class="card-title">ZEBRONICS NBC 5S</h5>
              <p class="card-text">$796/Rs.70,000</p>
              <button class="btn btn-primary add-to-cart" data-product="Product One">Add to Cart</button>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card product-card">
            <img src="{% static 'hp.png' %}"height="390px" width="225px" class="card-img-top" alt="Product 2">
            <div class="card-body">
              <h5 class="card-title">ZEBRONICS THUNDER PRO WIRELESS HEADPHONES</h5>
              <p class="card-text">$34/Rs.3,000</p>
              <button class="btn btn-primary add-to-cart" data-product="Product Two">Add to Cart</button>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card product-card">
            <img src="{% static 'key.png' %}" height="415px" width="420px" class="card-img-top" alt="Product 3">
            <div class="card-body">
              <h5 class="card-title">ZEBRONICS NITRO PLUS KEYBOARD</h5>
              <p class="card-text">$11.3/Rs.1,000</p>
              <button class="btn btn-primary add-to-cart" data-product="Product Three">Add to Cart</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section class="py-5 bg-light">
    <div class="container">
      <h3>Your Cart</h3>
      <ul id="cart-list" class="list-group mb-3">
        <li class="list-group-item">No items in cart.</li>
      </ul>
      <p><strong>Total Items:</strong> <span id="cart-count">0</span></p>
    </div>
  </section>
  <footer>
    <div class="container">
      <h4>2025 ZEBRONICS. ALL RIGHTS RESERVED.</h4>
    </div>
  </footer>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
  <script>
    const cart = {};
    const cartList = document.getElementById('cart-list');
    const cartCount = document.getElementById('cart-count');

    document.querySelectorAll('.add-to-cart').forEach(button => {
      button.addEventListener('click', () => {
        const product = button.getAttribute('data-product');
        cart[product] = (cart[product] || 0) + 1;
        updateCart();
      });
    });

    function updateCart() {
      cartList.innerHTML = '';
      let total = 0;

      for (const [product, quantity] of Object.entries(cart)) {
        const li = document.createElement('li');
        li.className = 'list-group-item d-flex justify-content-between align-items-center';
        li.innerHTML = `
          <span>${product}</span>
          <span class="badge bg-primary rounded-pill">${quantity}</span>
        `;
        cartList.appendChild(li);
        total += quantity;
      }

      if (total === 0) {
        cartList.innerHTML = '<li class="list-group-item">No items in cart.</li>';
      }

      cartCount.textContent = total;
    }
  </script>
</body>
</html>
```
# OUTPUT:

![alt text](<Screenshot 2025-10-11 190851.png>)
![alt text](<Screenshot 2025-10-11 190932.png>)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
