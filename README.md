<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Basics of Web Development</title>

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #6bf4f4;
            margin: 0;
            padding: 0;
        }

        .container {
            width: 80%;
            margin: auto;
            padding: 20px;
        }

        h1 {
            color: #f10404;
            text-align: center;
        }

        h2 {
            color: #e56504;
        }

        p {
            font-size: 16px;
            line-height: 1.6;
        }

        img {
            width: 250px;
            display: block;
            margin: 20px auto;
        }

        .app-buttons {
            margin-top: 20px;
            display: flex;
            justify-content: center;
            gap: 40px;
        }

        .app-icon {
            width: 110px;
            height: 110px;
            border-radius: 28px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            cursor: pointer;
            position: relative;
            box-shadow: 0 10px 20px rgba(0, 0, 0, .25);
            transition: 0.3s;
        }

        .app-icon::before {
            content: "";
            position: absolute;
            top: 10px;
            width: 70%;
            height: 28%;
            background: rgba(242, 241, 241, 0.35);
            border-radius: 18px;
        }

        .app-icon:hover {
            transform: translateY(-6px) scale(1.05);
            box-shadow: 0 16px 26px rgba(0, 0, 0, .35);
        }

        .app-icon i {
            font-size: 34px;
            margin-bottom: 6px;
        }

        .linkedin {
            background: #0A66C2;
        }

        .github {
            background: #24292F;
        }

        button {
            background-color: #0b6e4f;
            color: white;
            border: none;
            padding: 10px 18px;
            font-size: 15px;
            cursor: pointer;
            border-radius: 5px;
            margin: 5px;
        }

        button:hover {
            background-color: #065f46;
        }
    </style>
</head>

<body>

    <div class="container">

        <h1>Basics of Web Development</h1>

        <h2>Objective</h2>
        <p>Learn and apply foundational HTML, CSS and JavaScript concepts.</p>

        <h2>Steps</h2>

        <h3>1. Create a Simple Webpage Using HTML</h3>
        <p>This webpage includes headings, paragraphs, images, links and buttons.</p>

        <img src="https://cdn-icons-png.flaticon.com/512/919/919827.png" alt="HTML Logo">

        <h3>2. Style the Webpage Using CSS</h3>
        <p>CSS is used to add colors, fonts, spacing and layout.</p>

        <h3>3. Add Basic JavaScript for Interactivity</h3>
        <button onclick="showMessage()">Click Me</button>

        <div class="app-buttons">

            <div class="app-icon linkedin" onclick="openLinkedIn()">
                <i class="fa-brands fa-linkedin"></i>
                LinkedIn
            </div>

            <div class="app-icon github" onclick="openGitHub()">
                <i class="fa-brands fa-github"></i>
                GitHub
            </div>

        </div>

    </div>

    <script>
        function showMessage() {
            alert("JavaScript alert is working!");
        }

        function openLinkedIn() {
            window.open("https://www.linkedin.com", "_blank");
        }

        function openGitHub() {
            window.open("https://github.com", "_blank");
        }
    </script>

</body>

</html>
