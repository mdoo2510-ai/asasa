```html
<!DOCTYPE html>
<html dir="rtl" lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>دليل التميز والاعتماد المدرسي | [اسمك]</title>
    <!-- استخدام خط عربي أنيق من Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Cairo', sans-serif;
            background: linear-gradient(145deg, #f0f4f8 0%, #e6ecf3 100%);
            min-height: 100vh;
            padding: 2rem 1rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .container {
            max-width: 700px;
            width: 100%;
            margin: 0 auto;
        }

        /* بطاقة الرأس */
        .header-card {
            background: #ffffff;
            border-radius: 2.5rem;
            padding: 2rem 1.5rem;
            text-align: center;
            box-shadow: 0 25px 45px rgba(0, 20, 40, 0.12);
            margin-bottom: 2rem;
            border: 1px solid rgba(255, 255, 255, 0.6);
            backdrop-filter: blur(2px);
        }

        .school-badge {
            display: inline-block;
            background: #1e4a6b;
            color: white;
            padding: 0.4rem 1.8rem;
            border-radius: 3rem;
            font-size: 0.9rem;
            font-weight: 600;
            letter-spacing: 0.3px;
            margin-bottom: 1.2rem;
            background: linear-gradient(135deg, #1e4a6b 0%, #0d2f44 100%);
            box-shadow: 0 8px 14px rgba(20, 60, 90, 0.25);
        }

        .main-title {
            font-size: 2.2rem;
            font-weight: 800;
            color: #0b2b3d;
            line-height: 1.4;
            margin-bottom: 0.5rem;
        }

        .subtitle {
            font-size: 1.1rem;
            color: #3c5a6e;
            font-weight: 500;
            margin-bottom: 1.5rem;
            border-bottom: 2px dashed #bdd3e0;
            display: inline-block;
            padding-bottom: 0.7rem;
        }

        .contributor {
            background: #f4f9ff;
            border-radius: 2rem;
            padding: 0.8rem 1.5rem;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            font-weight: 600;
            color: #1e4a6b;
            border: 1px solid #cbdde9;
        }

        .contributor span {
            color: #0b2b3d;
            font-weight: 700;
        }

        /* شريط الإحصائيات */
        .stats-grid {
            display: flex;
            justify-content: space-around;
            gap: 1rem;
            margin: 1.8rem 0 0.5rem;
            flex-wrap: wrap;
        }

        .stat-item {
            background: white;
            border-radius: 2rem;
            padding: 0.8rem 1.2rem;
            display: flex;
            align-items: center;
            gap: 0.6rem;
            box-shadow: 0 12px 22px rgba(0,0,0,0.06);
            font-weight: 700;
            background: #ffffff;
            border: 1px solid #e2ebf3;
            min-width: 100px;
            justify-content: center;
        }

        .stat-emoji {
            font-size: 1.6rem;
        }

        .stat-number {
            font-size: 1.7rem;
            font-weight: 800;
            color: #113448;
        }

        .stat-label {
            font-size: 0.85rem;
            color: #4a6272;
            font-weight: 600;
        }

        /* بطاقة المجالات */
        .domains-title {
            font-size: 1.3rem;
            font-weight: 700;
            color: #153e54;
            margin: 1.8rem 0 1rem;
            text-align: center;
        }

        .domains-grid {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .domain-card {
            background: white;
            border-radius: 1.8rem;
            padding: 1.3rem 1.8rem;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 15px 28px rgba(0,0,0,0.07);
            border: 1px solid #e3edf6;
            transition: all 0.25s ease;
            cursor: pointer;
            background: linear-gradient(to left, #ffffff, #fafdff);
        }

        .domain-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 20px 32px rgba(18, 67, 97, 0.15);
            border-color: #aac7df;
        }

        .domain-info {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .domain-icon {
            font-size: 2.2rem;
            background: #e8f0f7;
            width: 55px;
            height: 55px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 1.3rem;
            color: #1a4057;
        }

        .domain-text h3 {
            font-size: 1.25rem;
            font-weight: 700;
            color: #0c2a3b;
            margin-bottom: 0.2rem;
        }

        .domain-text p {
            font-size: 0.85rem;
            color: #5b6f7e;
            font-weight: 500;
        }

        .arrow {
            font-size: 1.8rem;
            color: #6f8da0;
            font-weight: 400;
        }

        .footer-note {
            text-align: center;
            margin-top: 2.2rem;
            color: #486677;
            font-weight: 600;
            font-size: 0.9rem;
            background: rgba(255,255,255,0.7);
            padding: 0.7rem 1.5rem;
            border-radius: 2rem;
            backdrop-filter: blur(4px);
        }

        .footer-note strong {
            color: #0b2b3d;
        }

        @media (max-width: 480px) {
            .main-title {
                font-size: 1.8rem;
            }
            .domain-card {
                padding: 1rem 1.2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- البطاقة الرئيسية -->
        <div class="header-card">
            <div class="school-badge">
                🏫 مدارس [اسم مدرستك] الأهلية
            </div>
            <h1 class="main-title">خارطة الطريق للتميز<br>والاعتماد المدرسي</h1>
            <div class="subtitle">
                مساهمة من [اسمك] لنقل أثر التميز
            </div>
            
            <!-- مساهم -->
            <div class="contributor">
                ✨ تصميم وإعداد: <span>[اسمك الكامل]</span>
            </div>

            <!-- الإحصائيات السريعة (مطابقة للموقع الأصلي) -->
            <div class="stats-grid">
                <div class="stat-item">
                    <span class="stat-emoji">🗂️</span>
                    <span class="stat-number">4</span>
                    <span class="stat-label">مجالات</span>
                </div>
                <div class="stat-item">
                    <span class="stat-emoji">📋</span>
                    <span class="stat-number">11</span>
                    <span class="stat-label">معياراً</span>
                </div>
                <div class="stat-item">
                    <span class="stat-emoji">🎯</span>
                    <span class="stat-number">54</span>
                    <span class="stat-label">مؤشراً</span>
                </div>
            </div>
        </div>

        <!-- عنوان المجالات -->
        <div style="margin: 0.5rem 0 0.8rem; text-align: center;">
            <h2 style="font-size: 1.4rem; font-weight: 700; color: #123247;">المجالات الأربعة</h2>
            <p style="color: #3b5567; font-size: 0.9rem;">اختر المجال للاطلاع على معاييره ومؤشراته وخرائط الطريق</p>
        </div>

        <!-- قائمة المجالات (مطابقة للمحتوى الأصلي - تفاعلية) -->
        <div class="domains-grid">
            <!-- المجال الأول -->
            <div class="domain-card" onclick="showDomainMessage('القيادة المدرسية')">
                <div class="domain-info">
                    <div class="domain-icon">🏛️</div>
                    <div class="domain-text">
                        <h3>القيادة المدرسية</h3>
                        <p>المعايير والمؤشرات الخاصة بالقيادة</p>
                    </div>
                </div>
                <div class="arrow">←</div>
            </div>
            <!-- المجال الثاني -->
            <div class="domain-card" onclick="showDomainMessage('التعليم والتعلم')">
                <div class="domain-info">
                    <div class="domain-icon">📚</div>
                    <div class="domain-text">
                        <h3>التعليم والتعلم</h3>
                        <p>استراتيجيات التدريس وجودة المخرجات</p>
                    </div>
                </div>
                <div class="arrow">←</div>
            </div>
            <!-- المجال الثالث -->
            <div class="domain-card" onclick="showDomainMessage('بيئة المدرسة')">
                <div class="domain-info">
                    <div class="domain-icon">🌱</div>
                    <div class="domain-text">
                        <h3>بيئة المدرسة</h3>
                        <p>السلامة والمرافق والمناخ المدرسي</p>
                    </div>
                </div>
                <div class="arrow">←</div>
            </div>
            <!-- المجال الرابع -->
            <div class="domain-card" onclick="showDomainMessage('الشراكة المجتمعية')">
                <div class="domain-info">
                    <div class="domain-icon">🤝</div>
                    <div class="domain-text">
                        <h3>الشراكة المجتمعية</h3>
                        <p>العلاقة مع أولياء الأمور والمجتمع</p>
                    </div>
                </div>
                <div class="arrow">←</div>
            </div>
        </div>

        <!-- تذييل يحمل اسمك والمدرسة -->
        <div class="footer-note">
            © 2025 <strong>[اسمك]</strong> - <strong>مدارس [اسم مدرستك] الأهلية</strong> 🌟 جميع الحقوق محفوظة
        </div>
    </div>

    <!-- نافذة منبثقة بسيطة لعرض رسالة عند الضغط على مجال (تمثيل للتفاعل) -->
    <script>
        function showDomainMessage(domainName) {
            // في الموقع الأصلي تنتقل إلى صفحة تفاصيل المجال؛ هنا نعرض تنبيهًا توضيحيًا باسمك
            alert(`📌 أنت الآن في مجال: "${domainName}"\n\n(في النسخة الكاملة يمكن عرض المعايير والمؤشرات الخاصة بـ [اسمك] ومدرسة [اسم مدرستك])`);
        }
    </script>
</body>
</html>
```
