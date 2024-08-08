<p align="center"> <img src="https://github.com/user-attachments/assets/09294b73-ecc9-40ea-a2bd-9062438f7605" /> </p>

<p align="center">
    مقدمه‌ای بر Postman
    <br/>
    تحقیق پایانی برنامه سازی وب، دانشگاه صنعتی شریف
    <br/>
    ارائه دهنده درس: جناب آقای یحیی پورسلطانی
    <br/>
    نویسندگان: محیا ضرابی‌زاده، زهرا تهامی
</p>

<div dir="rtl">

## مقدمه

پستمن ابزاری قدرتمند و چندکاره است که به توسعه‌دهندگان پلتفرمی جامع برای طراحی، آزمون، مستندسازی، و اشتراک‌گذاری موثر APIها ارائه می‌دهد. در این مقاله قصد داریم راهنمایی برای شروع کار با پستمن ارائه دهیم. در ابتدا محیط پستمن و قابلیت‌های آن را معرفی می‌کنیم و سپس با استفاده از یک مثال عملی جامع، با کارایی این ابزار بهتر آشنا می‌شویم.

## پستمن چیست؟

پستمن یک پلتفرم API است که امکان طراحی، ساخت، و آزمون API را به توسعه‌دهندگان می‌دهد. این ابزار تمام مراحل چرخه‌ی زندگی API را ساده‌سازی می‌کند و مسیر همکاری را هموارتر می‌سازد. در نتیجه‌ی این موضوع، تیم‌های یک مجموعه می‌توانند APIهای بهتری را به طریق ساده‌تر و سریع‌تری تولید کنند[6].

پستمن برای کاربران به راحتی اجازه‌ی ذخیره‌سازی، فهرست کردن، و همکاری حول تمام مصنوعات API، روی یکم پلتفرم مرکزی، را ایجاد می‌کند. پستمن می‌تواند مشخصات، مستندات، تست‌کیس‌ها و نتایج، و همه‌ی چیزهای دیگری که مربوط به API شما هستند را ذخیره و مدیریت کند[6]. 

## ویژگی‌های کلیدی پستمن

پستمن طیف گسترده‌ای از ویژگی‌ها را ارائه می‌دهد که جنبه‌های مختلف توسعه و آزمون API را پوشش می‌دهند. برخی از ویژگی‌های برجسته‌ی آن عبارت‌اند از:

