# Project Responsive Web Design using Bootstrap
# Date:23/12/24
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
    <title>Dribbble Clone - Home</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .navbar {
            background-color: #3c3c3c;
        }
        .navbar-dark .navbar-nav .nav-link {
            color: #fff;
            margin-right: 15px;
        }
        .navbar-dark .navbar-brand {
            color: #fff;
            font-weight: bold;
        }
        .cta-btn {
            color: #fff;
            font-size: 0.9rem;
        }
        .btn-learn-more {
            background-color: #e0e0e0;
            color: #000;
        }
        .btn-sign-up {
            background-color: #ea4c89;
            color: #fff;
        }
        .form-control {
            max-width: 200px;
        }
        .footer {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
        }
        .image-gallery {
            padding: 60px 0;
        }
        .image-gallery img {
            width: 100%;
            height: auto;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link" href="#">Shots</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Community</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
                </ul>
                <div class="d-flex align-items-center">
                    <button class="btn btn-learn-more me-2 cta-btn">Learn more</button>
                    <button class="btn btn-sign-up me-2 cta-btn">Sign up</button>
                    <button class="btn btn-outline-light me-3 cta-btn">Sign in</button>
                    <input type="text" class="form-control" placeholder="Search">
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="bg-light py-5 text-center">
        <div class="container">
            <h1 class="mb-3">What are you working on?</h1>
            <p>Dribbble is show and tell for designers.</p>
            <a href="#" class="btn btn-primary btn-lg">Learn more</a>
            <a href="#" class="btn btn-danger btn-lg">Sign up</a>
        </div>
    </section>

    <!-- Image Gallery Section -->
    <section class="image-gallery text-center">
        <div class="container">
            <div class="row">
                <div class="col-md-3 mb-4">
                    <img src="C:\Users\sudharshan\OneDrive\Pictures\Screenshots\Screenshot 2024-12-21 181559.png" alt="Image 1">
                </div>
                <div class="col-md-3 mb-4">
                    <img src="C:\Users\sudharshan\OneDrive\Pictures\Screenshots\Screenshot 2024-12-21 181553.png"alt="Image 2">
                </div>
                <div class="col-md-3 mb-4">
                    <img src="C:\Users\sudharshan\OneDrive\Pictures\Screenshots\Screenshot 2024-12-21 181548.png" alt="Image 3">
                </div>
                <div class="col-md-3 mb-4">
                    <img src="C:\Users\sudharshan\OneDrive\Pictures\Screenshots\Screenshot 2024-12-21 181544.png" alt="Image 4">
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer text-center">
        <div class="container">
            <p>Designed by Sudharsan &copy; 2024</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
shots.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shots - Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .navbar {
            background-color: #3c3c3c;
        }
        .navbar-dark .navbar-nav .nav-link {
            color: #fff;
            margin-right: 15px;
        }
        .navbar-dark .navbar-brand {
            color: #fff;
            font-weight: bold;
        }
        .footer {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
        }
        .shot-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
            background-color: #fff;
        }
        .shot-card img {
            width: 100%;
            height: auto;
            border-radius: 8px;
        }
        .shot-card h5 {
            font-size: 1.25rem;
            margin-top: 15px;
        }
        .shot-card p {
            font-size: 1rem;
        }
        .view-details-btn {
            background-color: #ea4c89;
            color: #fff;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
        }
        .view-details-btn:hover {
            background-color: #d13972;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="shots.html">Shots</a></li>
                    <li class="nav-item"><a class="nav-link" href="designers.html">Designers</a></li>
                    <li class="nav-item"><a class="nav-link" href="teams.html">Teams</a></li>
                    <li class="nav-item"><a class="nav-link" href="community.html">Community</a></li>
                    <li class="nav-item"><a class="nav-link" href="jobs.html">Jobs</a></li>
                </ul>
                <div class="d-flex align-items-center">
                    <button class="btn btn-outline-light me-3">Sign up</button>
                    <button class="btn btn-outline-light">Sign in</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Shots Section -->
    <section class="py-5">
        <div class="container text-center">
            <h1>Latest Shots</h1>
            <p>Explore the latest design shots and get inspired by talented creatives from around the world.</p>

            <!-- Shots Showcase -->
            <div class="row">
                <div class="col-md-4">
                    <div class="shot-card">
                        <img src="C:\Users\sudharshan\Downloads\Minimalistic UI Design.png" alt="Shot 1">
                        <h5>Minimalistic UI Design</h5>
                        <p>A sleek and simple UI design focused on minimalism, with a clean layout and modern typography.</p>
                        <a href="#" class="view-details-btn">View Details</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="shot-card">
                        <img src="C:\Users\sudharshan\Downloads\Creative Logo Concept.png" alt="Shot 2">
                        <h5>Creative Logo Concept</h5>
                        <p>This logo design explores modern abstract shapes to create a unique and memorable brand identity.</p>
                        <a href="#" class="view-details-btn">View Details</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="shot-card">
                        <img src="C:\Users\sudharshan\Downloads\Mobile App Design.png" alt="Shot 3">
                        <h5>Mobile App Design</h5>
                        <p>A clean, user-friendly mobile app design that focuses on easy navigation and intuitive interaction.</p>
                        <a href="#" class="view-details-btn">View Details</a>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-md-4">
                    <div class="shot-card">
                        <img src="C:\Users\sudharshan\Downloads\Website Redesign.png" alt="Shot 4">
                        <h5>Website Redesign</h5>
                        <p>This project showcases a fresh redesign for a website, focusing on enhancing the user experience.</p>
                        <a href="#" class="view-details-btn">View Details</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="shot-card">
                        <img src="C:\Users\sudharshan\Downloads\Branding & Packaging.png" alt="Shot 5">
                        <h5>Branding & Packaging</h5>
                        <p>Beautiful and functional packaging design, reflecting the brand's values and personality.</p>
                        <a href="#" class="view-details-btn">View Details</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="shot-card">
                        <img src="C:\Users\sudharshan\Downloads\Illustration Art.png" alt="Shot 6">
                        <h5>Illustration Art</h5>
                        <p>Vibrant and colorful illustrations created to convey powerful messages through art.</p>
                        <a href="#" class="view-details-btn">View Details</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer text-center">
        <div class="container">
            <p>Designed by Sudharsan &copy; 2024</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

designer.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Designers - Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .navbar {
            background-color: #3c3c3c;
        }
        .navbar-dark .navbar-nav .nav-link {
            color: #fff;
            margin-right: 15px;
        }
        .navbar-dark .navbar-brand {
            color: #fff;
            font-weight: bold;
        }
        .footer {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
        }
        .designer-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
            background-color: #fff;
        }
        .designer-card img {
            width: 100%;
            height: auto;
            border-radius: 8px;
        }
        .designer-card h5 {
            font-size: 1.25rem;
            margin-top: 15px;
        }
        .designer-card p {
            font-size: 1rem;
        }
        .view-portfolio-btn {
            background-color: #ea4c89;
            color: #fff;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
        }
        .view-portfolio-btn:hover {
            background-color: #d13972;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="shots.html">Shots</a></li>
                    <li class="nav-item"><a class="nav-link" href="designers.html">Designers</a></li>
                    <li class="nav-item"><a class="nav-link" href="teams.html">Teams</a></li>
                    <li class="nav-item"><a class="nav-link" href="community.html">Community</a></li>
                    <li class="nav-item"><a class="nav-link" href="jobs.html">Jobs</a></li>
                </ul>
                <div class="d-flex align-items-center">
                    <button class="btn btn-outline-light me-3">Sign up</button>
                    <button class="btn btn-outline-light">Sign in</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Designers Section -->
    <section class="py-5">
        <div class="container text-center">
            <h1>Featured Designers</h1>
            <p>Discover talented designers and explore their portfolios. Get inspired by their work and connect with them.</p>

            <!-- Designers Showcase -->
            <div class="row">
                <div class="col-md-4">
                    <div class="designer-card">
                        <img src="C:\Users\sudharshan\Downloads\male UI_UX Designer male guy working.png"alt="Designer 1">
                        <h5>Jane Doe</h5>
                        <p>UI/UX Designer | Specializing in web and mobile interfaces. Passionate about creating user-friendly designs with a focus on functionality.</p>
                        <a href="#" class="view-portfolio-btn">View Portfolio</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="designer-card">
                        <img src="C:\Users\sudharshan\Downloads\male graphic designer.png" alt="Designer 2">
                        <h5>John Smith</h5>
                        <p>Graphic Designer | Expert in brand identity and visual storytelling. Transforming ideas into beautiful designs.</p>
                        <a href="#" class="view-portfolio-btn">View Portfolio</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="designer-card">
                        <img src="C:\Users\sudharshan\Downloads\Freelance Designer female.png" alt="Designer 3">
                        <h5>Alice Johnson</h5>
                        <p>Freelance Designer | Creating innovative graphics and illustrations. Striving to push the boundaries of creativity.</p>
                        <a href="#" class="view-portfolio-btn">View Portfolio</a>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <!-- Footer -->
    <footer class="footer text-center">
        <div class="container">
            <p>Designed by Sudharsan &copy; 2024</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

jobs.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jobs - Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .navbar {
            background-color: #3c3c3c;
        }
        .navbar-dark .navbar-nav .nav-link {
            color: #fff;
            margin-right: 15px;
        }
        .navbar-dark .navbar-brand {
            color: #fff;
            font-weight: bold;
        }
        .footer {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
        }
        .job-card {
            margin-bottom: 30px;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .job-card img {
            width: 80px;
            height: 80px;
            object-fit: cover;
            border-radius: 50%;
        }
        .job-card .card-body {
            padding-left: 20px;
        }
        .job-card h5 {
            font-size: 1.25rem;
        }
        .job-card p {
            font-size: 1rem;
        }
        .apply-btn {
            background-color: #ea4c89;
            color: #fff;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
        }
        .apply-btn:hover {
            background-color: #d13972;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="shots.html">Shots</a></li>
                    <li class="nav-item"><a class="nav-link" href="designers.html">Designers</a></li>
                    <li class="nav-item"><a class="nav-link" href="teams.html">Teams</a></li>
                    <li class="nav-item"><a class="nav-link" href="community.html">Community</a></li>
                    <li class="nav-item"><a class="nav-link" href="jobs.html">Jobs</a></li>
                </ul>
                <div class="d-flex align-items-center">
                    <button class="btn btn-outline-light me-3">Sign up</button>
                    <button class="btn btn-outline-light">Sign in</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Jobs Section -->
    <section class="py-5">
        <div class="container text-center">
            <h1>Job Opportunities</h1>
            <p>Explore exciting job opportunities for designers and creatives. Find your next role and join a creative team today!</p>
            
            <!-- Job Listings -->
            <div class="row">
                <div class="col-md-4">
                    <div class="card job-card">
                        <div class="d-flex align-items-center">
                            <img src="C:\Users\sudharshan\Downloads\UI_UX Designer company logo.png" alt="Company Logo">
                            <div class="card-body">
                                <h5 class="card-title">UI/UX Designer</h5>
                                <p class="card-text">Join our dynamic team as a UI/UX Designer to create engaging digital experiences for our products.</p>
                                <a href="#" class="apply-btn">Apply Now</a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card job-card">
                        <div class="d-flex align-items-center">
                            <img src="C:\Users\sudharshan\Downloads\Graphic Designer company logo.png" alt="Company Logo">
                            <div class="card-body">
                                <h5 class="card-title">Graphic Designer</h5>
                                <p class="card-text">We are looking for a talented Graphic Designer to help us create visual content for our campaigns.</p>
                                <a href="#" class="apply-btn">Apply Now</a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card job-card">
                        <div class="d-flex align-items-center">
                            <img src="C:\Users\sudharshan\Downloads\Web Designer company logo.png" alt="Company Logo">
                            <div class="card-body">
                                <h5 class="card-title">Web Designer</h5>
                                <p class="card-text">Help us design and develop interactive websites by joining our growing team as a Web Designer.</p>
                                <a href="#" class="apply-btn">Apply Now</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer text-center">
        <div class="container">
            <p>Designed by Sudharsan &copy; 2024</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

community.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Community - Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .navbar {
            background-color: #3c3c3c;
        }
        .navbar-dark .navbar-nav .nav-link {
            color: #fff;
            margin-right: 15px;
        }
        .navbar-dark .navbar-brand {
            color: #fff;
            font-weight: bold;
        }
        .footer {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
        }
        .community-card {
            margin-bottom: 30px;
        }
        .community-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        .community-card .card-body {
            text-align: center;
        }
        .community-card h5 {
            font-size: 1.25rem;
            margin-top: 15px;
        }
        .community-card p {
            font-size: 1rem;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="teams.html">Teams</a></li>
                    <li class="nav-item"><a class="nav-link" href="community.html">Community</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
                </ul>
                <div class="d-flex align-items-center">
                    <button class="btn btn-outline-light me-3">Sign up</button>
                    <button class="btn btn-outline-light">Sign in</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Community Section -->
    <section class="py-5 text-center">
        <div class="container">
            <h1>Community</h1>
            <p>Join the vibrant community of designers and creatives. Connect, share, and grow together.</p>
            
            <!-- Community Cards -->
            <div class="row">
                <div class="col-md-4">
                    <div class="card community-card">
                        <img src="C:\Users\sudharshan\Downloads\Creative Meetup team image.png" alt="Event Image 1">
                        <div class="card-body">
                            <h5 class="card-title">Creative Meetup</h5>
                            <p class="card-text">Join our monthly meetup where creatives gather to share ideas, collaborate, and inspire each other.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card community-card">
                        <img src="C:\Users\sudharshan\Downloads\Design Challenges team.png" alt="Event Image 2">
                        <div class="card-body">
                            <h5 class="card-title">Design Challenges</h5>
                            <p class="card-text">Participate in exciting design challenges and showcase your skills to the community.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card community-card">
                        <img src="C:\Users\sudharshan\Downloads\Workshops & Tutorials team image.png" alt="Event Image 3">
                        <div class="card-body">
                            <h5 class="card-title">Workshops & Tutorials</h5>
                            <p class="card-text">Learn from industry experts in our hands-on workshops and tutorials, designed to level up your skills.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Community Overview -->
            <div class="my-5">
                <h3>About the Dribbble Community</h3>
                <p>The Dribbble community is made up of designers, developers, and other creatives who come together to share work, ideas, and opportunities. Whether you’re a designer, developer, or someone with a passion for creativity, there’s a place for you here. Our community fosters collaboration, learning, and inspiration across the globe.</p>
                <a href="#" class="btn btn-primary btn-lg">Join the Community</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer text-center">
        <div class="container">
            <p>Designed by Sudharsan &copy; 2024</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

team.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teams - Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .navbar {
            background-color: #3c3c3c;
        }
        .navbar-dark .navbar-nav .nav-link {
            color: #fff;
            margin-right: 15px;
        }
        .navbar-dark .navbar-brand {
            color: #fff;
            font-weight: bold;
        }
        .footer {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
        }
        .team-card {
            margin-bottom: 30px;
        }
        .team-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        .team-card .card-body {
            text-align: center;
        }
        .team-card h5 {
            font-size: 1.25rem;
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="shots.html">Shots</a></li>
                    <li class="nav-item"><a class="nav-link" href="designers.html">Designers</a></li>
                    <li class="nav-item"><a class="nav-link" href="teams.html">Teams</a></li>
                    <li class="nav-item"><a class="nav-link" href="community.html">Community</a></li>
                    <li class="nav-item"><a class="nav-link" href="jobs.html">Jobs</a></li>
                </ul>
                <div class="d-flex align-items-center">
                    <button class="btn btn-outline-light me-3">Sign up</button>
                    <button class="btn btn-outline-light">Sign in</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Teams Section -->
    <section class="py-5 text-center">
        <div class="container">
            <h1>Teams</h1>
            <p>Explore creative teams and their inspiring work on Dribbble.</p>
            
            <!-- Team Cards -->
            <div class="row">
                <div class="col-md-4">
                    <div class="card team-card">
                        <img src="C:\Users\sudharshan\Downloads\wizard designing team image.png" alt="Team Image 1">
                        <div class="card-body">
                            <h5 class="card-title">Design Wizards</h5>
                            <p class="card-text">A team of highly creative designers who specialize in UI/UX and branding projects.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card team-card">
                        <img src="C:\Users\sudharshan\Downloads\A team working on a project.png" alt="Team Image 2">
                        <div class="card-body">
                            <h5 class="card-title">Pixel Pioneers</h5>
                            <p class="card-text">Pixel-perfect design experts creating stunning visual experiences for global brands.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card team-card">
                        <img src="C:\Users\sudharshan\Downloads\innovative team image.png" alt="Team Image 3">
                        <div class="card-body">
                            <h5 class="card-title">Innovative Creations</h5>
                            <p class="card-text">A creative team that focuses on innovative design strategies for web and mobile applications.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Team Overview -->
            <div class="my-5">
                <h3>About Our Teams</h3>
                <p>Our teams are at the forefront of design innovation. From UI/UX designers to branding specialists, our members bring fresh ideas to every project. Join us in discovering the most talented and creative teams that shape the digital world.</p>
                <a href="#" class="btn btn-primary btn-lg">View More Teams</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer text-center">
        <div class="container">
            <p>Designed by Sudharsan &copy; 2024</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

OUTPUT#:
![Screenshot 2024-12-21 183316](https://github.com/user-attachments/assets/2b3f44db-4117-420b-aca3-d17e982580ea)
![Screenshot 2024-12-21 185313](https://github.com/user-attachments/assets/79a1838c-4f91-4480-8be7-0f7cd359c483)
![Screenshot 2024-12-21 185702](https://github.com/user-attachments/assets/6263fc56-35e6-418e-9bf1-d5b70330c360)
![Screenshot 2024-12-21 190443](https://github.com/user-attachments/assets/b3c8bde5-5aa2-42fb-9c19-73c33560283b)
![Screenshot 2024-12-21 192923](https://github.com/user-attachments/assets/176552e3-fda4-4351-9db6-c05365bc8a83)
![Screenshot 2024-12-21 193520](https://github.com/user-attachments/assets/ba829afc-3cf0-4778-96ea-bdca1652401b)


# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
