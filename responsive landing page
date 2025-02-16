 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coffee Shop</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f5f5f5;
        }

        /* Navigation Styles */
        .nav-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: #2c3e50;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            z-index: 1000;
        }

        .nav-menu {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0;
            list-style: none;
            display: flex;
            justify-content: center;
            position: relative; /* Added for dropdown containment */
        }

        .nav-menu li {
            position: relative;
            padding: 0;
            margin: 0;
        }

        .nav-menu a {
            display: block;
            padding: 1.5rem 2rem;
            text-decoration: none;
            color: #ecf0f1;
            font-weight: 500;
            transition: all 0.3s ease;
            white-space: nowrap; /* Prevent text wrapping */
        }

        /* Dropdown Styles */
        .dropdown {
            position: absolute;
            top: 100%;
            left: 50%;
            transform: translateX(-50%) translateY(-10px);
            background-color: #34495e;
            min-width: 200px;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            border-radius: 0 0 4px 4px;
            z-index: 1001; /* Ensure dropdown stays above other content */
        }

        /* Adjust dropdown position for first and last items */
        .nav-menu li:first-child .dropdown {
            left: 0;
            transform: translateY(-10px);
        }

        .nav-menu li:last-child .dropdown {
            left: auto;
            right: 0;
            transform: translateY(-10px);
        }

        .nav-menu li:hover .dropdown {
            opacity: 1;
            visibility: visible;
            transform: translateX(-50%) translateY(0);
        }

        /* Adjust hover state for first and last items */
        .nav-menu li:first-child:hover .dropdown {
            transform: translateY(0);
        }

        .nav-menu li:last-child:hover .dropdown {
            transform: translateY(0);
        }

        .dropdown a {
            padding: 1rem 2rem;
            font-size: 0.95em;
            border-bottom: 1px solid rgba(236, 240, 241, 0.1);
        }

        .dropdown a:hover {
            background-color: #2c3e50;
            color: #3498db;
            padding-left: 2.5rem;
        }

        .nav-menu > li > a:hover {
            background-color: #34495e;
            color: #3498db;
        }

        /* Scrolled state */
        .nav-container.scrolled {
            background-color: #34495e;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        .nav-container.scrolled .nav-menu > li > a {
            padding: 1rem 2rem;
            font-size: 0.95em;
        }

        /* Menu Section Styles */
        .menu-section {
            margin-top: 100px;
            padding: 2rem;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
        }

        .menu-title {
            text-align: center;
            font-size: 2.5rem;
            color: #2c3e50;
            margin-bottom: 2rem;
            font-weight: bold;
        }

        /* Arrow indicator for dropdown */
        .nav-menu > li > a::after {
            content: '▼';
            margin-left: 8px;
            font-size: 0.8em;
            transition: transform 0.3s ease;
        }

        .nav-menu > li:hover > a::after {
            transform: rotate(-180deg);
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="nav-container">
        <ul class="nav-menu">
            <li>
                <a href="#home">Home</a>
                <div class="dropdown">
                    <a href="#welcome">Welcome</a>
                    <a href="#featured">Featured Items</a>
                    <a href="#special">Today's Special</a>
                </div>
            </li>
            <li>
                <a href="#about">About</a>
                <div class="dropdown">
                    <a href="#story">Our Story</a>
                    <a href="#team">Our Team</a>
                    <a href="#values">Values</a>
                    <a href="#sourcing">Coffee Sourcing</a>
                </div>
            </li>
            <li>
                <a href="#menu">Menu</a>
                <div class="dropdown">
                    <a href="#hot-drinks">Hot Drinks</a>
                    <a href="#cold-drinks">Cold Drinks</a>
                    <a href="#pastries">Pastries</a>
                    <a href="#seasonal">Seasonal Items</a>
                </div>
            </li>
            <li>
                <a href="#locations">Locations</a>
                <div class="dropdown">
                    <a href="#downtown">Downtown</a>
                    <a href="#uptown">Uptown</a>
                    <a href="#suburb">Suburb</a>
                    <a href="#new-locations">Coming Soon</a>
                </div>
            </li>
            <li>
                <a href="#contact">Contact</a>
                <div class="dropdown">
                    <a href="#support">Support</a>
                    <a href="#feedback">Feedback</a>
                    <a href="#careers">Careers</a>
                    <a href="#partnerships">Partnerships</a>
                </div>
            </li>
        </ul>
    </nav>

    <!-- Content Section -->
    <section class="menu-section">
        <h1 class="menu-title">Welcome to Our Coffee Shop</h1>
        <p style="text-align: center; color: #666;">Hover over the navigation items to see the dropdowns!</p>
    </section>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const nav = document.querySelector('.nav-container');
            const scrollThreshold = 50;

            // Handle scroll events
            window.addEventListener('scroll', () => {
                if (window.scrollY > scrollThreshold) {
                    nav.classList.add('scrolled');
                } else {
                    nav.classList.remove('scrolled');
                }
            });
        });
    </script>
</body>
</html>
