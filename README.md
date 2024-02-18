# python_db_shop_tk

1 
پروژه پايگاه داده 
 ١٤٠٠/١٠/٢٣
گردآورنده : علي زاهدي سهروفروزانی
نگاه كلي 
.١ زبان نوشته شده 
پروژه ذكر شده با زبان پايتون ورژن ٣.١٠ نوشته شده است 
.٢ كتابخانه هاي استفاده شده
در اين برنامه از كتابخانه هاي داخلي Tkinter و 3sqlite استفاده شده است 
تذكر : در صورتي كتابخانه هاي فوق موجود نبود با دستور 3sqlite install pip و tkinter install pip مي تواند آن هارا به سيستم اضافه نماييد 
.٣ شيوه اجراي برنامه 
با هدايت به پوشه نرم افزار ميتوانيد سورسو برنامه را با استفاده از مفسر پايتون اجرا نماييد
.٤ نام پايگاه داده 
پايگاه داده استفاده شده در اين پروژه db.SHOP نام دارد 
.٥ جداول پايگاه داده 
جداول در نظرگرفته شده براي پايگاه داده شامل : 
.١ مسئول صندوق (cashier(
.٢ مسئول چيدن قفسه ها (shelfer(
.٣ مشتري (customer(
.٤ آيتم ها (item(
.٥ رئيس (boss(
.٦ سابقه خريد (buy_history(
.٧ سابقه واريز حقوق (salary_history(
2 
.٦ اجزاي جداول 
cashier:
 1. id integer primary key 
 2. name text 
 3. shift text 
shelfer:
 1. id integer primary key 
 2. name text 
 4. shift text 
boss:
 1. id integer primary key 
 2. name text 
customer:
 1. id integer primary key 
 2. name text 
 3. address text 
 4. phone text 
item:
 1. id integer primary key 
 2. name text 
 3. price integer 
history_buy:
 1. id integer primary key 
 2. date integer 
 3. buyer integer foreign key(id customer)
 4. item integer foreign key(id item)
history_salary:
 1. id integer primary key 
 2. boss integer foreign key(id boss)
 3. salary integer 
 4. date integer 
