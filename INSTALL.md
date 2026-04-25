# 🏢 عقاراتي Pro — دليل التثبيت

## ⚡ الطريقة الأسرع: PWA (تثبيت فوري على الجوال)

1. افتح ملف `عقاراتي-Pro.html` على هاتفك
2. في متصفح Chrome: القائمة ← "إضافة إلى الشاشة الرئيسية"
3. التطبيق سيظهر كأيقونة على هاتفك تماماً كـ APK

---

## 📦 بناء APK حقيقي

### الطريقة 1: GitHub Actions (الأسهل)
1. أنشئ repository على GitHub
2. ارفع محتويات هذا المجلد
3. سيبني GitHub Actions الـ APK تلقائياً
4. حمّل الـ APK من قسم "Actions → Artifacts"

### الطريقة 2: Capacitor (محلياً)
```bash
# المتطلبات: Node.js + Android Studio
npm install
npx cap add android
npx cap sync
# افتح Android Studio:
npx cap open android
# ثم: Build → Build Bundle(s) / APK(s) → Build APK(s)
```

### الطريقة 3: PWA Builder (مباشر من الإنترنت)
1. اذهب إلى https://www.pwabuilder.com
2. ارفع ملف `عقاراتي-Pro.html`
3. اختر Android → حمّل APK

### الطريقة 4: WebIntoApp.com
1. اذهب إلى https://webintoapp.com
2. ارفع الملف أو ضع رابطه
3. حمّل APK جاهز

---

## 📱 ملفات المشروع

| الملف | الوصف |
|-------|-------|
| `عقاراتي-Pro.html` | التطبيق الكامل (ملف واحد) |
| `capacitor.config.json` | إعدادات Capacitor للبناء |
| `package.json` | تبعيات Node.js |
| `.github/workflows/` | بناء تلقائي على GitHub |
| `android/` | مشروع Android كامل |

---

## 🌐 التشغيل المباشر (بدون تثبيت)
فتح `عقاراتي-Pro.html` في أي متصفح — يعمل 100% بدون إنترنت
