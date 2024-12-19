# Project Responsive Web Design using Bootstrap
# Date:16/12/24
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
developed by:sudharsan s


reg no: 24009664

```
home page.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home - Creative Studio</title>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .hero-section {
      background: #343a40;
      color: white;
      padding: 100px 0;
      text-align: center;
    }
    .hero-section h2 {
      font-size: 3rem;
    }
    footer {
      background-color: #343a40;
      color: #fff;
      text-align: center;
      padding: 20px 0;
    }
    .card-body {
      text-align: center;
    }
  </style>
</head>
<body>

<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Creative Studio</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
      <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
      <li class="nav-item"><a class="nav-link" href="services.html">Services</a></li>
      <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
    </ul>
  </div>
</nav>

<!-- Hero Section -->
<div class="hero-section">
  <h2>Welcome to Creative Studio</h2>
  <p>Unleash your creativity with innovative design solutions.</p>
</div>

<div class="container mt-4">
  <h3>Our Work</h3>
  <p>We specialize in bringing your creative vision to life. Our team is passionate about delivering high-quality design solutions that leave a lasting impact.</p>

  <!-- Opening Hours Card -->
  <div class="row mt-4">
    <div class="col-md-4">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Opening Hours</h5>
          <p class="card-text">Monday - Friday: 9:00 AM - 6:00 PM</p>
          <p class="card-text">Saturday: 10:00 AM - 4:00 PM</p>
          <p class="card-text">Sunday: Closed</p>
        </div>
      </div>
    </div>
  </div>

</div>

<footer class="bg-dark text-white mt-5 py-4">
  <div class="container">Developed by Sudharsan S</div>
</footer>

</body>
</html>
```
about us page
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Us - Creative Studio</title>
  <!-- Bootstrap CSS -->
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .navbar { border-bottom: 1px solid rgba(0, 0, 0, 0.1); }
    .navbar-brand { font-weight: bold; }
    .container { padding-top: 20px; }
    footer { background-color: #343a40; color: #fff; }
    @media (max-width: 768px) { .container { padding-top: 60px; } }
    /* Custom image size */
    .about-img {
      max-width: 25%;  /* Adjust the width as needed */
      height: auto;
    }
  </style>
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Creative Studio</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item active">
        <a class="nav-link" href="index.html">Home</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">About</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="services.html">Services</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="contact.html">Contact</a>
      </li>
    </ul>
  </div>
</nav>

<!-- Main Content -->
<div class="container mt-4">
  <h2>About Us</h2>
  <p>Creative Studio is a hub for innovation and artistry. We specialize in delivering top-notch creative solutions for individuals and businesses. Our team of experts is passionate about bringing your vision to life.</p>
  <img src="C:\Users\sudharshan\Downloads\Creative Studio about page image (1).png" alt="Team Collaboration" class="img-fluid mt-4 about-img">
  <p class="mt-4">Whether it's branding, design, or digital marketing, we blend creativity with precision to ensure every project exceeds expectations.</p>
</div>

<!-- Footer -->
<footer class="bg-dark text-white mt-5 py-4">
  <div class="container">
    <p>&copy; 2024 Creative Studio. All rights reserved.</p>
  </div>
</footer>

</body>
</html>
```
service page
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Services - Creative Studio</title>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .service-item {
      margin-bottom: 30px;
    }
    .service-img {
      width: 120px; /* Increased image width */
      height: 120px; /* Increased image height */
      margin-right: 20px;
    }
    .service-description {
      max-width: 80%; /* Limit content width for better readability */
    }
  </style>
</head>
<body>
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Creative Studio</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
      <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
      <li class="nav-item"><a class="nav-link" href="services.html">Services</a></li>
      <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
    </ul>
  </div>
</nav>

<div class="container mt-4">
  <h2>Our Services</h2>
  
  <div class="service-item d-flex align-items-center">
    <img src="C:\Users\sudharshan\Downloads\costume design doing image.png" alt="Custom Designs" class="service-img">
    <div>
      <p><strong>Custom Designs</strong></p>
      <p class="service-description">We offer custom design services tailored to your specific needs. Whether you're looking for a unique branding solution or personalized artwork, our team is ready to bring your vision to life with creativity and precision.</p>
    </div>
  </div>
  
  <div class="service-item d-flex align-items-center">
    <img src="C:\Users\sudharshan\Downloads\Consultations doing image in creative studio.png" alt="Consultations" class="service-img">
    <div>
      <p><strong>Consultations</strong></p>
      <p class="service-description">Our expert consultations provide you with the guidance you need to take your creative projects to the next level. Whether it's design advice, strategy planning, or technical support, we are here to help.</p>
    </div>
  </div>
  
  <div class="service-item d-flex align-items-center">
    <img src="C:\Users\sudharshan\Downloads\Workshops in creative studio.png" alt="Workshops" class="service-img">
    <div>
      <p><strong>Workshops</strong></p>
      <p class="service-description">We offer a variety of workshops to help you hone your creative skills. From design basics to advanced techniques, our hands-on sessions are designed to inspire and educate.</p>
    </div>
  </div>

</div>

<footer class="bg-dark text-white mt-5 py-4">
  <div class="container text-center">Developed by Sudharsan S</div>
</footer>

</body>
</html>
```
contact us page
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Services - Creative Studio</title>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .service-item {
      margin-bottom: 30px;
    }
    .service-img {
      width: 120px; /* Increased image width */
      height: 120px; /* Increased image height */
      margin-right: 20px;
    }
    .service-description {
      max-width: 80%; /* Limit content width for better readability */
    }
  </style>
</head>
<body>
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Creative Studio</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
      <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
      <li class="nav-item"><a class="nav-link" href="services.html">Services</a></li>
      <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
    </ul>
  </div>
</nav>

<div class="container mt-4">
  <h2>Our Services</h2>
  
  <div class="service-item d-flex align-items-center">
    <img src="C:\Users\sudharshan\Downloads\costume design doing image.png" alt="Custom Designs" class="service-img">
    <div>
      <p><strong>Custom Designs</strong></p>
      <p class="service-description">We offer custom design services tailored to your specific needs. Whether you're looking for a unique branding solution or personalized artwork, our team is ready to bring your vision to life with creativity and precision.</p>
    </div>
  </div>
  
  <div class="service-item d-flex align-items-center">
    <img src="C:\Users\sudharshan\Downloads\Consultations doing image in creative studio.png" alt="Consultations" class="service-img">
    <div>
      <p><strong>Consultations</strong></p>
      <p class="service-description">Our expert consultations provide you with the guidance you need to take your creative projects to the next level. Whether it's design advice, strategy planning, or technical support, we are here to help.</p>
    </div>
  </div>
  
  <div class="service-item d-flex align-items-center">
    <img src="C:\Users\sudharshan\Downloads\Workshops in creative studio.png" alt="Workshops" class="service-img">
    <div>
      <p><strong>Workshops</strong></p>
      <p class="service-description">We offer a variety of workshops to help you hone your creative skills. From design basics to advanced techniques, our hands-on sessions are designed to inspire and educate.</p>
    </div>
  </div>

</div>

<footer class="bg-dark text-white mt-5 py-4">
  <div class="container text-center">Developed by Sudharsan S</div>
</footer>

</body>
</html>
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/cadd8995-96b0-402f-bc13-132196f54460)
![image](https://github.com/user-attachments/assets/bdcf6245-0072-4510-9a53-b26f2167969e)
![image](https://github.com/user-attachments/assets/f9f86f8c-e0a2-43c8-ac71-e6ff5cf63b31)
![image](https://github.com/user-attachments/assets/f06d2a4a-6c9d-4e09-9d33-564a35b7b977)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
