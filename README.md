# jwhr<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الجوهرة إكسبريس - توصيل سريع في دول الخليج</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        .navbar {
            background: #2c3e50;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .company-logo {
            max-width: 120px;
            height: auto;
        }

        .hero {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)),
                        url('https://images.unsplash.com/photo-1607083206869-4c7672e72a8a?ixlib=rb-1.2.1') center/cover;
            height: 70vh;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
        }

        .order-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            padding: 3rem;
            background: white;
        }

        .step-card {
            text-align: center;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .order-form {
            max-width: 800px;
            margin: 3rem auto;
            padding: 2rem;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        input, select, textarea {
            width: 100%;
            padding: 0.8rem;
            margin: 0.5rem 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        button {
            background: #e74c3c;
            color: white;
            border: none;
            padding: 1rem 2rem;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
            font-size: 1.1rem;
        }

        .contact-info {
            background: #34495e;
            padding: 1.5rem;
            text-align: center;
            color: white;
        }

        .contact-info a {
            color: #e74c3c;
            text-decoration: none;
            margin: 0 10px;
        }

        footer {
            background: #2c3e50;
            color: white;
            padding: 2rem;
            text-align: center;
        }
    </style>
</head>
<body>
    <!-- شريط التنقل مع الشعار -->
    <nav class="navbar">
        <div class="logo-container">
            <img src=""C:\Users\rajab\OneDrive\Desktop\jwharr\5827798879100323583_120.jpg"="Aljawhara Express Logo" class="company-logo">
        </div>
        <div>
            <a href="#order" style="color: white; text-decoration: none;">اطلب الآن</a>
        </div>
    </nav>

    <!-- قسم البط الرئيسي -->
    <section class="hero">
        <div>
            <h1 style="font-size: 2.8rem; margin-bottom: 1.5rem;">الجوهرة إكسبريس</h1>
            <p style="font-size: 1.2rem;">نصل إليك أينما كنت في الخليج 🚀</p>
        </div>
    </section>

    <!-- خطوات الطلب -->
    <section class="order-steps">
        <div class="step-card">
            <i class="fas fa-box-open fa-3x" style="color: #e74c3c;"></i>
            <h3>1. قدم طلبك</h3>
            <p>املأ النموذج ببيانات الشحن</p>
        </div>
        <div class="step-card">
            <i class="fas fa-truck fa-3x" style="color: #3498db;"></i>
            <h3>2. معالجة الطلب</h3>
            <p>فريقنا يجهز الشحنة</p>
        </div>
        <div class="step-card">
            <i class="fas fa-check-circle fa-3x" style="color: #2ecc71;"></i><h3>3. التوصيل</h3>
            <p>استلمها في باب منزلك</p>
        </div>
    </section>

    <!-- نموذج الطلب -->
    <section class="order-form" id="order">
        <h2 style="text-align: center; margin-bottom: 2rem;">نموذج طلب التوصيل 📝</h2>
        <form id="deliveryForm">
            <input type="text" placeholder="الاسم الكامل" required>
            <input type="tel" placeholder="رقم الواتساب (مثال: 963954653033)" pattern="[0-9]{8,15}" required>
            <input type="text" placeholder="عنوان الشحن" required>
            <select required>
                <option value="">اختر نوع الخدمة</option>
                <option>توصيل سريع (24 ساعة)</option>
                <option>توصيل عادي (48 ساعة)</option>
            </select>
            <textarea placeholder="ملاحظات إضافية" rows="4"></textarea>
            <button type="submit">تأكيد الطلب 🚀</button>
        </form>
    </section>

    <!-- قسم الاتصال -->
    <div class="contact-info">
        <h3>تواصل معنا:</h3>
        <p>
            <a href="https://wa.me/96555665192" target="_blank">
                <i class="fab fa-whatsapp"></i> واتساب: 963954653033
            </a>
            |
            <a href="mailto:en.thamerali@gmail.com">
                <i class="fas fa-envelope"></i> en.thamerali@gmail.com
            </a>
        </p>
    </div>

    <!-- تذييل الصفحة -->
    <footer>
        <p>جميع الحقوق محفوظة © 2024 الجوهرة إكسبريس</p>
    </footer>

    <script>
        // تفاعلية النموذج
        document.getElementById('deliveryForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const whatsappNumber = '963954653033';
            const message = `طلب جديد:%0A
                الاسم: ${this[0].value}%0A
                رقم الجوال: ${this[1].value}%0A
                العنوان: ${this[2].value}%0A
                الخدمة: ${this[3].value}`;

            window.open(`https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`, '_blank');
            
            alert('تم استلام طلبك بنجاح! سيتم التواصل معك خلال 10 دقائق.');
            this.reset();
        });
    </script>
</body>
</html>
