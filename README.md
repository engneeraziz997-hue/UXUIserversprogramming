# دليل رفع مشروع Synthetic AI إلى GitHub

> دليل عملي لرفع موقع وكالة "سينثيتيك" واستضافته على GitHub Pages

---

## المتطلبات المسبقة

قبل البدء، تأكد من توفر الأدوات التالية على جهازك:

| الأداة | الغرض | رابط التحميل |
|--------|-------|--------------|
| **Git** | نظام التحكم بالإصدارات | [git-scm.com](https://git-scm.com/downloads) |
| **GitHub Account** | لإنشاء المستودعات | [github.com/signup](https://github.com/signup) |
| **VS Code** (اختياري) | محرر أكواد متقدم | [code.visualstudio.com](https://code.visualstudio.com) |

---

## الخطوة 1: إنشاء مستودع جديد على GitHub

1. سجّل الدخول إلى [github.com](https://github.com)
2. اضغط على زر **➕ New** في أعلى الصفحة
3. أدخل اسم المستودع: `synthetic-ai-agency`
4. اختر **Public** (لاستضافة GitHub Pages المجانية)
5. ✅ **اشرك** خيار "Add a README file"
6. اضغط **Create repository**

---

## الخطوة 2: تجهيز الملفات محلياً

### 2.1 إنشاء مجلد المشروع

افتح الطرفية (Terminal) ونفّذ الأوامر التالية:

```bash
# إنشاء مجلد المشروع
mkdir synthetic-ai-agency
cd synthetic-ai-agency

# نسخ ملفات المشروع
# انسخ الملفات التالية إلى هذا المجلد:
# - index.html
# - DESIGN.md
# - screen.png
# - أي ملفات أصول أخرى (CSS, JS, صور)
```

### 2.2 هيكل الملفات المتوقع

```
synthetic-ai-agency/
├── index.html          ← الصفحة الرئيسية
├── DESIGN.md           ← وثيقة التصميم
├── screen.png          ← لقطة شاشة
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   └── main.js
│   └── images/
│       └── hero-bg.jpg
└── README.md           ← ملف التوثيق
```

---

## الخطوة 3: تهيئة Git ورفع الملفات

### 3.1 ربط المجلد بـ Git

```bash
# تهيئة Git في المجلد
git init

# إضافة الملفات إلى المنطقة المؤقتة
git add .

# إنشاء أول commit
git commit -m "🚀 الإصدار الأول: إطلاق موقع وكالة Synthetic AI"
```

### 3.2 ربط المستودع المحلي بالبعيد

ارجع إلى صفحة مستودعك على GitHub وانسخ رابط المستودع (HTTPS أو SSH):

```bash
# ربط المستودع المحلي بالبعيد
# استبدل USERNAME باسم المستخدم الخاص بك
git remote add origin https://github.com/USERNAME/synthetic-ai-agency.git

# رفع الملفات إلى الفرع الرئيسي
git branch -M main
git push -u origin main
```

---

## الخطوة 4: تفعيل GitHub Pages (الاستضافة المجانية)

1. في مستودعك على GitHub، اذهب إلى تبويب **Settings**
2. من القائمة الجانبية، اختر **Pages**
3. في قسم "Build and deployment":
   - **Source**: اختر `Deploy from a branch`
   - **Branch**: اختر `main` / `root`
4. اضغط **Save**

> ⏳ انتظر من 30 ثانية إلى دقيقتين، ثم ستجد رابط موقعك متاحاً على شكل:
> `https://USERNAME.github.io/synthetic-ai-agency/`

---

## الخطوة 5: التحديثات المستقبلية

عند إجراء أي تعديل على الموقع، استخدم هذه الأوامر لرفع التحديثات:

```bash
# مراجعة التغييرات
git status

# إضافة التغييرات
git add .

# إنشاء commit جديد
git commit -m "✨ وصف التعديل: تحسين الأداء / إضافة قسم جديد"

# رفع التحديثات
git push origin main
```

---

## 🛠️ أوامر Git السريعة (مرجع)

| الأمر | الوظيفة |
|-------|---------|
| `git status` | عرض حالة الملفات |
| `git log --oneline` | عرض سجل التعديلات |
| `git pull origin main` | سحب آخر التحديثات |
| `git checkout -b feature-x` | إنشاء فرع جديد |
| `git merge feature-x` | دمج فرع مع الفرع الحالي |

---

## ⚠️ نصائح مهمة

1. **لا ترفع ملفات حساسة**: أضف ملف `.gitignore` يحتوي على:
   ```
   .env
   node_modules/
   .DS_Store
   ```

2. **تحسين الأداء**: قبل الرفع، تأكد من:
   - ضغط الصور (استخدم [tinypng.com](https://tinypng.com))
   - تقليل حجم ملفات CSS/JS

3. **تخصيص النطاق**: يمكنك ربط نطاق خاص (Domain) بـ GitHub Pages من إعدادات Pages

---


---

**تم إعداد هذا الدليل بواسطة مساعد Synthetic AI 🧠**
