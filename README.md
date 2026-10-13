# نموذج بوابة معهد الدراسات القضائية والقانونية

نموذج تفاعلي بصفحات **HTML وCSS وJavaScript**. العربية هي اللغة الافتراضية مع دعم الإنجليزية واتجاهي RTL وLTR. التصميم مستلهم من https://services.housing.gov.bh/home باستخدام الأزرق الداكن والذهبي، وبطاقات خدمات بيضاء وخلفية فاتحة.

## التشغيل

فك ضغط جميع الملفات، ثم افتح `index.html` الموجود في المجلد الرئيسي بالنقر المزدوج. جميع الملفات في مجلد واحد بدون مجلدات فرعية. احتفظ بملفات JavaScript وCSS والخطوط وبقية صفحات HTML بجانب `index.html`. لا يحتاج النموذج إلى تثبيت حزم أو اتصال بالإنترنت. للحصول على حفظ متسق بين الصفحات، يفضّل تشغيل المجلد الرئيسي على خادم HTTP محلي (مثل `python -m http.server 8080`) ثم فتح `http://localhost:8080`.

## الرفع إلى GitHub Pages / Upload to GitHub Pages

فك ضغط الحزمة، ثم افتح المجلد وحدّد جميع الملفات بداخله وارفعها إلى جذر مستودع `jlsi` بجانب `index.html` الحالي. وافق على استبدال الملفات القديمة ثم اضغط Commit changes. لا ترفع ملف ZIP نفسه أو المجلد الخارجي. انتظر اكتمال نشر GitHub Pages ثم حدّث الصفحة باستخدام Ctrl + F5.

Extract the ZIP, open the extracted folder, and select ALL files inside it. Upload these files to the root of the `jlsi` repository, replacing existing files, then choose Commit changes. Do not upload the ZIP or the outer folder. Wait for GitHub Pages to deploy, then refresh with Ctrl + F5.

## تجربة المسار الرئيسي

1. من البرامج التدريبية أنشئ برنامجًا جديدًا بالعربية والإنجليزية.
2. افتح تفاصيل البرنامج ثم تبويب الاعتمادات، واعتمد المراحل حتى إتاحته للتسجيل.
3. قدّم ترشيحًا باستخدام بيانات وهمية ومعرّف مثل `DEMO-106`.
4. افتح الترشيحات والطلبات واعتمد الطلب؛ تُحدّث المقاعد المتاحة.
5. في الحضور، استخدم `DEMO-101` إلى `DEMO-105`، أو عدّل الحالة مع كتابة مبرر.
6. عدّل درجات العينة في صفحة الاختبارات. ثم راجع أهلية الشهادة واطبعها أو احفظها PDF.
7. أرسل تقييمًا وراجع مؤشرات التقارير، أو أضف مصروفًا وجرّب دورة اعتماده وصرفه.

## الصفحات

الرئيسية، لوحة المتابعة، البرامج، تفاصيل البرنامج، الترشيحات، الجدول، المدربون، الحضور، الاختبارات والدرجات، التقييمات، الشهادات، المالية، التقارير، الأرشيف الإعلامي، الإعدادات.

## حدود النموذج

- JavaScript هي لغة التفاعل في هذه النسخة؛ لا يتضمن النموذج خادمًا خلفيًا بلغة Java.
- جميع البيانات افتراضية. لا توجد حسابات حقيقية أو اتصال بالمفتاح الإلكتروني أو المعهد أو وزارة العدل أو الرسائل أو الدفع.
- اختيار الدور يغير التنقل لأغراض العرض، وليس نظام صلاحيات أو مصادقة.
- البيانات والمرفقات تبقى في `localStorage` بالمتصفح والجهاز الحاليين؛ لا توجد قاعدة بيانات أو مزامنة بين المستخدمين. المرفقات محدودة إلى 500 كيلوبايت للملف وتخضع لسعة المتصفح.
- سجل الحضور يعرض عينة مشتركة من خمسة متدربين. الدرجات والشهادات مرتبطة ببرنامج تجريبي مكتمل (`JLSI-024`)؛ الترشيحات الجديدة لا تنشئ تلقائيًا سجلات درجات في تلك العينة.
- معايير الشهادة تستخدم نسبة الحضور ومتوسط درجتي الاختبار والتكليف. يمكن تعديل حدود الاجتياز من الإعدادات.
- الشهادات مطبوعة بوسم تجريبي وليست وثائق رسمية.
- موافقات البرامج والصرف مبسطة للمراجعة. التكاملات والأمان ومسارات الرفض والاستثناءات الكاملة تحتاج تطويرًا في النظام الفعلي.

## Structure / English notes

Open `index.html` in the root folder after extracting the entire ZIP. All files are in one folder with no subfolders. Keep the JavaScript, CSS, fonts and all HTML pages beside `index.html`. This is a dependency-free, multipage HTML/CSS/JavaScript prototype. `app.js` provides bilingual rendering and local interactions; `data.js` contains fictional sample records. It is not a production system or a Java backend. Each HTML page can be served by any static web server. Data is browser-local and resettable from Settings. The bundled Tajawal font is licensed under the SIL Open Font License; see `FONT-LICENSE.txt`.
