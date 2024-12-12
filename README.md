<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Portfolio</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #111;
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 100vh;
        }

        .container {
            max-width: 900px;
            width: 100%;
            text-align: center;
            flex: 1;
        }

        .profile {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
        }

        .profile img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 2px solid #fff;
        }

        h1 {
            margin: 0;
            font-size: 2em;
        }

        .about {
            margin-top: 20px;
            font-size: 1.1em;
            line-height: 1.6;
            padding: 0 20px; /* Same padding as buttons */
        }

        .about span {
            background: #444;
            padding: 3px 6px;
            border-radius: 5px;
            color: #fff;
            display: inline-block;
        }

        .about span:nth-child(1) {
            background-color: #5A8DEE;
        }

        .about span:nth-child(2) {
            background-color: #39DA8A;
        }

        .about span:nth-child(3) {
            background-color: #FDAC41;
        }

        .socials {
            margin-top: 30px;
            padding: 0 20px; /* Same padding as buttons */
        }

        .socials a {
            color: #fff;
            text-decoration: none;
            background: #333;
            padding: 10px 20px;
            margin-right: 10px;
            border-radius: 5px;
            display: inline-block;
        }

        .socials a:hover {
            background: #555;
        }

        .toolbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            padding: 10px 20px;
            background: #222;
            position: fixed;
            bottom: 0;
            left: 0;
        }

        .toolbar a {
            color: #fff;
            text-decoration: none;
            padding: 5px 10px;
            border-radius: 5px;
        }

        .toolbar a:hover {
            background: #555;
        }

        .toolbar .mode-toggle {
            background: #333;
            color: #fff;
            border: none;
            padding: 5px 10px;
            border-radius: 5px;
            cursor: pointer;
        }

        .toolbar .mode-toggle:hover {
            background: #555;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Profile Section -->
        <div class="profile">
            <img src="https://i.imgur.com/RjyRyGs.png" alt="Profile Picture">
            <h1>Adam Busby</h1>
        </div>

        <!-- About Section -->
        <div class="about">
            <p>I enjoy learning about <span>cybersecurity</span> and <span>creating software</span>. I also like staying fit and strong by going to the <span>gym</span>.</p>
        </div>

        <!-- Socials Section -->
        <div class="socials">
            <a href="https://www.instagram.com/adam_busby_">Instagram</a>
            <a href="https://www.github.com/M1NM1">GitHub</a>
            <a href="https://www.stackoverflow.com/users/15796123/atheriums">Stack Overflow</a>
        </div>
    </div>

    <!-- Bottom Toolbar -->
    <div class="toolbar">
        <div></div> <!-- Placeholder to center content -->
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
        <button class="mode-toggle" onclick="toggleMode()">Switch to Light Mode</button>
    </div>

    <script>
        function toggleMode() {
            const body = document.body;
            const button = document.querySelector('.mode-toggle');

            if (body.style.backgroundColor === 'white') {
                body.style.backgroundColor = '#111';
                body.style.color = '#fff';
                button.textContent = 'Switch to Light Mode';
            } else {
                body.style.backgroundColor = 'white';
                body.style.color = '#000';
                button.textContent = 'Switch to Dark Mode';
            }
        }
    </script>
</body>
</html>
