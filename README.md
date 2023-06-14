<html>
<head>
    <title>Protected Content</title>
    <script>
        function checkPIN() {
            var pinInput = document.getElementById("pin").value;
            var content = document.getElementById("content");

            if (pinInput === "1234") {
                content.textContent = "CARIOCA";
            } else {
                content.textContent = "Incorrect PIN. Access denied.";
            }
        }
    </script>
</head>
<body>
    <h1>Protected Content</h1>
    <label for="pin">Enter PIN:</label>
    <input type="password" id="pin">
    <button onclick="checkPIN()">Submit</button>

    <div id="content"></div>
</body>
</html>
