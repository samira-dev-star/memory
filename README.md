# Make Connections

This is a project that everyone can comment and find other people that have similar interests or they can share a memory which is coming from deja vu and find other people that have the same feeling or experience the same in another or same time.

There may be some social media networks like whats up telegram or Instagram that user can interact with each other by liking each other post sending each other messages but only people can make connection with each other without career knowledge about each other's interests or it is sometimes very difficult to find a subject between two people to discuss about before have a good deal of knowledge about each other. There are some people in the world that feel very lonely and have a very rare type of interest or personality which leads other people to not understand them or comprehend them and their aspirations very clearly as a type of personality and they cannot cope in society with other people easily because it is very difficult for them to find people with the same interest or the same experience because that experience may seem very odd in perspective of others.

There are many social applications that pair people with each other but usually people do not present their true selves in them sometimes people want to play with each other on a much more deep level especially very rare personality I want people to comprehend them or perceive their perspective as they want to be matched with another person with the same experience. What this website intends to do is to connect people on double level further so that they are not gonna start everything from bscratch. 

In other social network applications people many just show off or heat on other people or just make connection on a basic level but in this web application people get to know with each others cheapest secrets and feelings and experiences and that is why I decided to make this website.

This website is a part that the users can write their comments in it and the other people can see the comments and the comments are saved may seem very odd in perspective of others in the database and the comments are displayed in the website.


# creating my virtual environment:
py -3.12 -m venv env

# start my django project:
django-admin startproject memory

# which applications do we need in this project:
1. main application 
- in the main application we need to show some of the comments
- write a brief and interesting description of what is the purpose of this website
- we need to create a part for the user that leads them to create a user panel for themselves if they want to write their memory or comments and share it with others
- this application needs the part for the users to write their ideas about this website and also a part to show the top comments about the website and show to show their experience in this website
- ** optional** 

2. comment application
- in the comment application we need to show the comments that are saved in the database for example we can show them 10 comments per page. Or by adding a show more link when the user click on show more they can't see more comments.
- we need a part for the user to write their comments and enter for sending it.

3. ( this application is optional)MBTI test application:
- in this application we can design a test for the users to decide about their MBTI type

4. Accounting application:
- this accounting application has all the details and information regarding the user that is signed in.
- the best matches for the current user who are similar to this user either with a specific memory or MBTI type or personality should be shown here to the user. New matches can be shown based on the recent matches at the top of the accounting page and also the list of all the matches for the person wether through memory matches or with personality type matches can be recorded and saved in their panel separately.


5. Chatting application:
- we should make able users through this application to initiate a chat with other people that they are matched together and also optionally we can make them able create group chat for themselves in the website and chat at the same time with each other.


# ----------------------------------------------------

پروژه‌ای که توصیف کردی—یک شبکه اجتماعی عمیق برای اتصال افراد بر اساس خاطرات، تجربه‌های خاص، و تیپ‌های شخصیتی—خیلی خاص و خلاقانه‌ست. برای ساخت چنین پروژه‌ای با Django، به مجموعه‌ای از زبان‌ها، ابزارها، کتابخانه‌ها و مهارت‌ها نیاز داری. اینجا یک راهنمای کامل برات آوردم:

---

## 🧠 زبان‌ها و تکنولوژی‌های مورد نیاز

### 1. **زبان‌های برنامه‌نویسی**
- **Python**: زبان اصلی برای توسعه بک‌اند با Django
- **HTML/CSS**: برای طراحی صفحات وب
- **JavaScript**: برای تعاملات پویا در فرانت‌اند (مثل دکمه "نمایش بیشتر")
- **SQL**: برای کار با پایگاه داده‌ها (مثل PostgreSQL یا SQLite)

---

## 🧰 ابزارها و کتابخانه‌ها

| ابزار/کتابخانه | کاربرد |
|----------------|--------|
| **Django** | فریم‌ورک اصلی برای ساخت اپلیکیشن وب |
| **Django REST Framework** | برای ساخت APIها (مثلاً برای چت یا تست MBTI) |
| **Bootstrap یا Tailwind CSS** | برای طراحی رابط کاربری زیبا و واکنش‌گرا |
| **Celery + Redis** | برای مدیریت وظایف پس‌زمینه (مثل ارسال ایمیل یا نوتیفیکیشن) |
| **Channels** | برای پیاده‌سازی چت بلادرنگ با WebSocket |
| **PostgreSQL** | پایگاه داده قدرتمند برای ذخیره اطلاعات کاربران و کامنت‌ها |
| **pytest یا unittest** | برای تست کردن کدها |
| **Docker (اختیاری)** | برای مدیریت محیط توسعه و استقرار راحت‌تر |
| **Git + GitHub** | برای کنترل نسخه و همکاری تیمی |

---

## 🧩 ساختار پیشنهادی اپلیکیشن‌ها

### 1. **main app**
- صفحه اصلی با توضیح هدف سایت
- نمایش کامنت‌های برتر
- فرم ارسال ایده درباره سایت

### 2. **comment app**
- مدل کامنت با فیلدهایی مثل متن، زمان، نویسنده
- صفحه نمایش کامنت‌ها با قابلیت "نمایش بیشتر"
- فرم ارسال کامنت

### 3. **MBTI app (اختیاری)**
- فرم تست MBTI
- ذخیره نتیجه در پروفایل کاربر
- استفاده از نتیجه برای پیشنهاد دوستان مشابه

### 4. **accounting app**
- پروفایل کاربر
- نمایش تطابق‌های شخصیتی یا خاطره‌ای
- لیست تطابق‌های ذخیره‌شده

### 5. **chat app**
- چت بلادرنگ با WebSocket
- قابلیت ساخت گروه چت
- نمایش تاریخچه گفتگوها

---

## 🔐 امنیت و احراز هویت

- استفاده از **Django Auth** برای ثبت‌نام و ورود
- امکان ورود با گوگل یا شبکه‌های اجتماعی (با استفاده از `django-allauth`)
- رمزنگاری اطلاعات حساس
- محافظت از فرم‌ها با CSRF

---

## 🌐 تجربه کاربری و طراحی

- طراحی ساده و احساسی برای جذب کاربران خاص
- امکان فیلتر کردن کامنت‌ها بر اساس موضوع یا احساس
- استفاده از انیمیشن‌های سبک برای تعامل بهتر

---

اگر بخوای شروع کنی، پیشنهاد می‌کنم اول روی اپلیکیشن‌های اصلی تمرکز کنی (main + comment + accounting) و بعد به مرور MBTI و chat رو اضافه کنی. دوست داری برات یک نقشه راه مرحله‌به‌مرحله هم بنویسم؟