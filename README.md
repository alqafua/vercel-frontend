# RSI Scanner Pro — Vercel + Railway

## الهيكل
- **Vercel** → الواجهة (public/index.html)
- **Railway** → السيرفر (Node.js + WebSocket)

## خطوات النشر

### 1. Railway (السيرفر)
1. روح [railway.app](https://railway.app) → New Project
2. **Deploy from GitHub** أو **Deploy from local**
3. ارفع مجلد `railway-server/`
4. أضف Environment Variables:
   ```
   PORT=3000
   JWT_SECRET=اكتب_كلمة_سر_عشوائية
   ALLOWED_ORIGINS=https://your-app.vercel.app
   NODE_ENV=production
   ```
5. انسخ الرابط: `https://xxx.up.railway.app`

### 2. Vercel (الواجهة)
1. روح [vercel.com](https://vercel.com) → New Project
2. ارفع مجلد `vercel-frontend/`
3. لا تحتاج إعدادات إضافية
4. بعد النشر ← افتح الرابط

### 3. الإعداد الأول
- افتح رابط Vercel في المتصفح
- ستظهر شاشة "إعداد السيرفر"
- أدخل رابط Railway: `https://xxx.up.railway.app`
- اضغط ✅ حفظ والمتابعة
- سجّل دخول: **Alqafua / 7007**

## ملاحظة مهمة
Railway مجاني بحد **500 ساعة/شهر** (كافي لسيرفر واحد 24/7)
لو تبي بدون حدود → اشترك بـ **5$/شهر**
