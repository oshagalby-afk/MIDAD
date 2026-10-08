# بيان حزمة مِداد | MIDAD-Netlify-source.zip

**الجذر داخل الأرشيف:** `MIDAD-Netlify-source/`  
**الاستخدام:** مصدر المشروع الحالي القابل للتثبيت والاختبار والبناء إلى Netlify؛ ليس ملف HTML واحدًا.

## قواعد الحزمة

- تشمل المصدر والاختبارات والوثائق والأصول، إضافة إلى ناتج `dist/` الحالي القابل لإعادة البناء.
- تشمل `.env.example` فقط؛ **لا تشمل `.env` أو مفاتيح أو قاعدة SQLite أو بيانات مستخدمين**.
- لا تشمل `node_modules/` أو `.git/` أو بيانات التشغيل المؤقتة؛ يعاد تثبيت الاعتماديات عبر `npm ci`.
- `SHA256SUMS.txt` يحوي بصمات SHA-256 لكل ملف ضمن المصدر والوثائق (ومنها هذا البيان)، ولا يحتوي بصمة ذاته.
- الملفات المبنية داخل `dist/` أصول عامة فقط؛ راجع `PROJECT_AUDIT.md` و`NETLIFY_DEPLOYMENT_AR.md` لحدود Netlify وعدم الاتصال الحي.

## الملفات

