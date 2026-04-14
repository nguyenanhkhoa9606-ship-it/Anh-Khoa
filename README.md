# Anh-Khoa
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description" content="Website cá nhân của Nguyễn Anh Khoa - Kỹ sư Chăn nuôi & Thạc sĩ Thú y. Khám phá hành trình, kinh nghiệm và kỹ năng chuyên môn.">
    <meta name="keywords" content="Nguyễn Anh Khoa, Kỹ sư chăn nuôi, Thú y, Đại học Cần Thơ, Portfolio">
    <meta name="author" content="Nguyễn Anh Khoa">
    <title>Nguyễn Anh Khoa | Kỹ sư Chăn nuôi & Thú y</title>

    <!-- Font chữ Quicksand -->
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Icon FontAwesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --bg-color: #FFF9F9;
            --text-main: #4A4A4A;
            --text-light: #7A7A7A;
            --pastel-blue: #AEE1E1;
            --pastel-pink: #F4C2C2;
            --pastel-orange: #FCD2AE;
            --pastel-green: #D3EBCD;
            --pastel-yellow: #FCF4DD;
            --white: #FFFFFF;
            --shadow: 0 10px 30px rgba(0,0,0,0.05);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Quicksand', sans-serif; }
        body { background-color: var(--bg-color); color: var(--text-main); line-height: 1.6; overflow-x: hidden; }
        a { text-decoration: none; color: inherit; }
        ul { list-style: none; }
        .container { max-width: 1100px; margin: 0 auto; padding: 0 20px; }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        .fade-in { opacity: 0; transform: translateY(30px); transition: opacity 0.8s ease, transform 0.8s ease; }
        .fade-in.appear { opacity: 1; transform: translateY(0); }

        section { padding: 80px 0; }
        .section-title { text-align: center; font-size: 2.2rem; margin-bottom: 40px; color: #333; position: relative; }
        .section-title::after {
            content: ''; display: block; width: 60px; height: 4px; background: var(--pastel-pink);
            margin: 10px auto 0; border-radius: 2px;
        }

        .hero { display: flex; align-items: center; justify-content: space-between; min-height: 100vh; gap: 40px; }
        .hero-content { flex: 1; }
        .greeting { font-size: 1.2rem; color: var(--pastel-orange); font-weight: 700; margin-bottom: 10px; }
        .hero-title { font-size: 3.5rem; line-height: 1.2; margin-bottom: 20px; color: #333; }
        .hero-title span { color: #f28b82; }
        .hero-desc { font-size: 1.1rem; color: var(--text-light); margin-bottom: 30px; }

        .personal-info { display: flex; flex-wrap: wrap; gap: 15px; margin-bottom: 30px; }
        .info-tag { background: var(--white); padding: 8px 15px; border-radius: 20px; box-shadow: var(--shadow); font-weight: 600; font-size: 0.95rem; display: flex; align-items: center; gap: 8px; }
        .info-tag i { color: #f28b82; }

        .social-links { display: flex; gap: 15px; }
        .social-btn {
            width: 45px; height: 45px; border-radius: 50%; background: var(--white); display: flex;
            align-items: center; justify-content: center; font-size: 1.2rem; box-shadow: var(--shadow);
            transition: all 0.3s ease; color: var(--text-main);
        }
        .social-btn:hover { background: var(--pastel-pink); color: var(--white); transform: translateY(-5px); }

        .hero-image { flex: 1; display: flex; justify-content: center; position: relative; }
        .blob-bg {
            position: absolute; width: 400px; height: 400px; background: var(--pastel-blue);
            border-radius: 40% 60% 70% 30% / 40% 50% 60% 50%; animation: float 6s ease-in-out infinite; z-index: -1;
        }
        .profile-img {
            width: 320px; height: 320px; object-fit: cover; border-radius: 50%; border: 8px solid var(--white); box-shadow: var(--shadow);
        }

        @media (max-width: 768px) {
            .hero { flex-direction: column; text-align: center; padding-top: 100px; justify-content: center; }
            .hero-title { font-size: 2.5rem; }
            .personal-info, .social-links { justify-content: center; }
            .blob-bg { width: 300px; height: 300px; }
            .profile-img { width: 250px; height: 250px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <section class="hero fade-in">
            <div class="hero-content">
                <div class="greeting">👋 Xin chào, mình là</div>
                <h1 class="hero-title">Nguyễn Anh <span>Khoa</span></h1>
                <p class="hero-desc">
                    Một Kỹ sư Chăn nuôi đam mê nghiên cứu và phát triển bền vững. Mình luôn hướng tới việc áp dụng khoa học kỹ thuật để nâng cao sức khỏe vật nuôi.
                </p>

                <div class="personal-info">
                    <div class="info-tag"><i class="fa-solid fa-cake-candles"></i> 02/10/2000</div>
                    <div class="info-tag"><i class="fa-solid fa-location-dot"></i> An Phú, An Giang</div>
                    <div class="info-tag"><i class="fa-solid fa-user-graduate"></i> Kỹ sư Chăn nuôi</div>
                </div>

                <div class="social-links">
                    <a href="mailto:nguyenanhkhoa9606@gmail.com" class="social-btn"><i class="fa-solid fa-envelope"></i></a>
                    <a href="tel:+84869089606" class="social-btn"><i class="fa-solid fa-phone"></i></a>
                    <a href="#" class="social-btn"><i class="fa-brands fa-github"></i></a>
                    <a href="#" class="social-btn"><i class="fa-brands fa-facebook-f"></i></a>
                </div>
            </div>

            <div class="hero-image">
                <div class="blob-bg"></div>
                <img src="/mnt/data/z4595929194390_3180868dd5b1cebf7ef751c606706813.jpg" alt="Nguyễn Anh Khoa" class="profile-img">
            </div>
        </section>
    </div>

</body>
</html>
