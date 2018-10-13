---
title: Divide and Conquer Algorithms
localeTitle: خوارزمية تقسيم و قهر
---
## خوارزمية تقسيم و قهر

تقسيم وقهر (المقدمة) مثل Greedy و Dynamic Programming ، يعتبر Divide و Conquer نموذجًا خوارزميًا. تحل خوارزمية Divide و Conquer النموذجية مشكلة باستخدام الخطوات الثلاث التالية.

1.  القسمة: كسر المشكلة المعطاة إلى مشاكل فرعية من نفس النوع.
2.  قهر: حل متكرر هذه المشاكل الفرعية
3.  الجمع بين: الجمع بين الإجابات بشكل مناسب

فيما يلي بعض الخوارزميات القياسية التي هي خوارزميات Divide و Conquer.

1) البحث الثنائي عبارة عن خوارزمية بحث. في كل خطوة ، تقارن الخوارزمية عنصر الإدخال x مع قيمة العنصر الأوسط في الصفيف. إذا تطابقت القيم ، فأرجع فهرس الوسط. وبخلاف ذلك ، إذا كانت x أقل من العنصر الأوسط ، فستتكرر الخوارزمية إلى الجانب الأيسر من العنصر الأوسط ، ثم تتكرر للجانب الأيمن من العنصر الأوسط.

2) Quicksort هو خوارزمية الفرز. تختار الخوارزمية عنصرًا محوريًا ، وتعيد ترتيب عناصر الصفيف بحيث تنتقل جميع العناصر الأصغر من العنصر المحوري المختار إلى الجانب الأيسر من المحور ، وتتحرك جميع العناصر الأكبر إلى الجانب الأيمن. وأخيرًا ، تقوم الخوارزمية بشكل متكرر بفرز subarrays على يمين ويسار العنصر المحوري.

3) دمج التصنيف هو أيضا خوارزمية الفرز. تقسم الخوارزمية المصفوفة إلى نصفين ، وتقوم بترتيبها بشكل متكرر ، ثم تقوم في النهاية بدمج النصفين اللذين تم فرزهما.

4) أقرب نقطة من النقاط المشكلة هي العثور على أقرب زوج من النقاط في مجموعة من النقاط في طائرة س ص. يمكن حل المشكلة في زمن O (n ^ 2) من خلال حساب المسافات لكل زوج من النقاط ومقارنة المسافات للعثور على الحد الأدنى. خوارزمية Divide و Conquer يحل المشكلة في وقت O (nLogn).

5) خوارزمية ستراسن هي خوارزمية فعالة لضرب المصفوفتين. هناك طريقة بسيطة لمضاعفة المصفوفتين تحتاج إلى 3 حلقات متداخلة وهي O (n ^ 3). تضاعف خوارزمية ستراسن مصفوفتين في زمن O (n ^ 2.8974).

6) خوارزمية تحويل Cooley – Tukey Fast Fourier Transform (FFT) هي أكثر الخوارزميات شيوعاً بالنسبة لـ FFT. هو عبارة عن خوارزمية divide و conquer التي تعمل في زمن O (nlogn).

7) كانت خوارزمية Karatsuba أول خوارزمية الضرب أسرع بشكل تقريبي من خوارزمية "المدرسة الصفية" التربيعية. يقلل من مضاعفة رقمين n-digit على الأكثر إلى n ^ 1.585 (وهو تقريب لسجل 3 في الأساس 2) من رقم واحد. وبالتالي فهو أسرع من الخوارزمية الكلاسيكية ، والتي تتطلب n ^ 2 منتجات من رقم واحد.

### Divide and Conquer (D & C) vs Dynamic Programming (DP)

يقسم النموذجان (D & C و DP) المشكلة المطروحة إلى مشاكل فرعية ويحلان المشكلات الفرعية. كيفية اختيار واحد منهم لمشكلة معينة؟ يجب استخدام Divide و Conquer عندما لا يتم تقييم المشاكل الثانوية نفسها عدة مرات. خلاف ذلك يجب استخدام البرمجة الديناميكية أو Memoization.

على سبيل المثال ، البحث الثنائي عبارة عن خوارزمية Divide و Conquer ، لم نقم أبدًا بتقييم نفس المشاكل الفرعية مرة أخرى. من ناحية أخرى ، من أجل حساب رقم فيبوناتشي nt ، ينبغي تفضيل البرمجة الديناميكية.