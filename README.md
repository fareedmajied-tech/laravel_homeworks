# تكاليف لارفل — وفاء النبهاني

مشروع Laravel لتكاليف مادة لارفل النظري والعملي.

## المتطلبات

- PHP 8.2 أو أحدث
- Composer
- SQLite (مُعد افتراضيًا) أو قاعدة بيانات أخرى تدعمها Laravel
- Node.js و npm عند تعديل ملفات الواجهة

## التشغيل المحلي

```powershell
composer install
Copy-Item .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

افتح `http://127.0.0.1:8000` في المتصفح. تأكد من ضبط اتصال قاعدة البيانات في `.env` قبل تشغيل الترحيلات إذا لم تستخدم SQLite.

## الواجهة الأمامية

```powershell
npm install
npm run dev
```

ولإنشاء ملفات الإنتاج:

```powershell
npm run build
```

## الاختبارات

```powershell
php artisan test
```

المشروع مبني على Laravel 12، المتوافق مع PHP 8.2.
