# 🚀 Droy Code Editor

<p align="center">
  <img src="https://img.shields.io/badge/Droy-1.0.125-purple?style=for-the-badge&logo=code" alt="Droy 100%">
  <img src="https://img.shields.io/badge/Version-1.0.0-blue?style=for-the-badge" alt="Version 1.0.0">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License">
</p>

<p align="center">
  <strong>محرر أكواد مكتوب بالكامل بلغة Droy</strong>
</p>

---

## 📋 نظرة عامة

**Droy Code Editor** هو محرر أكواد متكامل مكتوب 100% بلغة برمجة Droy. يدعم:

- ✅ تلوين الصيغة (Syntax Highlighting)
- ✅ مفسر Droy مدمج
- ✅ مستكشف الملفات
- ✅ طرفية مدمجة
- ✅ الوضع الداكن/الفاتح
- ✅ إدارة الملفات

---

## 📁 هيكل المشروع

```
droy-editor-droy/
├── src/
│   └── main.droy              # الملف الرئيسي
├── lib/
│   ├── core.droy              # الوظائف الأساسية
│   ├── ui.droy                # واجهة المستخدم
│   ├── editor.droy            # محرر الأكواد
│   ├── interpreter.droy       # مفسر Droy
│   └── filemanager.droy       # إدارة الملفات
├── assets/
│   └── (الأصول والصور)
└── README.md
```

---

## 🚀 كيفية التشغيل

### المتطلبات

- مترجم Droy (droy-lang)
- LLVM

### التشغيل

```bash
# استنساخ المستودع
git clone https://github.com/droy-go/droy-lang.git
cd droy-editor-droy

# بناء المشروع
droy build src/main.droy -o droy-editor

# التشغيل
./droy-editor
```

---

## 💻 مثال على الاستخدام

```droy
// إنشاء محرر جديد
var editor = new DroyEditor()

// تهيئة المحرر
editor.init()

// كتابة كود
editor.updateContent("// Hello World\nem \"Hello, Droy!\"")

// تشغيل الكود
editor.runCode()

// حفظ الملف
editor.saveFile()
```

---

## 🎯 المميزات

### 1. تلوين الصيغة
- دعم كامل لكلمات Droy المفتاحية
- تلوين المتغيرات الخاصة (`@var`)
- تلوين النصوص والأرقام

### 2. المفسر المدمج
- تنفيذ كود Droy مباشرة
- دعم المتغيرات والدوال
- دعم الأصناف والوراثة

### 3. مستكشف الملفات
- شجرة ملفات تفاعلية
- إنشاء/حذف/إعادة تسمية الملفات
- تصفح المجلدات

### 4. الطرفية المدمجة
- عرض نتائج التنفيذ
- عرض الأخطاء
- سجل العمليات

---

## 📝 لغة Droy

### المتغيرات
```droy
var name = "Droy"
~s @si = 100
set @ui = 200
```

### الدوال
```droy
fn greet(user) {
    ret "Hello, " + user
}
```

### الأصناف
```droy
class Person {
    var name: string
    fn constructor(n: string) {
        this.name = n
    }
}
```

### الكتل
```droy
block myBlock {
    em "Block executed"
}
myBlock
```

---

## 🔧 التطوير

### إضافة ميزة جديدة

1. أنشئ ملف `.droy` في مجلد `lib/`
2. اربطه في `main.droy`:
```droy
link id: "mymodule" api: "./lib/mymodule.droy"
pkg load "mymodule"
```

### بناء المشروع

```bash
droy build src/main.droy -o droy-editor --release
```

---

## 📄 الترخيص

MIT License - راجع ملف LICENSE للتفاصيل.

---

<p align="center">
  <strong>صنع بـ ❤️ بلغة Droy</strong>
</p>

<p align="center">
  🌟 لا تنسَ إعطاء نجمة للمشروع! 🌟
</p>
