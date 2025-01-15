<!DOCTYPE html>
<html lang="en">
<head>
    
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Navigation Menu</title>
    <style>
        body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: #333;
    transition: background-color 0.3s, color 0.3s;
}

.navbar ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: space-around;
}

.navbar li {
    padding: 15px 20px;
}

.navbar a {
    color: white;
    text-decoration: none;
    transition: color 0.3s;
}

.navbar a:hover {
    color: #ff6347; /* Change color on hover */
}

.scrolled {
    background-color: #555; /* Background color when scrolled */
}

.content {
    margin-top: 60px; /* Space for fixed navbar */
}

    </style>
</head>
<<!doctype html>
<html lang="en">

<head>
    <!--MY Navigation HTML CODE-->
<body>

    <nav class="navbar" id="navbar">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <div class="content">
        <h1>Welcome to Our Website</h1>
        <p>Scroll down to see the effect on the navigation menu.</p>
        <div style="height: 1500px;"></div> <!-- Just to create scrollable content -->
    </div>
<!--JAVASCRIPT-->
    <script>window.onscroll = function() {
        var navbar = document.getElementById("navbar");
        
        if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
            navbar.classList.add("scrolled");
        } else {
            navbar.classList.remove("scrolled");
        }
    };
    </script>
</body>
</html>

