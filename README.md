<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sticker Hub - صانع ملصقات مميز</title>
    <link rel="stylesheet" href="style.css">
    <!-- استيراد خط مناسب وايقونات إذا تحتاج -->
</head>
<body>

    <div class="app-container">
        <!-- الهيدر العُلوي -->
        <header class="app-header">
            <div class="logo-area">
                <span class="hub-icon">⚡</span>
                <span class="hub-title">STICKER HUB</span>
            </div>
            <div class="top-actions">
                <button class="send-btn">📤</button>
            </div>
        </header>

        <!-- بطاقة الحساب والاشتراك -->
        <div class="profile-card">
            <div class="user-info">
                <div class="avatar-container">
                    <img src="https://via.placeholder.com/50" alt="Avatar" class="avatar">
                    <span class="status-dot"></span>
                </div>
                <div class="user-details">
                    <h3 class="username">صفصف لـ ۰۰۰۰۰۰</h3>
                    <p class="plan-status">أنت تستخدم الخطة المجانية الآن</p>
                </div>
            </div>
            <button class="subscribe-btn">
                <span class="crown">👑</span> اشترك
            </button>
        </div>

        <!-- استخدامك اليوم -->
        <div class="usage-box">
            <div class="usage-info">
                <span>استخدامك اليوم</span>
                <span class="usage-count">2 / 2</span>
            </div>
            <div class="progress-bar">
                <div class="progress-fill" style="width: 100%;"></div>
            </div>
        </div>

        <!-- الإحصائيات (ملصق مصمم وحزمة منشأة) -->
        <div class="stats-grid">
            <div class="stat-card">
                <div class="stat-icon pink-glow">✨</div>
                <h2 class="stat-number">2</h2>
                <p class="stat-label">ملصق مصمم</p>
            </div>
            <div class="stat-card">
                <div class="stat-icon purple-glow">📦</div>
                <h2 class="stat-number">23</h2>
                <p class="stat-label">حزمة منشأة</p>
            </div>
        </div>

        <!-- البانر الترويجي (فيديو / يوتيوب) -->
        <div class="promo-banner">
            <div class="banner-content">
                <h3>الملصقات المميزة الاحترافية في تليجرام بلاش!</h3>
                <p class="banner-sub">سورس العمدة</p>
            </div>
            <div class="video-preview">
                <div class="play-button">▶</div>
            </div>
        </div>

        <!-- الشريط السفلي (Navigation Bar) -->
        <nav class="bottom-nav">
            <a href="#" class="nav-item">
                <span class="nav-icon">📦</span>
                <span>حزمي</span>
            </a>
            <a href="#" class="nav-item">
                <span class="nav-icon plus-icon">+</span>
                <span>إنشاء ملصق</span>
            </a>
            <a href="#" class="nav-item active">
                <span class="nav-icon">🏠</span>
                <span>الرئيسية</span>
            </a>
        </nav>
    </div>

</body>
</html>
