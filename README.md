# 🎵 فروشگاه حرفه‌ای آهنگ و موسیقی

> یک سامانه جامع و امن برای عرضه، معرفی، پیش‌نمایش و فروش آثار موسیقی دیجیتال

## 🎯 اهداف پروژه

- 🎧 **پیش‌نمایش آهنگ‌ها** برای تمام کاربران
- 🔐 **دانلود امن** فقط برای خریداران تأیید‌شده
- 💬 **ارتباط مستقیم** کاربر و مدیریت
- 📊 **پنل مدیریت حرفه‌ای** برای کنترل کامل سامانه
- 📱 **رابط واکنش‌گرا** برای تمام دستگاه‌ها
- 🎨 **طراحی لوکس و مدرن** الهام‌گرفته از استودیوهای موسیقی

## 🛠️ فناوری‌های استفاده‌شده

### Backend
- **Python 3.10+**
- **Django 4.2+**
- **Django REST Framework**
- **PostgreSQL**
- **Celery** (برای تسک‌های async)
- **Redis** (برای caching و Celery)

### Frontend
- **HTML5**
- **CSS3**
- **JavaScript (ES6+)**
- **Bootstrap 5**
- **Responsive Design**

### DevOps
- **Docker & Docker Compose**
- **Gunicorn**
- **Nginx**

## 📁 ساختار پروژه

```
music-shop/
├── backend/                    # اپلیکیشن Django
│   ├── manage.py
│   ├── requirements.txt
│   ├── .env.example
│   ├── config/                 # تنظیمات اصلی
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── wsgi.py
│   │   └── asgi.py
│   │
│   ├── apps/                   # اپلیکیشن‌های مختلف
│   │   ├── accounts/           # مدیریت کاربران
│   │   ├── music/              # مدیریت آهنگ‌ها
│   │   ├── artists/            # مدیریت هنرمندان
│   │   ├── categories/         # مدیریت دسته‌بندی‌ها
│   │   ├── purchases/          # مدیریت خریدها
│   │   ├── downloads/          # مدیریت دانلودها
│   │   ├── messaging/          # سیستم پیام‌ها
│   │   ├── notifications/      # سیستم اعلان‌ها
│   │   ├── blog/               # وبلاگ
│   │   ├── contact/            # تماس با ما
│   │   ├── dashboard/          # داشبورد مدیریت
│   │   └── core/               # عملکردهای عمومی
│   │
│   ├── media/                  # فایل‌های آپلود‌شده
│   │   ├── previews/           # فایل‌های پیش‌نمایش
│   │   ├── full_tracks/        # فایل‌های کامل (Private)
│   │   └── covers/             # تصاویر کاور
│   │
│   ├── static/                 # فایل‌های static
│   │   ├── css/
│   │   ├── js/
│   │   └── images/
│   │
│   ├── templates/              # الگو‌های HTML
│   │   ├── base.html
│   │   ├── accounts/
│   │   ├── music/
│   │   ├── dashboard/
│   │   └── ...
│   │
│   └── logs/                   # فایل‌های log
│
├── frontend/                   # رابط کاربری (اختیاری - React/Next.js)
│
├── docker/                     # فایل‌های Docker
│   ├── Dockerfile
│   ├── docker-compose.yml
│   └── nginx.conf
│
├── docs/                       # مستندات پروژه
│
└── scripts/                    # اسکریپت‌های مفید
```

## 🚀 شروع سریع

### 1. نیازمندی‌ها
- Python 3.10+
- PostgreSQL 12+
- Redis (اختیاری)
- Git

### 2. نصب
```bash
# Clone repository
git clone https://github.com/ahmadi2015/music-shop.git
cd music-shop

# ایجاد Virtual Environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# نصب وابستگی‌ها
cd backend
pip install -r requirements.txt

# تنظیم فایل .env
cp .env.example .env
# ویرایش .env با تنظیمات خود

# اجرای Migration‌ها
python manage.py migrate

# ایجاد Super User
python manage.py createsuperuser

# جمع‌آوری Static Files
python manage.py collectstatic

# اجرای سرور
python manage.py runserver
```

## 📚 API Documentation

اطلاعات کامل API در `/api/docs/` موجود است.

## 🔐 امنیت

- ✅ CSRF Protection
- ✅ XSS Prevention
- ✅ SQL Injection Protection
- ✅ Secure File Storage
- ✅ Permission Management
- ✅ Rate Limiting
- ✅ HTTPS Support

## 📖 مستندات

بیشتر اطلاعات در پوشه `docs/` موجود است:
- [نصب و راه‌اندازی](docs/INSTALLATION.md)
- [معماری سامانه](docs/ARCHITECTURE.md)
- [API Reference](docs/API.md)
- [مدل‌های داده](docs/DATABASE.md)

## 👥 مشارکت

این پروژه برای استفاده شخصی ایجاد شده است.

## 📄 لایسنس

MIT License

## 📞 تماس

برای سؤالات و پیشنهادات تماس بگیرید.

---

**ساخت‌شده با ❤️ برای دوستداران موسیقی**