* **ساخت درخواست HTTP:** پستمن به شما امکان ایجاد درخواست‌های HTTP با متودها، هدرها، پارامترها، و بدنه‌های درخواست متفاوت را می‌دهد. شما می‌توانید این درخواست‌ها را برای استفاده‌ی مجدد در آینده ‌خیر، یا آن‌ها را در مجموعه‌ها دسته‌بندی کنید.
* **نمایش پاسخ:** پستمن یک نمای جامع از پاسخ API، شامل کد وضعیت، هدرها، و بدنه پاسخ، ارائه می‌دهد. این ابزار از فرمت‌های مختلف داده مانند JSON، XML، و داده‌های فرم‌کدگذاری‌شده پشتیبانی می‌کند.
* **مدیریت محیط‌ها:** پستمن به شما اجازه می‌دهد محیط‌های متعددی را تعریف کنید که هر کدام متغیرهای مخصوص خود را دارند. این ویژگی به طور خاص برای جابه‌جایی بین محیط‌های توسعه، آزمایش، و تولید بدون نیاز به تغییر URL‌های درخواست یا هدرها مفید است.
* **مکانیزم‌های احراز هویت:** پستمن از روش‌های مختلف احراز هویت، از جمله کلیدهای API، OAuth 1.0a، OAuth 2.0 و احراز هویت پایه، پشتیبانی می‌کند. این ابزار فرآیند تنظیم و مدیریت احراز هویت برای درخواست‌های API شما را بسیار ساده‌تر می‌کند.
* **اسکریپت‌های تست:** پستمن به شما امکان می‌دهد با استفاده از جاوا اسکریپت برای اعتبارسنجی رفتار API‌های خود اسکریپت‌های آزمون بنویسید. این آزمون‌ها می‌توانند کدهای وضعیت پاسخ، هدرها، و محتوای بدنه را بررسی کنند و ثبات و قابلیت اطمینان بودن API شما را بسنجند.
* **پشتیبانی از کد جاوا اسکریپت:** اپلیکیشن پستمن از اجرای کدهای جاوا اسکریپت پشتیبانی می‌کند. این ویژگی به شما امکان انجام عملیات‌های داینامیک مانند تولید داده‌ی تصادفی، دستکاری پارامترهای درخواست، یا استخراج داده از پاسخ‌ها برای استفاده در درخواست‌های بعدی، را می‌دهد.
* **پشتیبانی از انواع فرمت‌های داده:**  پستمن با فرمت‌های مختلف داده مانند JSON، XML، فرم‌کدگذاری‌شده، و داده‌های باینری کار می‌کند. این ابزار برای پاسخ‌های JSON و XML، قابلیت syntax highlighting و automatic parsing فراهم می‌کند که کار با داده‌های API را آسان‌تر می‌سازد.
* **همکاری:** پستمن به شما فضاهای کاری تیمی ارائه می‌دهد، که به کاربران متعدد اجازه می‌دهد بر روی پروژه‌های API همکاری کنند. اعضای تیم می‌توانند مجموعه‌ها، محیط‌ها، و مجموعه‌های آزمون را به اشتراک بگذارند، که به ثبات و تسهیل همکاری کمک می‌کند.
* **مستندسازی API:** پستمن می‌تواند براساس درخواست‌ها و موارد آزمون تعریف‌شده در مجموعه‌های شما، به طور خودکار مستنداتی برای API‌هایتان تولید کند. این ویژگی در به‌روز و در دسترس نگه داشتن مستندات API کمک شایانی می‌کند.
* **نظارت:** پستمن دارای یک ویژگی نظارت است که به شما امکان برنامه‌ریزی چک‌هایی برای API‌هایتان می‌دهد. این چک‌ها می‌توانند در دسترس بودن، زمان پاسخ، و درستی API‌های شما را بررسی کنند و به شما در شناسایی و رفع مشکلات به صورت پیشگیرانه کمک کنند.


## شروع کار با پستمن

