<!DOCTYPE html>
<html>
<head>
    <title>Protected Content</title>
    <style>
        .preloader {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 9999;
        }
    </style>
    <script>
        function showPreloader() {
            var preloader = document.getElementById("preloader");
            var pinInput = document.getElementById("pin").value;

            if (pinInput === "1234") {
                preloader.style.display = "block";
                setTimeout(showContent, 2000); // Simulating a delay of 2 seconds before showing the content
            } else {
                alert("Incorrect PIN. Access denied.");
            }
        }

        function showContent() {
            var preloader = document.getElementById("preloader");
            preloader.style.display = "none";

            var contentPage = document.getElementById("content-page");
            contentPage.style.display = "block";
        }
    </script>
</head>
<body>
    <div id="preloader" class="preloader">
        <img src="path_to_your_preloader.gif" alt="Loading...">
    </div>

    <div id="content-page" style="display: none;">
        <h1>Protected Content</h1>
        <p>CARIOCA</p>
    </div>

    <div id="pin-page">
        <h1>Enter PIN</h1>
        <label for="pin">PIN:</label>
        <input type="password" id="pin">
        <button onclick="showPreloader()">Submit</button>
    </div>
</body>
</html>