| المسار النسبي | الحجم بالبايت | SHA-256 | الوصف |
|---|---:|---|---|
| `.env.example` | 920 | `baa64dc99db27b72fb61bd9723e579bc3d8e42cfc14272ee0be6cd3878dfac59` | مثال أسماء إعدادات فقط، بلا قيم أسرار. |
| `.gitignore` | 104 | `7839288226681612e89dd93eb7c8fd7e440b2496f188ea02b17b0c2ca3a6d855` | استثناءات Git وملفات البيئة والبيانات المحلية. |
| `NETLIFY_DEPLOYMENT_AR.md` | 8,062 | `fd2fd344691b1e0dce5f1c1214b2764a66e1b104a20b804c7de141a6a2fbbed3` | تجهيز Netlify وتكاليفه وحدوده الموثقة. |
| `PROJECT_AUDIT.md` | 18,758 | `fa71d64d1d8992a036ae16d8ab290ca1113a44d6f19aeca1414114a572e81717` | تقرير التدقيق ومصفوفة حالة المزايا والاختبارات. |
| `README.md` | 9,921 | `5f691acec5b0d7fb4d470edfbca0c01bb982567090c9a568f9dc6d1c042d9efc` | دليل عربي للتشغيل وإعداد البيئة وحدود النسختين. |
| `RESEARCH_SOURCES.md` | 3,212 | `064ef8340fad359f7652ea41c001b92f391ec218da799b4987b6d510d963055f` | مصادر Netlify/البحث الموثقة في المشروع. |
| `SECURITY.md` | 9,940 | `f6743c5f614b712ce319338b4fcacb4c516cab2480d2e6350d1513b75c14936a` | مراجعة ضوابط الأمان والمخاطر المتبقية. |
| `SOURCE_RECOVERY.md` | 1,143 | `da5eb29a55d67273e9236c51e259bdb1bfc00a27600fce1b39bb6f4cd20cb835` | حدود استعادة المصدر المرفق. |
| `_headers` | 651 | `23b17da8385222dce5c7602fc67fe2039ed9e8d73abc0be7b0c7605d753ddede` | ترويسات النشر والسياسات الأمنية. |
| `ai-provider.mjs` | 2,426 | `ce3b4d4111d657db4b9005efdfd925472741311d47ce401b4ff055901be7b2bb` | مهايئ مزود AI على الخادم المحلي. |
| `ai-service.mjs` | 18,406 | `8146636fd0ccf16adf61da0fb456cf20fcca34e78c03a81d17d36cd2c36ef865` | RAG وسياق المحادثة ومراجع الإجابات. |
| `ai-service.test.mjs` | 3,544 | `dea9de8f0c7726b6ecbd0d395d254fe860a5f8df5e5b098872f65d509615db28` | اختبارات AI والعزل وسياق المحادثة. |
| `app.js` | 109,122 | `453b3787cbe3c20685414cd916bb2fcad7d2bd4f24add1c8fac5332ec6a6992d` | الواجهة وتفاعلات التعلم والبحث والمكتبة وPWA. |
| `bootstrap.mjs` | 16,548 | `44b94def36ea4e5ed37773c7f6ae9de2a186c54e4e423637d01e388f96f37160` | تسجيل الدخول والجلسات والمزامنة واللغة. |
| `database.mjs` | 16,390 | `ffe8b462d1e8d2b7f33565321dcac88154f48efe0b1e11c459676b8e04a060b8` | مخطط SQLite ومستودعات البيانات المحلية. |
| `dist/_headers` | 651 | `23b17da8385222dce5c7602fc67fe2039ed9e8d73abc0be7b0c7605d753ddede` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/app.js` | 109,122 | `453b3787cbe3c20685414cd916bb2fcad7d2bd4f24add1c8fac5332ec6a6992d` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/bootstrap.mjs` | 16,548 | `44b94def36ea4e5ed37773c7f6ae9de2a186c54e4e423637d01e388f96f37160` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/file-policy.mjs` | 3,183 | `f4b42856609ebcc80bbd9f7142533e02e262bcd0de69b176053bb758d21014af` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/icon.svg` | 419 | `ac9784130f7861a9bc06714f652da960ad28e137b95eeb97e3d82bc6b127837e` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/index.html` | 9,242 | `c350153db359621099098b5bd271043ce289398b3c56703cf8cb28d72f9fd04c` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/manifest.webmanifest` | 446 | `1fa3d95d6efaa66cdb48f05a2c659a6e4e058df7361489c784ef73a3cf70182f` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/styles.css` | 33,610 | `1ddbd4eb77565a9bf874ee5ec9aee04e4adacf7f486c98e93b59367e42f2f674` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `dist/sw.js` | 1,664 | `33c51277a6aecf5a950ab0fd64d2fae34694955fc92bb809dc7a71544d167457` | ناتج Netlify المنشور: أصل عام نُسخ من المصدر. |
| `file-policy.mjs` | 3,183 | `f4b42856609ebcc80bbd9f7142533e02e262bcd0de69b176053bb758d21014af` | تحقق الملفات والحدود قبل التخزين. |
| `file-processing.mjs` | 3,390 | `2c7837cc515acca454fe0b24d62ad626c3cc50260b35aeb0bcda5573db3c0f14` | استخراج النص المحلي وتقسيمه وفهرسته. |
| `icon.svg` | 419 | `ac9784130f7861a9bc06714f652da960ad28e137b95eeb97e3d82bc6b127837e` | أيقونة التطبيق المتجهة. |
| `index.html` | 9,242 | `c350153db359621099098b5bd271043ce289398b3c56703cf8cb28d72f9fd04c` | قشرة الواجهة وبيانات PWA وحقول الدخول. |
| `manifest.webmanifest` | 446 | `1fa3d95d6efaa66cdb48f05a2c659a6e4e058df7361489c784ef73a3cf70182f` | هوية PWA وأيقوناتها. |
| `netlify.toml` | 180 | `1856a37971d6d19a207eff8bff5c078dde21fea5c90029f41a291760d4365aad` | تعريف build وFunctions وتوجيه API. |
| `netlify/api.mjs` | 28,152 | `721449044428c80daa1bb9e5414c817db649dbf9cd78cb2831fc0acfcb1ac996` | توجيه API ومسارات Netlify. |
| `netlify/database/migrations/0001_core.sql` | 3,395 | `d81ac41451515a274712e27a3de72c8e1e6400ffbc625dbc0295565f82510b8d` | ترحيل PostgreSQL الأولي. |
| `netlify/functions/api.mjs` | 1,448 | `fa950a69ab73d554631629f740823af2e00cbf9cb3423bdc37b0172b5d76ec64` | مدخل Netlify Function. |
| `netlify/repository.mjs` | 10,509 | `e66197885e653515123c8445274e39940d2ec1cfc055fa97ace2b1be25cc05e5` | مستودع PostgreSQL وNetlify Blobs. |
| `netlify/tests/api.test.mjs` | 9,056 | `2de84be4ce415de2779aa3feabccac62d63fb8dcac446640b91a0877ec34309c` | اختبارات API/قاعدة Netlify محليًا. |
| `netlify/tests/build.test.mjs` | 974 | `af5d69ef5b0114eaab77a4e06052235d2fa006c761bb86fbc5afd2469cb1760b` | اختبار قائمة أصول dist وعدم تسريب الخادم. |
| `netlify/tests/helpers.mjs` | 3,040 | `1f71c40e1cd128f4657184dc0f9b0ec96bc039d19fcb5cda0e022948c7acb740` | مساعدات بيانات اختبار Netlify. |
| `package-lock.json` | 30,918 | `863a099c12092c9413810bdbada5d01915f15d6388e51a63cc8137a3917c8ef2` | قفل نسخ npm لتحقيق تثبيت قابل للتكرار. |
| `package.json` | 760 | `c80b87a192c13b40dd4a88ca9af82bbeff05f5ecb1150d80ca6e8c215a7a7ab4` | اعتماديات وأوامر المشروع. |
| `scientific-search.mjs` | 9,169 | `0bf86028e8ae28702de33b9dc9c28bbce76f67e02f24fc449061f650f151e420` | اتصال PubMed وEurope PMC وتطبيع المراجع. |
| `scripts/build-netlify.mjs` | 682 | `16ff1be34c5b7fe09fc74b9643e36d1f87b5d6364426d8a34a32b7e5cb8fdee4` | بناء dist من قائمة أصول عامة صريحة. |
| `security.test.mjs` | 14,182 | `3f17cd246046a4acd1a58651440428594540e118f1f8a7e5942405da43fb1b4b` | اختبارات أمن وتكامل المسار المحلي. |
| `server.mjs` | 33,957 | `b1f09c0be76f104cda88f3f04990edc8cb46ad512d15e416b36633d90ae2972a` | الخادم المحلي ومسارات API والأمان. |
| `styles.css` | 33,610 | `1ddbd4eb77565a9bf874ee5ec9aee04e4adacf7f486c98e93b59367e42f2f674` | تنسيقات الواجهة المتجاوبة وRTL/LTR. |
| `sw.js` | 1,664 | `33c51277a6aecf5a950ab0fd64d2fae34694955fc92bb809dc7a71544d167457` | عامل خدمة للأصول العامة دون API خاصة. |
