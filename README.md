# ملخصات الأنمي

واجهة ثابتة (public/) + دالة Serverless (api/summary.js) لتوليد الملخصات.

## تشغيل محلي
1. `npm i -g vercel`
2. `cp .env.example .env` وحط `ANTHROPIC_API_KEY`
3. `vercel dev` ثم افتح http://localhost:3000

## الرفع على Vercel
1. ارفع المجلد على GitHub.
2. Vercel > Add New Project > اختر الريبو.
3. Settings > Environment Variables: أضف `ANTHROPIC_API_KEY` (و`ANTHROPIC_MODEL` اختياري).
4. Deploy.

> الكاش الحالي في /tmp مؤقت على Vercel. للدوام استخدم Vercel KV أو Upstash Redis.
