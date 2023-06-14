<html>
<head>
    <title>Protected Content</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: white;
        }
        
        .preloader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            background-color: white;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .preloader img {
            width: 200px;
        }
        
        .content {
            display: none;
        }
    </style>
    <script>
        function showPreloader() {
            var pinInput = document.getElementById("pin").value;

            if (pinInput === "1234") {
                var preloader = document.getElementById("preloader");
                var content = document.getElementById("content");
                
                preloader.style.display = "flex";
                content.style.display = "none";
                
                setTimeout(function() {
                    preloader.style.display = "none";
                    content.style.display = "block";
                }, 3000); // Show content after 3 seconds (3000 milliseconds)
            } else {
                alert("Incorrect PIN. Access denied.");
            }
        }
    </script>
</head>
<body>
    <!-- Preloader -->
    <div id="preloader" class="preloader">
        <!-- Insert your preloader GIF here -->
         <img src="d1dec4302ac31fd085ca7b45c56df7cb_w200.gif" alt="Preloader"> 
    </div>
    
    <!-- Content -->
    <div id="content" class="content">
        <!-- Blank white page -->
    </div>
    
    <!-- PIN input -->
    <div id="pin-page">
        <h1>Enter PIN</h1>
        <label for="pin">PIN:</label>
        <input type="password" id="pin">
        <button onclick="showPreloader()">Submit</button>
    </div>
</body>
</html>
