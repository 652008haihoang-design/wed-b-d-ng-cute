<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gửi Dương ❤️</title>
    <style>
        body {
            background-color: #ffb6c1; /* Nền màu hồng nhạt */
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        .card {
            background-color: rgba(255, 255, 255, 0.85);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            text-align: center;
            max-width: 500px;
            width: 80%;
        }

        h1 {
            color: #d81b60;
            margin-bottom: 20px;
        }

        #text-container {
            font-size: 1.2rem;
            color: #4a4a4a;
            line-height: 1.6;
            min-height: 100px;
            white-space: pre-line; /* Giữ nguyên các dòng xuống hàng */
        }

        /* Hiệu ứng con trỏ nhấp nháy khi chữ đang chạy */
        .cursor {
            display: inline-block;
            width: 2px;
            background-color: #d81b60;
            animation: blink 0.7s infinite;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }
    </style>
</head>
<body>

    <div class="card">
        <h1>Gửi cô gái tên Dương 💕</h1>
        <div id="text-container"><span id="typed-text"></span><span class="cursor">&nbsp;</span></div>
    </div>

    <script>
        // Nội dung lời nhắn muốn gửi đến Dương
        const text = "Chào Dương nè! ✨\nChúc Dương một ngày thật xinh đẹp, luôn vui vẻ và ngập tràn hạnh phúc nhé! 💕";
        
        let index = 0;
        const speed = 80; // Tốc độ chạy chữ (mili-giây mỗi ký tự)

        function typeWriter() {
            if (index < text.length) {
                document.getElementById("typed-text").textContent += text.charAt(index);
                index++;
                setTimeout(typeWriter, speed);
            }
        }

        // Bắt đầu chạy hiệu ứng chữ khi trang web tải xong
        window.onload = typeWriter;
    </script>

</body>
</html>
