Original file line number	Diff line number	Diff line change
@@ -0,0 +1,241 @@
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ستار نت - أسعار الاشتراك</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }
        /* خلفية متحركة باستخدام تدرجات */
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, #74b9ff, #a29bfe, #81ecec, #fab1a0);
            background-size: 400% 400%;
            animation: gradientAnimation 15s ease infinite;
            z-index: -1;
        }
        /* حركة تدرج اللون للخلفية */
        @keyframes gradientAnimation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        header {
            background-color: rgba(44, 62, 80, 0.85);
            padding: 20px;
            color: #ecf0f1;
        }
        h1 {
            margin: 0;
            display: inline-block;
            font-size: 26px;
            color: #f39c12;
        }
        .star {
            color: #f39c12;
            font-size: 24px;
            vertical-align: middle;
            margin-left: 5px;
        }
        /* شريط متحرك بتنسيق أكبر */
        .marquee, .marquee2 {
            background-color: #e67e22;
            color: #fff;
            padding: 15px;
            font-size: 24px; /* تكبير الخط */
            overflow: hidden;
            white-space: nowrap;
            box-sizing: border-box;
        }
        .marquee-text, .marquee-text2 {
            display: inline-block;
            padding-left: 100%;
            animation: marquee 10s linear infinite;
        }
        /* الشريط الثاني */
        .marquee2 {
            background-color: #3498db;
            margin-top: 5px;
        }
        .marquee-text2 {
            animation-duration: 12s;
        }
        /* حركة الشريط المتحرك */
        @keyframes marquee {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
        }
        .container {
            padding: 20px;
        }
        /* تصميم الباقات */
        .plan {
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 15px;
            margin: 15px auto;
            max-width: 280px;
            background-color: rgba(255, 255, 255, 0.8);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .plan h2 {
            color: #2c3e50;
            font-size: 20px;
        }
        .price {
            font-size: 22px;
            color: #e74c3c;
            margin: 10px 0;
        }
        .button {
            background-color: #3498db;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            display: inline-block;
            font-size: 14px;
            transition: background-color 0.3s;
        }
        .button:hover {
            background-color: #2980b9;
        }
        footer {
            background-color: rgba(44, 62, 80, 0.85);
            color: #ecf0f1;
            padding: 10px 5px;
            font-size: 12px;
        }
        /* نقاط البيع */
        .sales-points-container {
            margin: 15px 0;
        }
        .sales-points-header {
            font-size: 15px;
            color: #2980b9;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .sales-points-header .cart-icon {
            font-size: 18px;
            margin-right: 5px;
        }
        .sales-point-box {
            display: inline-block;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 8px;
            margin: 5px;
            background-color: #f5f5f5;
            color: #333;
            width: 120px;
            font-size: 14px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        /* تصميم المهندس بن طاهر */
        .designer-section {
            background-color: #9b59b6; /* خلفية بنفسجية */
            border-radius: 10px; /* زوايا دائرية */
            padding: 20px; /* padding داخلي */
            margin: 20px auto; /* هوامش تلقائية لتمركز العنصر */
            max-width: 300px; /* عرض أقصى */
            text-align: center; /* مركزية النص */
        }
        .designer-text {
            font-size: 14px; /* حجم الخط صغير */
            color: #ffffff; /* لون النص أبيض */
            margin: 0; /* إزالة الهوامش */
            font-style: italic; /* جعل الخط مائل */
        }
    </style>
</head>
<body>
    <!-- الشريط المتحرك العلوي -->
    <div class="marquee">
        <span class="marquee-text">نحن لا نتحمل أي خلل خارج عن إرادتنا</span>
    </div>
    <!-- الشريط المتحرك الثاني -->
    <div class="marquee2">
        <span class="marquee-text2">للتزويد بخدمة الإنترنت إلى منزلك تواصل معنا عبر الواتساب: 780483098</span>
    </div>
    <header>
        <h1>شبكة ستار نت</h1>
        <span class="star">★</span>
        <p>أسعار الاشتراك في باقات الإنترنت</p>
    </header>
    <div class="container">
        <div class="plan">
            <h2>باقة 700 ميجا</h2>
            <p class="price">200 ريال / شهر</p>
            <a href="https://wa.me/780483098" class="button">تواصل عبر واتساب</a>
        </div>
        <div class="plan">
            <h2>باقة 2.5 جيجا</h2>
            <p class="price">500 ريال / شهر</p>
            <a href="https://wa.me/780483098" class="button">تواصل عبر واتساب</a>
        </div>
        <div class="plan">
            <h2>باقة 4 جيجا</h2>
            <p class="price">1000 ريال / شهر</p>
            <a href="https://wa.me/780483098" class="button">تواصل عبر واتساب</a>
        </div>
        <div class="plan">
            <h2>باقة 20 جيجا</h2>
            <p class="price">5000 ريال / شهر</p>
            <a href="https://wa.me/780483098" class="button">تواصل عبر واتساب</a>
        </div>
    </div>
    <!-- قسم تصميم المهندس بن طاهر -->
    <div class="designer-section">
        <h2 class="designer-text">تصميم المهندس بن طاهر</h2>
    </div>
    <footer>
        <div class="sales-points-container">
            <div class="sales-points-header">
                <span class="cart-icon">🛒</span>
                <span>نقاط البيع</span>
            </div>
            <div class="sales-point-box">سوبر ماركت البسمة</div>
            <div class="sales-point-box">بقالة الخير</div>
            <div class="sales-point-box">عبر الواتساب</div>
        </div>
        <p>&copy; 2024 شبكة ستار نت | جميع الحقوق محفوظة</p>
        <p>يتوفر لدينا خدمة تسديد عبر بنك الكريمي</p>
    </footer>
</body>
</html>
