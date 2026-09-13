<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مركز الملصقات - صانع ملصقات مميز</title>
    <style>
        body {
            background-color: #0b0f19;
            color: #ffffff;
            font-family: Tahoma, sans-serif;
            margin: 0;
            padding: 0;
            padding-bottom: 70px;
        }
        .app-container {
            padding: 15px;
        }
        .app-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        .hub-title {
            font-weight: bold;
            color: #ff9800;
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        .bottom-nav {
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            background-color: #131826;
            display: flex;
            justify-content: space-around;
            padding: 10px 0;
            border-top: 1px solid #222b3c;
        }
        .nav-item {
            background: none;
            border: none;
            color: #8c9bae;
            cursor: pointer;
            font-size: 14px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .nav-item.active {
            color: #ff9800;
        }
        .card {
            background-color: #131826;
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 15px;
            text-align: center;
        }
    </style>
</head>
<body>

    <div class="app-container">
        <!-- الهيدر العلوي -->
        <header class="app-header">
            <div class="logo-area">
                <span class="hub-icon">⚡</span>
                <span class="hub-title">STICKER HUB</span>
            </div>
        </header>

        <!-- صفحة الرئيسية -->
        <div id="home-tab" class="tab-content active">
            <div class="card">
                <h3>أهلاً بك في صانع الملصقات المميز</h3>
                <p>الملصقات المميزة الاحترافية في التليجرام بلكششن وسورس المساعدة.</p>
            </div>
        </div>

        <!-- صفحة إنشاء ملصق -->
        <div id="create-tab" class="tab-content">
            <div class="card">
                <h3>تجربة صفصف - صنع ملصقات مميزة</h3>
                <p>اختر قالباً لبدء تصميم الملصق</p>
                <div style="border: 2px dashed #3a4b6c; padding: 20px; border-radius: 10px; margin-top: 10px;">
                    إرسال ملصق جديد ليصبح قالباً +
                </div>
            </div>
        </div>

        <!-- صفحة حزمي -->
        <div id="packs-tab" class="tab-content">
            <div class="card">
                <h3>حزمي وملصقاتي المنشأة</h3>
                <p>ليس لديك حزم ملصقات مسجلة حالياً.</p>
            </div>
        </div>
    </div>

    <!-- الشريط السفلي (Navigation Bar) -->
    <nav class="bottom-nav">
        <button class="nav-item" onclick="switchTab('packs-tab', this)">
            <span>📦</span>
            <span>حزمي</span>
        </button>
        <button class="nav-item" onclick="switchTab('create-tab', this)">
            <span>➕</span>
            <span>إنشاء ملصق</span>
        </button>
        <button class="nav-item active" onclick="switchTab('home-tab', this)">
            <span>🏠</span>
            <span>الرئيسية</span>
        </button>
    </nav>

    <script>
        function switchTab(tabId, element) {
            // إخفاء كل الصفحات
            document.querySelectorAll('.tab-content').forEach(tab => {
                tab.classList.remove('active');
            });
            
            // إزالة التفعيل من كل الأزرار
            document.querySelectorAll('.nav-item').forEach(btn => {
                btn.classList.remove('active');
            });
            
            // إظهار الصفحة المطلوبة وتفعيل زرها
            document.getElementById(tabId).classList.add('active');
            element.classList.add('active');
        }
    </script>
</body>
</html>
