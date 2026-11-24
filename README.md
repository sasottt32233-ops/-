# نشر عداد النشر على GitHub Pages (مجاني)
1. في Apps Script: ضع آخر نسخة من Code.gs (فيها doPost)، ثم Deploy ← Manage deployments ← ✏️ ← New version. (Execute as: Me / Anyone).
2. **مهم للأمان:** مستودع GitHub العام يعرض رابطك لكل الناس. أضف في Project Settings ← Script properties الخاصية ACCESS_KEY بكلمة سر طويلة. التطبيق يطلبها مرة واحدة على كل جهاز ويتذكرها.
3. افتح config.js وضع رابط النشر (المنتهي بـ /exec).
4. على github.com: New repository (مثلاً post-counter) ← Add file ← Upload files ← ارفع كل ملفات هذا المجلد (index.html وconfig.js وsw.js وmanifest.webmanifest وicon-192.png وicon-512.png) ← Commit.
5. Settings ← Pages ← Source: Deploy from a branch ← Branch: main و/ (root) ← Save. بعد دقيقة يظهر رابط https://اسمك.github.io/post-counter/
6. على الهاتف: افتح الرابط في Chrome ← ⋮ ← "تثبيت التطبيق" (Install app). يظهر كتطبيق مستقل بأيقونة.
## ملاحظات
- عند تعديل الملفات غيّر V في sw.js (مثلاً pc-v2) ليتحدّث التطبيق عند المستخدمين.
- لا ترفع Code.gs إلى GitHub، فهو يبقى في Apps Script.
- نفس الجدول والبيانات على الكمبيوتر والهاتف.
