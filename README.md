
<html>
<head>
    <title>My Favorite Hobby - Basketball</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
        }

        h1 {
            color: #d35400;
        }

        img {
            border-radius: 10px;
            margin: 10px;
        }

        a {
            color: #2980b9;
            text-decoration: none;
            font-weight: bold;
        }

        a:hover {
            color: #e74c3c;
        }

        form {
            background: white;
            padding: 15px;
            width: 300px;
            margin: auto;
            border-radius: 10px;
            box-shadow: 0px 0px 10px gray;
        }

        input, textarea {
            width: 90%;
            padding: 8px;
            margin: 5px 0;
        }

        input[type="submit"] {
            background-color: #d35400;
            color: white;
            border: none;
            cursor: pointer;
        }

        input[type="submit"]:hover {
            background-color: #e67e22;
        }

        button {
            margin-top: 10px;
            padding: 10px;
            background-color: #27ae60;
            color: white;
            border: none;
            cursor: pointer;
        }

        button:hover {
            background-color: #2ecc71;
        }
    </style>

</head>
<body>

    <h1>My Favorite Hobby: Basketball 🏀</h1>

    <!-- Image -->
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7a/Basketball.png" width="400" alt="Basketball">

    <p id="description">
        Basketball is my favorite hobby because it is fun, exciting, and keeps me active.
        I enjoy playing with friends and improving my skills like shooting and dribbling.
    </p>

    <!-- Button with JS -->
    <button onclick="changeText()">Click to Change Description</button>

    <!-- Combined External Links Section -->
    <p>
        Learn more about basketball:
        <a href="https://en.wikipedia.org/wiki/Basketball" target="_blank">
            Basketball Article
        </a>
    </p>

    <p>
        Explore my personal page:
        <a href="https://sagonoydenmar7-debug.github.io/learn-more/" target="_blank">
            Learn More Page
        </a>
    </p>

    <!-- Internal Link -->
    <p>
        <a href="gallery.html">View My Gallery</a>
    </p>

    <h2>Canvas Drawing</h2>
    <canvas id="myCanvas" width="300" height="200" style="border:1px solid black;"></canvas>

    <script>
        // Canvas drawing
        var canvas = document.getElementById("myCanvas");
        var ctx = canvas.getContext("2d");

        ctx.beginPath();
        ctx.arc(150, 100, 50, 0, 2 * Math.PI);
        ctx.stroke();

        ctx.beginPath();
        ctx.moveTo(100, 100);
        ctx.lineTo(200, 100);
        ctx.stroke();

        ctx.beginPath();
        ctx.moveTo(150, 50);
        ctx.lineTo(150, 150);
        ctx.stroke();

        // JavaScript function
        function changeText() {
            document.getElementById("description").innerHTML =
            "Basketball helps me stay healthy, build teamwork, and have fun while competing!";
        }
    </script>

    <h2>Leave a Comment</h2>

    <form onsubmit="showMessage(); return false;">
        <input type="text" name="name" placeholder="Your Name" required><br>
        <input type="email" name="email" placeholder="Your Email" required><br>
        <textarea name="comment" rows="4" placeholder="Your Comment"></textarea><br>
        <input type="submit" value="Submit">
    </form>

    <p id="message"></p>

    <script>
        function showMessage() {
            document.getElementById("message").innerHTML =
            "✅ Thank you for your comment!";
            document.querySelector("form").reset();
        }
    </script>

</body>
</html>
