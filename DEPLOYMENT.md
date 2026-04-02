# 📲 دليل نشر ميكروباصي على Google Play و App Store

## 🟢 الطريقة الأولى: PWABuilder (الأسهل — موصى بها)

### الخطوات:
1. **ادخل على** [pwabuilder.com](https://pwabuilder.com)
2. **اكتب الرابط:** `https://galalemad75-creator.github.io/mikrobassi/`
3. **اضغط** "Package for stores"
4. **اختر** "Android" → حمّل حزمة `.aab`
5. **ادخل** [Google Play Console](https://play.google.com/console)
6. **أنشئ تطبيق جديد** → ارفع ملف `.aab`
7. **املأ** معلومات التطبيق (الوصف، الصور، التصنيف)
8. **أرسل** للمراجعة

---

## 🔷 Google Play — خطوات تفصيلية

### ١. إنشاء حساب مطور
- روح [play.google.com/console](https://play.google.com/console)
- سجّل بحساب Google
- ادفع **$25 رسوم تسجيل** (مرة واحدة)

### ٢. إنشاء تطبيق جديد
- اضغط "Create app"
- **اسم التطبيق:** ميكروباصي
- **اللغة الافتراضية:** Arabic
- **نوع التطبيق:** App (ليس Game)
- **مجاني أم مدفوع:** حسب رغبتك

### ٣. ملء المعلومات المطلوبة

| الحقل | القيمة |
|-------|--------|
| Short description | تطبيق نقل ذكي بسيارات فان في مصر |
| Full description | ميكروباصي — تطبيق نقل ذكي متخصص في سيارات الفان 7 راكب. احجز رحلاتك بسهولة مع سائقين موثوقين وأسعار شفافة. وضع العائلة، مشاركة الموقع، وطوارئ مباشرة. |
| App category | Maps & Navigation / Transportation |
| Contact email | support@mikrobassi.com |
| Privacy policy URL | https://galalemad75-creator.github.io/mikrobassi/#privacy |

### ٤. رفع الصور المطلوبة

| الصورة | الحجم | الحالة |
|--------|-------|--------|
| App icon | 512×512 | ✅ موجود |
| Feature graphic | 1024×500 | ⚠️ تحتاج تصميم |
| Screenshots (2+) | 1080×1920 | ⚠️ لازم تاخذ سكرين شوتات |

### ٥. تصنيف المحتوى
- استبيان تصنيف →交通运输
- بدون محتوى عنيف أو بالغ

### ٦. إرسال للمراجعة
- عادة 1-3 أيام

---

## 🍎 Apple App Store — خطوات تفصيلية

### ١. اشتراك مطور
- روح [developer.apple.com](https://developer.apple.com)
- سجّل بحساب Apple
- ادفع **$99/سنة**

### ٢. تجهيز التطبيق (باستخدام Capacitor)

```bash
# تثبيت Capacitor
npm init -y
npm install @nickvdh/nickvdh @nickvdh/nickvdh/cli

# إضافة iOS
npx cap add ios

# بناء
npx cap sync
npx cap open ios

# من Xcode: Product → Archive → Upload
```

### ٣. App Store Connect
- روح [appstoreconnect.apple.com](https://appstoreconnect.apple.com)
- أنشئ تطبيق جديد
- ارفع الـ IPA من Xcode
- ملأ معلومات التطبيق

### ٤. معلومات مطلوبة

| الحقل | القيمة |
|-------|--------|
| App name | ميكروباصي |
| Subtitle | نقل ذكي في مصر |
| Category | Navigation |
| Privacy URL | https://galalemad75-creator.github.io/mikrobassi/#privacy |
| Support URL | https://galalemad75-creator.github.io/mikrobassi/ |

### ٥. Privacy Labels
- يجمع: الموقع، رقم الهاتف، التقييمات
- لا يشارك مع أطراف ثالثة

### ٦. مراجعة Apple
- عادة 2-7 أيام
- ممكن يرفضوا ويطلبوا تعديلات

---

## ⚡ نصائح للقبول من أول مرة

### Google Play:
✅ سياسة خصوصية — موجودة
✅ شروط استخدام — موجودة
✅ أيقونة 512×512 — موجودة
⚠️ لازم Feature Graphic 1024×500
⚠️ لازم 2+ سكرين شوتات
✅ لا محتوى مخالف
✅ يعمل بدون أخطاء

### App Store:
✅ Privacy Policy — موجودة
✅ Terms of Service — موجودة
⚠️ لازم screenshots لكل أحجام الشاشات
⚠️ لا تستخدم أيقونات Apple في التطبيق
✅ لا crashes أو bugs
✅ يعمل على آخر iOS

---

## 📁 الملفات المجهزة

```
mikrobassi/
├── .well-known/
│   ├── assetlinks.json          ← Digital Asset Links (لـ TWA)
│   └── apple-app-site-association ← Universal Links (لـ iOS)
├── manifest.json                ← PWA Manifest
├── sw.js                        ← Service Worker
├── icons/                       ← كل الأحجام
└── index.html                   ← التطبيق
```

---

## 🚀 خطوات سريعة (Google Play فقط)

1. **حمّل** من PWABuilder.com → ملف `.aab`
2. **ادخل** Google Play Console
3. **ارفع** الملف
4. **املأ** المعلومات
5. **أرسل** للمراجعة
6. **انتظر** 1-3 أيام ✅

---

**بالتوفيق! 🚐**
