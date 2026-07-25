
<div align="center">

# ⚡ SYNTHETIC — وكالة سينثيتيك لأتمتة الذكاء الاصطناعي

**أتمتة مستقبل عملك بذكاء اصطناعي متقدم**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=flat&logo=github&logoColor=white)](https://pages.github.com)

</div>

---

## 🧠 نظرة عامة

موقع وكالة **سينثيتيك** هو واجهة تفاعلية عالية الأداء تعرض حلول أتمتة الذكاء الاصطناعي للمؤسسات. صُمم الموقع بأسلوب "الكينتيك مونوليث" (Kinetic Monolith) — مزيج من البنائية القاسية والطاقة الرقمية المتفجرة، باستخدام لوحة ألوان داكنة مبنية على الأخضر العميق والنيون الأخضر المشع.

> 🎯 **الهدف**: تحويل المهام اليدوية إلى تدفقات عمل ذكية ومستقلة تضاعف الإنتاجية دون زيادة في عدد الموظفين.

---

## ✨ المميزات الرئيسية

| الميزة | الوصف |
|--------|-------|
| 🎨 **تصميم عصري** | واجهة داكنة بتدرجات أخضر النيون مع تأثيرات Glassmorphism |
| 📱 **تصميم متجاوب** | يعمل بسلاسة على جميع أحجام الشاشات (هاتف، تابلت، ديسكتوب) |
| ⚡ **أداء فائق** | استخدام Tailwind CSS CDN مع تحميل مُحسّن |
| 🔤 **دعم العربية** | واجهة عربية كاملة باتجاه RTL مع خط IBM Plex Sans Arabic |
| 🖼️ **بطاقات زجاجية** | تأثير blur وشفافية عالية لعمق بصري |
| 🟢 **مؤشرات حية** | نقاط نبض (Data Pulse) تشير إلى حالة النظام |

---

## 🖼️ لقطة شاشة

![لقطة شاشة لموقع Synthetic AI](screen.png)

---

## 🛠️ التقنيات المستخدمة

- **HTML5** — الهيكل الأساسي للصفحة
- **Tailwind CSS** — إطار التصميم المسؤول عن الألوان، المسافات، والتخطيط
- **Google Fonts** — خطوط IBM Plex Sans Arabic و Inter
- **Material Symbols** — أيقونات Google المادية
- **JavaScript (Vanilla)** — التفاعلات والرسوم المتحركة

---

## 📁 هيكل الملفات

```
synthetic-ai-agency/
├── index.html          ← الصفحة الرئيسية (واجهة الموقع الكاملة)
├── DESIGN.md           ← وثيقة نظام التصميم (Design System)
├── screen.png          ← لقطة شاشة للموقع
└── README.md           ← هذا الملف
```

> **ملاحظة**: الموقع مبني كصفحة واحدة (Single Page) تعتمد على Tailwind CSS عبر CDN، مما يلغي الحاجة لملفات CSS/JS منفصلة.

---

## 🎨 نظام التصميم (Design System)

### "الكينتيك مونوليث" — The Kinetic Monolith

يتحرك المشروع بعيداً عن قوالب الوضع الداكن التقليدية. يُشعر المستخدم بأنه يتعامل مع قطعة أجهزة عالية الأداء حية.

### اللون الأساسي — "الأخضر المشع" (Radioactive Neon)

| الدور | اللون | الكود |
|-------|-------|-------|
| الخلفية الأساسية | أسود أخضر عميق | `#001204` |
| النص الأساسي | أخضر فاتح ناعم | `#d1fcd2` |
| اللون الأساسي | أخضر نيون مشع | `#39FF14` |
| اللون الثانوي | بنفسجي فاتح | `#ac89ff` |
| النص الثانوي | أخضر رمادي | `#8cb58f` |

### القواعد التصميمية الرئيسية

- ❌ **ممنوع استخدام الحدود (Borders)** — الحدود الفاصلة تُعتبر فشلاً تصميمياً
- ✅ **التدرجات اللونية** — لتحديد الحدود عبر تغيير الخلفية والفراغات
- ✅ **Glassmorphism** — بطاقات شفافة مع `backdrop-filter: blur(20px)`
- ✅ **التدرج المائل** — زر CTA بتدرج 135° من `#8eff71` إلى `#2ff801`
- ✅ **الخط Space Grotesk** — شعور تقني هندسي بدون التضحية بالوضوح

---

## 🚀 طريقة التشغيل

### 1. تشغيل محلي

بما أن المشروع لا يحتاج إلى build، يمكنك تشغيله مباشرة:

```bash
# استنساخ المستودع
git clone https://github.com/USERNAME/synthetic-ai-agency.git
cd synthetic-ai-agency

# فتح الملف في المتصفح
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

### 2. الاستضافة على GitHub Pages

1. ارفع الملفات إلى مستودع GitHub
2. اذهب إلى **Settings → Pages**
3. اختر المصدر: `Deploy from a branch` → `main` → `/ (root)`
4. احفظ الإعدادات وانتظر دقيقة
5. الموقع سيُنشر على: `https://USERNAME.github.io/synthetic-ai-agency/`

---

## 📐 الأقسام الرئيسية للموقع

| القسم | المحتوى |
|-------|---------|
| **الشريط العلوي** | شعار SYNTHETIC + روابط التنقل + زر CTA |
| **الهيرو (Hero)** | عنوان ضخم + وصف + أزرار رئيسية + خلفية شبكة عصبية |
| **الخدمات** | 4 بطاقات زجاجية (أتمتة، روبوتات، تحليلات، تكامل) |
| **دراسات الحالة** | شبكة Bento Grid مع إحصائيات ومميزات |
| **اتصل بنا** | نموذج تواصل + معلومات الاتصال |
| **التذييل** | روابط النظام البيئي والقانونية + حالة الشبكة |

---

## 📝 الترخيص

هذا المشروع مفتوح المصدر تحت رخصة **MIT**.

```
MIT License

Copyright (c) 2024 Synthetic AI Agency

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

<div align="center">

**🟢 الشبكة متصلة — النظام العصبي نشط**

صُمم بإتقان بواسطة فريق Synthetic AI

</div>
