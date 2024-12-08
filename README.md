<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Troll Người Yêu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background-color: #f4f4f4;
        }
        h1 {
            color: #ff6347;
        }
        .button {
            padding: 15px 30px;
            font-size: 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            background-color: #45a049;
        }
        /* Style cho trái tim */
        .heart {
            font-size: 100px;
            color: red;
            display: none;
            animation: beat 1s infinite;
        }

        /* Animation trái tim đập */
        @keyframes beat {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
            100% {
                transform: scale(1);
            }
        }
    </style>
</head>
<body>
    <h1>Chào người yêu! Bấm vào nút dưới đây...</h1>
    <button class="button" onclick="revealHeart()">Bấm vào đây</button>
    
    <!-- Trái tim -->
    <div id="heart" class="heart">
        ❤️
    </div>

    <script>
        function revealHeart() {
            var heart = document.getElementById("heart");
            heart.style.display = "block"; // Hiển thị trái tim
        }
    </script>
</body>
</html>

