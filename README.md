# 📝 Task: Personal Task Manager API (Express.js + Auth)

أهلاً بك في التحدي التقني! المطلوب بناء Back-end API لإدارة مهام شخصية. الهدف تقييم مهاراتك في بناء RESTful APIs، إدارة البيانات، وتأمين الواجهات.

---

## 🚀 المطلوب (The Mission)
Build a simple server where users can register/login and manage their personal task lists.

- كل مستخدم يستطيع إنشاء، قراءة، تعديل، وحذف المهام الخاصة به فقط.

### 1) نظام المستخدمين والـ Auth
- Sign up: تسجيل باسم، إيميل، وكلمة مرور.
- Login: عند النجاح يرجع JWT token.
- Security: كلمات المرور يجب أن تكون مشفرة (bcrypt).

### 2) إدارة المهام (Tasks)
- كل "مهمة" تتضمن: العنوان، الوصف، حالة الإنجاز، وتاريخ الإضافة.
- Create Task: إضافة مهمة مرتبطة بالمستخدم.
- Get My Tasks: جلب مهام المستخدم الحالي فقط.
- Update/Delete: تعديل أو حذف مهمة — فقط صاحب المهمة يمكنه ذلك.

### 3) المتطلبات التقنية
- Environment: Express.js (Node.js)
- Database: MongoDB (Mongoose) أو MySQL (Sequelize/TypeORM)
- Validation: تأكد من صحة المدخلات (مثال: email format، title required).

---

## 🛠️ كيف رح نقيم الشغل؟ (Evaluation Criteria)
- Clean Code: تنظيم الملفات ووضوح المسؤوليات (controllers, models, routes).
- Error Handling: تعامل واضح مع الأخطاء (مثل: duplicate email، invalid IDs).
- Middlewares: استخدام مصادقة ومسارات محمية (JWT middleware).
- GitHub: وجود `.gitignore` وcommits منظمة (لا ترفع `node_modules` أو `.env`).

---

## ✅ طريقة التسليم (Delivery)
1. ادفع الكود على repository خاص في GitHub.
2. عدّل هذا الملف `README.md` ليشرح كيفية تشغيل المشروع محلياً.
3. أرسل رابط المستودع.

---

## مثال سريع لتشغيل محلي
1. تثبيت الاعتمادات:

```bash
npm install
```

2. إعداد ملف `.env` (مثال):

```
PORT=3000
MONGO_URI=mongodb://localhost:27017/task-manager
JWT_SECRET=your_jwt_secret
```

3. تشغيل الخادم:

```bash
npm run dev
```

---