برای استفاده از پستمن، شما می‌توانید [اپلیکیشن پستمن]( https://www.postman.com/downloads/) را دانلود و نصب کنید، و یا از [نسخه‌ی وب پستمن]( https://www.postman.com/downloads/) استفاده کنید. توجه کنید که برای استفاده از نسخه‌ی وب و دسترسی کامل به همه‌ی قابلیت‌های اپلیکیشن، باید یک [حساب کاربری پستمن]( https://identity.getpostman.com/signup?continue=https%3A%2F%2Fgo.postman.co%2Fhome) ایجاد کنید[6].

پس از ورود، با میز کار پستمن رو به رو خواهید شد که مطابق تصویر زیر است: 

<img width="1552" alt="Screen Shot 2024-07-17 at 7 00 17 PM" src="https://github.com/user-attachments/assets/704dfbd8-00d4-4b4f-8874-63a355a0d52f">

در ادامه به اختصار با نحوه‌ی استفاده از قابلیت‌های اصلی پستمن آشنا خواهیم شد.

### ایجاد درخواست

با استفاده از پستمن می‌توان انواع درخواست‌ها را به APIهای متفاوت ارسال و پاسخ آ‌ن‌ها را بررسی کرد. 

مراحل ایجاد و ارسال یک درخواست:
1. ایجاد درخواست با کلیک بر روی دکمه "+" در نوار بالایی بخش اصلی میز کار.
2. تنطیم متد، آدرس، و در صورت لزوم، پارامترها، هدرها، و موارد دیگر مربوط به درخواست.
3. ارسال درخواست.
4. بررسی پاسخ در پنل پایین صفحه.

<img width="1552" alt="Screen Shot 2024-07-17 at 7 33 01 PM" src="https://github.com/user-attachments/assets/7093ff74-94a2-44c7-a45f-93dce30479d6">


### ایجاد مجموعه‌

مجموعه‌ها در پستمن به شما امکان سازمان‌دهی درخواست‌های API را می‌دهند[1]. این ویژگی به خصوص برای مدیریت APIهای پیچیده یا پروژه‌های متعدد بسیار مفید است.

مراحل ایجاد یک مجموعه و افزودن درخواست به آن:
1. کلیک کردن بر روی دکمه‌ی "Collections" در نوار کناری صفحه.
2. کلیک کردن بر روی دکمه‌ی "+" در بالای پنل کناری برای ایجاد یک موجوعه جدید.
3. کلیک کردن بر روی سه‌نقطه‌ی مقابل اسم مجموعه و انتخاب گزینه‌ی "Add request" برای ایجاد یک درخواست جدید در آن.

<img width="1552" alt="Screen Shot 2024-07-17 at 7 33 01 PM" src="https://github.com/user-attachments/assets/0de39549-ad29-4357-abef-1f47f215d623">

مجموعه‌ها علاوه بر ذخیره‌سازی و سازمان‌دهی درخواست‌های API، برای دخیره‌ی آزمون‌های API نیز به کار می‌روند. در واقع یک مجموعه، پوشه‌ی اصلی پروژه‌ی شماست و درخواست‌ها و آزمون‌ها را درون آن باید پوشه‌بندی و مرتب‌سازی کنید. رایج‌ترین روش برای سازمان‌دهی یک مجموعه، ایجاد یک پوشه به ازای هر اندپوینت، و ایجاد یک پوشه‌ی "Integration tests" برای قرار دادن آزمون‌های APIای که ارتباط بین اندپوینت‌های متفاوت را می‌آزمایند است[6].

### ایجاد محیط

محیط‌ها در پستمن مجموعه‌ای از متغیرها هستند که می‌توانیم در درخواست‌های متفاوت از آن‌ها استفاده کنیم[6].

مراحل ایجاد یک محیط و افزودن متغیر به آن:
1. کلیک کردن بر روی دکمه‌ی "Environments" در نوار کناری صفحه.
2. کلیک کردن بر روی دکمه‌ی "+" در بالای پنل کناری برای ایجاد یک محیط جدید.
3. ایجاد یک متغیر محیطی جدید با وارد کردن نام متغیر و مقدار آن در جدول.
4. ذخیره‌ی تغییرات اعمال‌شده.

 <img width="1552" alt="Screen Shot 2024-07-17 at 7 58 03 PM" src="https://github.com/user-attachments/assets/08420af7-6f82-4306-a521-b1a5f46ad0e6">

   
### نوشتن آزمون‌

پستمن به شما این امکان را می‌دهد که برای درخواست‌های API خود، آزمون‌هایی به زبان جاوااسکریپت بنویسید[1]. این آزمون‌ها می‌توانند داده‌های پاسخ را تأیید کنند، کدهای وضعیت را بررسی کنند، و یا سایر اعتبارسنجی‌ها را انجام دهند.

مراحل ایجاد آزمون برای یک درخواست:
1. انتخاب یک درخواست از پنل کناری.
2. کلیک کردن بر روی تب "Scripts".
3. وارد کردن کد تست در قسمت "Post-response".
4. بررسی تب "Test Results" در بخش پاسخ برای دیدن نتایج آزمون.

<img width="1552" alt="Screen Shot 2024-07-17 at 8 19 20 PM" src="https://github.com/user-attachments/assets/397e7550-4594-4f50-849b-61dc34bdf374">


### مستندسازی

پستمن می‌تواند به طور خودکار و بر اساس مجموعه‌های شما، مستنداتی برای APIتان تولید کند[1]. این ویژگی در به‌‌روز نگه داشتن مستندات API و دسترسی‌پذیری آسان‌تر آن‌ها کمک شایانی می‌کند.

مراحل دسترسی به مستندات:
1. کلیک کردن بر روی سه‌نقطه‌ی مقابل اسم مجموعه در پنل کناری و انتخاب گزینه‌ی "View documentation".
2. اعمال تغییرات لازم در توضیحات مربوط به مجموعه و درخواست‌ها.
3. در صورت لزوم، اشتراک‌گذاری با استفاده از دکمه‌ی "Publish" در گوشه‌ی بالا سمت راست صفحه. 

<img width="1552" alt="Screen Shot 2024-07-17 at 8 25 50 PM" src="https://github.com/user-attachments/assets/4721e3ad-4951-4583-ab10-afc84b10feae">


## مثال‌های عملی از کاربرد پستمن

در این بخش با استفاده از [Swagger Petstore API](https://petstore.swagger.io/#/)، که یک سرور نمونه‌ی فروشگاه حیوانات خانگی است، مجموعه مثال‌های عملی‌ای برای شرح کامل‌تر کاربرد پستمن می‌آوریم[6].

با ساخت یک مجموعه شروع می‌کنیم. مطابق توصیحات داده شده، مجموعه‌ای به نام "Petstore" می‌سازیم و به ازای هر یک از سه اندپوینت Petstore API، یک پوشه برای دسته‌بندی درخواست‌های مربوط به آن ایجاد می‌کنیم.

<img width="1552" alt="Screen Shot 2024-07-17 at 9 43 24 PM" src="https://github.com/user-attachments/assets/62d013c9-d995-45c1-a85b-3cc44197234e">

براساس داکیومنتیشن این API، می‌دانیم که url پایه‌ی همه‌ی درخواست‌ها یکسان و برابر `https://petstore.swagger.io/v2` است. بنابراین یک محیط نیز ایجاد می‌کنیم تا در آن یک متغیر `base_url` تعریف‌ کنیم و مقدار آن را برابر url داده‌شده قرار دهیم.

<img width="1552" alt="Screen Shot 2024-07-17 at 9 36 35 PM" src="https://github.com/user-attachments/assets/1f4a798a-1ca6-4165-8185-450de9e39c7c">

در ادامه می‌خواهیم درخواست‌هایی با متدهای مختلف ارسال و تست کنیم.

 ### ارسال یک درخواست با متد GET

اولین درخواست را می‌خواهیم به اندپوینت `pet/findByStatus/` ارسال کنیم. این درخواست یک پارامتر `status` دریافت می‌کند که مقدار آن می‌تواند یکی از مقادیر `available/pending/sold‍` باشد.

برای ارسال این درخواست،‌ مراحل زیر را دنبال می‌کنیم:
1. از نوار بالایی صفحه، محیط "Petstore" را انتخاب می‌کنیم.
2. داخل پوشه‌ی "pet"، یک درخواست به نام "find pet by status" ایحاد می‌کنیم.
3. متد درخواست را برابر `GET`، و url درخواست را برابر مقدار زیر قرار می‌دهیم:
   
<div dir="ltr">
<pre>
    {{base_url}}/pet/findByStatus
</pre>
</div>

4. در تب "Params"، پارامتر `status` با مقدار `available` را تعریف می‌کنیم. مشاهده خواهیم کرد که این پارامتر به صورت خودکار به url افزوده می‌شود.
5. دکمه‌ی "Send" را می‌زنیم.

<img width="1552" alt="Screen Shot 2024-07-17 at 9 57 56 PM" src="https://github.com/user-attachments/assets/f9e93238-3311-48d4-a029-8440d9239dc2">

 پاسخ درخواست در پنل پایین صفحه، مشابه پاسخ زیر خواهد بود:
 
<div dir="ltr">
<pre>
    [  
    {  
        "id": 493751,  
        "category": {  
            "id": 1,  
            "name": "Dogs"  
        },  
        "name": "Lucy",  
        "photoUrls": [],   
        "tags": [  
            {  
                "id": 1,  
                "name": "test"  
            }  
        ],  
        "status": "available"  
    },  
    ...  
    ]
</pre>
</div>

در مرحله‌ی بعد، می‌خواهیم یک آزمون ساده برای این درخواست اضافه کنیم. مطابق توصیحات داده‌شده، وارد تب "Scripts" و بخش "Post-response" می‌شویم. در سمت راست این بخش، یک دکمه‌ی ">" شکل وجود دارد که در آن، قطعه‌کدهای آزمون آماده موجود هستند. با جست‌وجو در این بخش، می‌توانیم قطعه کدهای مربوط به آزمون کد وضعیت و مقدار بدنه‌ی پاسخ را تحت عناوین “Status code: Code is 200” و “Response body: JSON value check” بیابیم. این قطعه‌کدها را انتخاب می‌کنیم و قطعه‌کد دوم را به صورت زیر ادیت می‌کنیم تا وجود حیوان‌خانگی‌ای به نام "doggie" را تایید کند:

<div dir="ltr">
<pre>
    pm.test("First pet check name", function () {
        var jsonData = pm.response.json();
        pm.expect(jsonData[0].name).to.eql("doggie");
    });
</pre>
</div>

با ارسال دوباره‌ی درخواست، در تب "Test Results" در بخش پاسخ می‌توانیم نتیجه‌ی آزمون را ببینیم. 

<img width="1552" alt="Screen Shot 2024-07-17 at 10 07 16 PM" src="https://github.com/user-attachments/assets/d74b3b94-fec7-4c21-ab2a-bec5aca2fe7c">

نتیجه‌ی آزمون دوم ممکن است در زمان‌هایی FAIL شود، زیرا موجود بودن حیوانی با این نام همواره تضمین‌شده نیست.


### ارسال یک درخواست با متد POST

درخواست بعد را می‌خواهیم به اندپوینت `pet/` ارسال کنیم که برای ایجاد حیوان‌خانگی جدید به کار می‌رود. این درخواست مانند همه‌ی درخواست‌های POST، باید همراه یک بدنه با فرمت زیر ارسال شود:

<div dir="ltr">
<pre>
{
  "id": 0,
  "category": {
    "id": 0,
    "name": "string"
  },
  "name": "doggie",
  "photoUrls": [
    "string"
  ],
  "tags": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "status": "available"
}
</pre>
</div>

برای ارسال این درخواست،‌ مراحل زیر را دنبال می‌کنیم:
1. داخل پوشه‌ی "pet"، یک درخواست به نام "create pet" ایحاد می‌کنیم.
2. متد درخواست را برابر `POST`، و url درخواست را برابر مقدار زیر قرار می‌دهیم:
<div dir="ltr">
<pre>
    {{base_url}}/pet
</pre>
</div>

3. در تب "Body"، گزینه‌ی "raw" را انتخاب می‌کنیم و قطعه کدی مانند قطعه کد بالا در بخش بدنه وارد می‌کنیم.
4. دکمه‌ی "Send" را می‌زنیم.
   
<img width="1552" alt="Screen Shot 2024-07-17 at 10 38 05 PM" src="https://github.com/user-attachments/assets/4daf3707-3935-49c1-b439-43c63c063417">

برای تست این درخواست، مجددا می‌توانیم کد وضعیت و صحت پاسخ آن را با قطعه‌ کد‌های زیر بررسی کنیم:
<div dir="ltr">
<pre>
    pm.test("Status code is 200", function () {
        pm.response.to.have.status(200);
    });
    pm.test("New pet response check", function () {
       var jsonData = pm.response.json();
       pm.expect(jsonData.name).to.eql("doggie");
    });    
</pre>
</div>

<img width="1552" alt="Screen Shot 2024-07-18 at 1 35 19 AM" src="https://github.com/user-attachments/assets/14e952ed-c5b4-451c-9f18-c824a7227bac">

### ارسال یک درخواست با متد PUT

می‌توانیم در اندپوینت `pet/` با متد PUT، اطلاعات مربوط به یک حیوان‌خانگی را تغییر دهیم. این درخواست هم یک بدنه مانند بدنه‌ی درخواست قبل دریافت می‌کند. 

برای مشخص کردن حیوان‌خانگی مدنظر، از آی‌دی آن استفاده می‌کنیم. یک روش برای دریافت یک آی‌دی معتبر، ذخیره‌ی آی‌دی حیوان‌خانگی ایجاد شده در مرحله‌ی قبل است. برای این کار مراحل زیر را دنبال می‌کنیم:
1. درخواست قبل را باز می‌کنیم و به تب "Scripts" آن می‌رویم.
2. از قطعه‌کد‌های پیش‌فرض، کد با عنوان “Set a collection variable” را انتخاب می‌کنیم و مطابق کد زیر آن را تغییر می‌دهیم:
<div dir="ltr">
<pre>
    pm.collectionVariables.set("pet_id", pm.response.json().id);
</pre>
</div>
درخواست را دوباره ارسال می‌کنیم تا این بار نتیحه‌ی آن ذخیره شود.

حال می‌توانیم درخواست PUT را با استفاده از متغیر `{{pet_id}}` ارسال کنیم:
1. داخل پوشه‌ی "pet"، یک درخواست به نام "update pet" ایحاد می‌کنیم.
2. متد درخواست را برابر `PUT`، و url درخواست را برابر مقدار زیر قرار می‌دهیم:
   
<div dir="ltr">
<pre>
    {{base_url}}/pet
</pre>
</div>

3. در تب "Body"، گزینه‌ی "raw" را انتخاب می‌کنیم و قطعه کدی مانند قطعه کد زیر در بخش بدنه وارد می‌کنیم:

<div dir="ltr">
<pre>
    {
    "id": {{petId}},
    "name": "lucy",
    "status": "sold"
    }
</pre>
</div>

4. دکمه‌ی "Send" را می‌زنیم.

<img width="1552" alt="Screen Shot 2024-07-17 at 10 55 32 PM" src="https://github.com/user-attachments/assets/a7b6fd87-2aaa-4eec-8e7e-04ba73b2195a">

### ارسال یک درخواست با متد DELETE

آخرین درخواست را با متد DELETE به اندپوینت `{petID}/pet/` ارسال می‌کنیم. این درخواست یک پارامتر اجباری `petId` دربافت می‌کند. برای این درخواست هم از آی‌دی ذخیره‌شده‌ی خودمان استفاده می‌کنیم و درخواست را این گونه پیکربندی می‌کنیم:
1. داخل پوشه‌ی "pet"، یک درخواست به نام "delete pet" ایحاد می‌کنیم.
2. متد درخواست را برابر `DELETE`، و url درخواست را برابر مقدار زیر قرار می‌دهیم:
<div dir="ltr">
<pre>
    {{base_url}}/pet/{{pet_id}}
</pre>
</div>

  برای تست کردن پاک شدن حیوان‌خانگی با استفاده از این درخواست، می‌توانیم از درخواست GET اندپوینت `{petID}/pet/` استفاده کنیم که باید به ما کد وضعیت 404 برگرداند. برای تعریف این آزمون مراحل زیر را دنبال می‌کنیم:
1. به تب "Scripts" درخواست می‌رویم.
2. قطعه‌کد‌ پیش‌فرض “Send a request” را انتخاب می‌کنیم و مطابق کد زیر آن را تغییر می‌دهیم:
<div dir="ltr">
```
pm.sendRequest(pm.variables.get("baseUrl")+"/pet/" + pm.variables.get("petId"), function (err, response) {
   pm.test('Get pet data after deletion', function() {
       pm.expect(response.code).to.eql(404)
   });
});
```
</div>

با ارسال درخواست، مشاهده می‌کنیم که نتیجه‌ی تست PASS می‌شود.

<img width="1552" alt="Screen Shot 2024-07-17 at 11 11 28 PM" src="https://github.com/user-attachments/assets/6c2de9a9-ffe7-448d-839b-4902c2b20d05">


## خودکارسازی جریان‌های کاری با نیومن

نیومن همراه خط فرمان پستمن است که به شما اجازه می‌دهد مجموعه‌های خود را از خط فرمان اجرا و آزمون کنید[1]. این ویژگی به خصوص برای ادغام آزمون‌های پستمن در خط لوله CI/CD مفید است.

مراحل اجرای یک مجموعه‌ با استفاده از نیومن:
1. نصب Node.js.
2. نصب نیومن از طریق دستور زیر:
<div dir="ltr">

```
npm install -g newman
```

</div>
3. کلیک راست بر روی مجموعه‌ی موردنظر در پستمن و انتخاب گزینه‌ی "Export".
4. باز کردن ترمینال در دایرکتوری‌ای که مجموعه‌ی اکسپورت‌شده‌ در آن قرار دارد.
5. اجرای دستور زیر (با جایگزینی `YourCollection.json` با نام مجموعه‌):

<div dir="ltr">

```
newman run YourCollection.json
```

</div>

## همکاری با فضاهای کاری تیمی

پستمن فضاهای کاری تیمی را برای همکاری در پروژه‌های API فراهم می‌کند[1]. با استفاده از این قابلیت، اعضای تیم می‌توانند مجموعه‌ها، محیط‌ها، و منابع دیگر را با هم در پروژه‌های تیمی به اشتراک بگذارند.

مراحل ایجاد یک تیم:
1. کلیک کردن بر روی عکس پروفایل در هدر اصلی و انتخاب گزینه‌ی "Settings" برای ورود به تنظیمات پروفایل.
2. کلیک کردن بر روی تب "Teams".
3. کلیک کردن بر روی دکمه‌ی "Create Team" و وارد کردن اطلاعات و افراد.

مراحل ایجاد یک میز کار تیمی:
1. کلیک کردن بر روی دکمه "Workspaces" در هدر اصلی و انتخاب گزینه‌ی "Create Workspace".
2. نام‌گذاری فضای کاری و انتخاب دسترسی تیمی برای تیم موردنظر.
3. ایجاد و یا انتقال مجموعه‌ها و محیط‌های لازم به این فضای کاری.


## نتیجه‌گیری

پستمن ابزاری ارزشمند برای توسعه و آزمون API  است. این ابزار می‌تواند فرآیند توسعه‌ی API شما را بهبود ببخشد و همکاری درون‌تیمی را آسان‌تر کند. در این مقاله، پستمن و ویژگی‌های آن را معرفی کردیم. سپس با قابلیت‌های اصلی آن، از جمله ارسال درخواست‌ها، سازمان‌دهی مجموعه‌ها، استفاده از متغیرهای محیطی، نوشتن آزمون‌ها، و تولید مستندات آشنا شدیم. در ادامه با یک مثال عملی، این قابلیت‌ها را به کار گرفتیم. در نهایت نیومن و روش خودکارسازی جریان‌های کاری با آن را معرفی کردیم و مراحل آماده‌سازی فضای کاری تیمی برای همکاری در پروژه‌های API را شرح دادیم.


## مراجع

[1] https://learning.postman.com/docs/introduction/overview/

[2] https://www.coursehero.com/file/37994877/Postman-Essaydocx/

[3] https://www.tutorialspoint.com/postman/postman_introduction.html/

[4] https://www.coursehero.com/file/66153937/Essay-4-Postman-Epilogue2docx/

[5] https://learning.postman.com/docs/getting-started/basics/postman-basics/

[6] https://www.testdevlab.com/blog/using-postman-for-api-testing/