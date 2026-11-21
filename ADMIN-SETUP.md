# لوحة تحكم موقع علاء سليم

هذه النسخة تبقي الموقع الحالي على GitHub Pages بنفس التصميم والرابط، وتضيف لوحة تحكم على:

`/admin/`

## ما الذي تغيّر؟

- انتقل محتوى الموقع من داخل `index.html` إلى `data/content.json`.
- أصبح الموقع يقرأ المحتوى من `data/content.json`.
- أضيفت لوحة Decap CMS في `admin/`.
- الصور الجديدة المرفوعة من اللوحة تحفظ في `img/` مع صور الموقع الحالية، حتى تظهر معاينات الصور الموجودة بشكل صحيح داخل اللوحة.
- كل حفظ من اللوحة ينشئ Commit في المستودع، ثم ينشر GitHub Pages التحديث تلقائياً بعد رفع هذه النسخة إلى المستودع.

## إعداد Decap Turbo

تم إنشاء موقع Turbo وربطه بمستودع GitHub الخاص بالموقع.

- Organization: `Alaa Saleem Design`
- Plan: Free
- Site name: `Alaa Saleem Portfolio`
- Site ID: `9cd510cc-a3fd-423f-9966-0985ad3eebc6`
- Git provider: GitHub
- Repo: `alaasaleemdesign/portfolio`
- Branch: `main`
- Config path: `admin/config.yml`
- Admin interface URL: `https://alaasaleemdesign.github.io/portfolio/admin/`

تم منح تطبيق Decap Turbo الوصول إلى مستودع `alaasaleemdesign/portfolio` فقط، وليس إلى كل المستودعات.

## خطوة التفعيل المتبقية

ارفع محتويات هذه الحزمة كما هي إلى جذر مستودع `alaasaleemdesign/portfolio` على فرع `main`، مع استبدال `index.html` الحالي وإضافة مجلدي `admin/` و`data/`. لا ترفع مجلد الحزمة نفسه كمجلد إضافي، بل ارفع الملفات والمجلدات الموجودة داخله.

بعد اكتمال رفع الملفات وتحديث GitHub Pages، افتح:

`https://alaasaleemdesign.github.io/portfolio/admin/`

ثم اتبع تسجيل الدخول الذي تظهره Decap Turbo.

## ملاحظات

- ملف `admin/config.yml` جاهز ويحتوي Site ID الفعلي.
- لا تحذف `data/content.json`؛ الموقع يعتمد عليه.
- معاينة Decap المدمجة معطلة لأن الصفحة تستخدم تنسيقاً مخصصاً؛ استخدم رابط الموقع للمعاينة بعد النشر.
- قبل استبدال النسخة الحالية، احتفظ بنسخة احتياطية من المستودع أو من ملف `index.html` الحالي.
