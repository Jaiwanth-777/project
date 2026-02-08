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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Dribbble Shots</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f5f5f5;
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #2d2d2d;
      color: white;
      padding: 10px 20px;
    }

    .navbar .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .navbar .nav-links,
    .navbar .auth {
      display: flex;
      gap: 15px;
    }

    .navbar a {
      color: white;
      text-decoration: none;
    }

    .sub-header {
      background: #fafafa;
      padding: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    .sub-actions button {
      margin-left: 10px;
      padding: 8px 12px;
      border: 1px solid #ccc;
      background: white;
      cursor: pointer;
    }

    .sign-up {
      background: #ea4c89;
      color: white;
      border: none;
    }

    .filter-bar {
      display: flex;
      gap: 10px;
      padding: 15px 20px;
      background: white;
      border-bottom: 1px solid #ddd;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 20px;
      padding: 20px;
    }

    .card {
      background: white;
      border-radius: 6px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      transition: transform 0.2s;
    }

    .card:hover {
      transform: translateY(-4px);
    }

    .card img {
      width: 100%;
      display: block;
    }

    .card .info {
      padding: 10px;
    }

    .card .author {
      font-weight: bold;
      margin: 0 0 4px;
    }

    .card .stats {
      font-size: 0.8rem;
      color: #666;
      margin: 0;
    }
  </style>
</head>
<body>
  <header class="navbar">
    <div class="logo">Dribbble</div>
    <nav>
      <ul class="nav-links">
        <li><a href="# "> Shots</a></li>
        <li><a href="# "> Designers</a></li>
        <li><a href="# "> Teams</a></li>
        <li><a href="# "> Community</a></li>
        <li><a href="# "> Jobs</a></li>
      </ul>
    </nav>
    <div class="auth">
      <a href="#">Sign up</a>
      <a href="#">Sign in</a>
    </div>
  </header>

  <section class="sub-header">
    <p>What are you working on? <strong>Dribbble</strong> is show and tell for designers.</p>
    <div class="sub-actions">
      <button>Learn more</button>
      <button class="sign-up">Sign up</button>
    </div>
  </section>

  <section class="filter-bar">
    <select><option>Popular</option></select>
    <select><option>Shots</option></select>
    <select><option>Now</option></select>
  </section>

  <main class="grid">
    <!-- Repeat this block for more cards -->
    <div class="card">
      <img src="p1.png" alt="Design shot">
      <div class="info">
        <p class="author">Indhu Priya</p>
        <p class="stats">9,876 views • 14 comments • 290 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p2.png" alt="Design shot">
      <div class="info">
        <p class="author">Praneya</p>
        <p class="stats">2,222 views • 13 comments • 236 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p3.png" alt="Design shot">
      <div class="info">
        <p class="author">James-web desinger</p>
        <p class="stats">3,985 views • 17 comments • 264 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p4.png" alt="Design shot">
      <div class="info">
        <p class="author">Aashika Jain</p>
        <p class="stats">292 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p5.png" alt="Design shot">
      <div class="info">
        <p class="author">Jackson Jhons</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p6.png" alt="Design shot">
      <div class="info">
        <p class="author">Diana</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p7.png" alt="Design shot">
      <div class="info">
        <p class="author">Ronas IT/UV</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p8.png" alt="Design shot">
      <div class="info">
        <p class="author">Chandhana</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p9.png" alt="Design shot">
      <div class="info">
        <p class="author">Mr.Mockup</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p10.png" alt="Design shot">
      <div class="info">
        <p class="author">Md.Harun</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p11.png" alt="Design shot">
      <div class="info">
        <p class="author">Fernia Fender</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <div class="card">
      <img src="p12.png" alt="Design shot">
      <div class="info">
        <p class="author">Adom</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>
    <!-- Add more cards as needed -->
  </main>
</body>
</html>
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/26fc7795-de42-405b-826a-7c382209e6de)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
