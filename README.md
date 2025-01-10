# FullStack_Portal
#This project aims to create a system for managing and displaying student details efficiently. It includes             dynamic data retrieval, search and filter functionality, and interactive features like calling #and messaging             directly from the interface.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom right, #f7f7f7, #e3e3e3);
            color: #333;
        }
        #splash-screen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #66a6ff;
            color: #fff;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            z-index: 1000;
            opacity: 1;
            transition: opacity 1s ease-in-out;
        }

        #splash-screen img {
            max-width: 150px;
            margin-bottom: 20px;
            box-shadow: 8px 8px 15px black;
        }

        #splash-screen h1 {
            font-size: 24px;
            text-shadow: 2px 2px 4px #000;
            text-align: center;
        }

        #splash-screen.hide {
            opacity: 0;
            visibility: hidden;
        }
        @media (max-width: 600px) {
            #splash-screen img {
                max-width: 120px;
            }

            #splash-screen h1 {
                font-size: 20px;
            }
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #007BFF;
            color: #fff;
            padding: 15px 30px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        header a {
            color: #fff;
            text-decoration: none;
            font-size: 16px;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header a:hover {
            color: #ffcc00;
        }

        .content {
            padding: 40px;
            max-width: 900px;
            margin: auto;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .content h1 {
            text-align: center;
            margin-bottom: 20px;
            font-size: 28px;
            color: #007BFF;
        }

        .feature {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            gap: 15px;
        }

        .feature img {
            width: 100px;
            height: 100px;
            object-fit: cover;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        .feature-description {
            flex: 1;
        }

        .interactive-buttons {
            display: flex;
            justify-content: space-around;
            margin-top: 30px;
        }

        .interactive-buttons a {
            text-decoration: none;
            padding: 10px 20px;
            background: #007BFF;
            color: white;
            border-radius: 5px;
            transition: background 0.3s ease, transform 0.2s ease;
        }

        .interactive-buttons a:hover {
            background: #0056b3;
            transform: scale(1.05);
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #007BFF;
            color: white;
            position: fixed;
            bottom: 0;
            width: 100%;
            font-size: 14px;
        }

        @media (max-width: 600px) {
            header {
                flex-direction: column;
                text-align: center;
            }

            .interactive-buttons {
                flex-direction: column;
            }

            .interactive-buttons a {
                margin-bottom: 10px;
            }
        }
    </style>
</head>
<body>
    <div id="splash-screen">
        <img src="https://camo.githubusercontent.com/db4c7f852ac5951515814bba18551cd7aeb48c4271df6f9ab1519bb8f49b4866/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f7468756d622f322f32312f4e65632e706e672e6a70672f32323070782d4e65632e706e672e6a7067" alt="College Logo">
        <h1>Welcome to NEC(IT) Portal</h1>
    </div>
    <header>
        <div>
            <a href="#">Home</a>
        </div>
        <div>
            <a href="initial.html">Get Student Info</a>
        </div>
        <div>
            <a href="code.html">Code</a>
        </div>
    </header><br><br>

    <div class="content">
        <h1>Welcome to the Student Management System</h1>
        <p>
            <strong>Project Requirement:</strong> Full-Stack Web Application with Java, Spring Boot, and MySQL.
        </p>
        <p>
            This project aims to create a system for managing and displaying student details efficiently. It includes
            dynamic data retrieval, search and filter functionality, and interactive features like calling and messaging
            directly from the interface.
        </p>
        <p>
            Key Features:
        </p>

        <div class="feature">
            <img src="https://cloudinary-marketing-res.cloudinary.com/images/w_1000,c_scale/v1695059532/Dynamic_website_In_text/Dynamic_website_In_text-png?_i=AA" alt="Dynamic Data Retrieval">
            <div class="feature-description">
                <strong>Dynamic Data Retrieval:</strong> The system connects to a MySQL database to fetch and display student
                information dynamically, ensuring real-time data consistency and scalability.
            </div>
        </div>

        <div class="feature">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSKKskPVTfaXZyaJYyJ7FfdmXd57Kf4Z0mOxQ&s" alt="Search & Filter">
            <div class="feature-description">
                <strong>Search & Filter by Branch, Section, and Year:</strong> Users can easily filter students using an intuitive
                interface to quickly locate specific information.
            </div>
        </div>

        <div class="feature">
            <img src="data:image/png;base64,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" alt="Interactive Icons">
            <div class="feature-description">
                <strong>Interactive Icons for Call and Message:</strong> Each student record includes clickable call and message
                icons to initiate quick communication through the device's default apps.
            </div>
        </div>

    </div><br><br>

    <footer>
        &copy; 2025 Student Management System. All rights reserved.
    </footer>
    <script>
    // Hide the splash screen after 2 seconds and show the form
window.addEventListener('load', () => {
    setTimeout(() => {
        const splashScreen = document.getElementById('splash-screen');
        if (splashScreen) {
            splashScreen.classList.add('hide');
        }
    }, 2000);
});

    </script>
</body>
</html>
