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

```<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribbble Simplified Clone</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Navigation Bar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Dribbble</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#">Explore</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Blog</a></li>
          <li class="nav-item"><a class="nav-link text-primary" href="#">Sign Up</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Log In</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="hero-section text-center text-white d-flex align-items-center justify-content-center">
    <div class="container">
      <h1 class="display-4 fw-bold">WORLD OF NATURE</h1>
      <p class="lead">The world of nature is a vast, interconnected web of life, where every plant, animal, and ecosystem plays a vital role in maintaining balance. From the towering trees in lush forests to the depths of the oceans, nature is a constant source of wonder and inspiration</p>
    <form class="d-flex justify-content-center mt-3">
        <input type="text" class="form-control w-50" placeholder="Search" />
      </form>
    </div>
  </header>

  <!-- Trending Searches Section -->
  <section class="py-5 text-center">
    <div class="container">
      <h2>Trending Searches</h2>
      <div class="d-flex flex-wrap justify-content-center mt-3">
        <a href="#" class="btn btn-primary m-1">Nature</a>
        <a href="#" class="btn btn-outline-primary m-1">Untouched paradise</a>
        <a href="#" class="btn btn-outline-primary m-1">Tranquil</a>
        <a href="#" class="btn btn-outline-primary m-1">Vibrant</a>
        <a href="#" class="btn btn-outline-primary m-1">Scenery</a>
        <a href="#" class="btn btn-outline-primary m-1">Amber-hued</a>
      </div>
    </div>
  </section>

  <!-- Featured Designs Section -->
  <section class="py-5 bg-light">
    <div class="container">
      <div class="row g-4">
        <!-- Example Card -->
        <div class="col-md-4">
            <div class="card shadow-sm">
              <img src="autumn.jpg" class="card-img-top" alt="Northern Lights">
              <div class="card-body">
                <h5 class="card-title">Northern Light</h5>
                <p class="card-text text-muted">Emote Team | 7.2k Views</p>
              </div>
            </div>
          </div>
        <div class="col-md-4">
          <div class="card shadow-sm">
            <img src="misty.jpg" class="card-img-top" alt="Falls">
            <div class="card-body">
              <h5 class="card-title">Falls</h5>
              <p class="card-text text-muted">Emote Team | 8.2k Views</p>
            </div>
          </div>
        </div>
        <!-- Repeat for other cards -->
        <div class="col-md-4">
          <div class="card shadow-sm">
            <img src="beach.jpg" class="card-img-top" alt="Beach">
            <div class="card-body">
              <h5 class="card-title">Beach</h5>
              <p class="card-text text-muted">Emote Team | 9.2k Views</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card shadow-sm">
            <img src="mountains.jpg" class="card-img-top" alt="Flight">
            <div class="card-body">
              <h5 class="card-title">Flight</h5>
              <p class="card-text text-muted">Emote Team | 5.2k Views</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
            <div class="card shadow-sm">
              <img src="rain.jpg" class="card-img-top" alt="Mountain">
              <div class="card-body">
                <h5 class="card-title">Mountain</h5>
                <p class="card-text text-muted">Emote Team | 100k Views</p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card shadow-sm">
              <img src="thunder.jpg" class="card-img-top" alt="Flower">
              <div class="card-body">
                <h5 class="card-title">Flower</h5>
                <p class="card-text text-muted">Emote Team | 105k Views</p>
              </div>
            </div>
          </div>
        <!-- Add more cards -->
      </div>
    </div>
  </section>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/6a045484-eba7-4832-a703-469bb2bcf43f)

![image](![egejgljere](https://github.com/user-attachments/assets/f443eeb5-a958-487f-b60f-b4b63e6dfd7c)


# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
