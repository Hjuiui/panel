<h1 align="center">نصب از طریق Cloudflare Workers</h1>

خب اول کد Worker رو دانلود کنید و ببرید توی داشبورد ورکر کلادفلر و فایل رو آپلود کنید.

 در نهایت ورکر رو `Save and Deploy` کنید.
حالا از اینجا به داشبورد ورکر برگردید و این مراحل را دنبال کنید:

از این قسمت وارد صفحه `KV` بشید:

> ![Screenshot (4)](https://private-user-images.githubusercontent.com/161088226/337188002-f840b806-6fe7-498a-bee1-0c750b016805.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTc2NjMyNTIsIm5iZiI6MTcxNzY2Mjk1MiwicGF0aCI6Ii8xNjEwODgyMjYvMzM3MTg4MDAyLWY4NDBiODA2LTZmZTctNDk4YS1iZWUxLTBjNzUwYjAxNjgwNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNjA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDYwNlQwODM1NTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02ZGY0Yjc5YTk4YTQ5YjlhZWMyMzJmNjNlNzdlMWNhM2JhZTAyZTI0ZjEyNDFmMzRjYTA5ZDQ4YjNjNDA3YTJlJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.d5uD2nlXt625Wm64_XWc30UAKdKzIv_W6h5v3kHHF28)

تو قسمت KV بزنید `Create a namespace` و یه اسم دلخواه وارد کنید مثلا Test و `Add` کنید.
> ![Screenshot (5)](https://private-user-images.githubusercontent.com/161088226/337189936-0f6af6fe-8520-494d-b13c-b9139625c839.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTc2NjM0MjAsIm5iZiI6MTcxNzY2MzEyMCwicGF0aCI6Ii8xNjEwODgyMjYvMzM3MTg5OTM2LTBmNmFmNmZlLTg1MjAtNDk0ZC1iMTNjLWI5MTM5NjI1YzgzOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNjA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDYwNlQwODM4NDBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iMGJhNGFhODBlODFkNDNlYTU2Nzg1Y2M1ZjVhYWY4OWU5YzRiMmFhMzI3MDIxNzg1NTc1ZTc4Y2E1YWE1ZWI4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.g-go4A4YJ4ANZVW0wTTp8KKO3DvufIFXRqjgsN7ArvE)

دوباره از منوی سمت چپ به قسمت `Workers & Pages` برید، ورکری که ساختید رو باز کنید، برید به قسمت `Settings` و `Variables` رو انتخاب کنید. یه کم بیاید پایین قسمت `KV Namespace Bindings` رو میبینید، روی `Add binding` بزنید و مطابق تصویر زیر از کشویی سمت راست اون KV که ساخته بودید انتخاب کنید (در مثال Test بود). چیزی که مهمه کشویی سمت چپه، حتما باید مقدارش رو بذارید `hosein` و `Save and Deploy` و تمام.

> ![Screenshot (3)](https://private-user-images.githubusercontent.com/161088226/337185674-2c91de2a-75a4-4f51-9678-1feb2a35ba62.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTc2NjI5NDksIm5iZiI6MTcxNzY2MjY0OSwicGF0aCI6Ii8xNjEwODgyMjYvMzM3MTg1Njc0LTJjOTFkZTJhLTc1YTQtNGY1MS05Njc4LTFmZWIyYTM1YmE2Mi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNjA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDYwNlQwODMwNDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iZThlNjIxZWU1YjJmYjRiNDI1MTA5YjVhOTU2ZTM0M2MwYjc3OGMwYjE4MDA1YjE5OGRjMmJmMGFjMjk2ZGYzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.FbTNOKOpq9ykkiNseJCuZWiZuqIr9siu8ZVwTMvR4-Y)

برای مثال، فرض کنید دامنه‌ی ورکر شما هست worker-polished-leaf-d022.workers.dev، یه `panel/` تهش اضافه کنید و وارد پنل بشید. مثال:

>`https://worker-polished-leaf-d022.workers.dev/panel`

اول میره به صفحه‌ی لاگین، پسورد پیشفرض یعنی `admin` رو وارد کنید و تمام.
نصب به پایان رسیده و توضیحاتی که در ادامه اومده شاید برای عموم لازم نباشه.

<br><br>
##  تنظیمات پیشرفته (اختیاری)
شاید تا الان متوجه شده باشید که در مورد تغییر UUID و Proxy IP چیزی نگفتیم چون میتونید از پیشفرض خود پنل استفاده کنید. اما برای تغییرشون میتونید مراحل زیر رو دنبال کنید، توصیه میشه حداقل UUID رو تغییر بدید. 

### 1- تغییر UUID
همونطور که میدونید UUID  مثل اسم رمزی میمونه که داخل لینک‌های اشتراک و کانفیگ ها قرار میگیره و شما در صورت نیاز میتونید تغییر بدید. در صورت تغییر این پارامتر اتصال کاربرهای شما قطع میشه  و لازم هست لینک اشتراک و یا کانفیگ ها رو مجددا در اختیارشون قرار بدید. در صورتی که این UUID رو در این مرحله تعریف نکنید هم کد از یک UUID پیشفرض استفاده خواهد کرد.

تو خط 9 یه UUID هست و میتونید تغییرش ندید ولی ترجیحا اینجوری عوضش کنید: از [اینجا](https://www.uuidgenerator.net/) (تو خط 9 کد هم هست) یه UUID بگیرید و کپی کنید تو خط 10 جای قبلی و تمام. ورکر رو Save and Deploy کنید.



### 2- ثابت کردن Proxy IP

ما یه مشکلی داریم که این کد به صورت پیشفرض از تعداد زیادی IP Proxy استفاده میکنه که برای هر بار اتصال به سایتای پشت کلادفلر ( شامل بخش وسیعی از وب میشه) به صورت رندوم IP جدیدی انتخاب میکنه و در نتیجه به صورت متناوب IP شما تغییر پیدا میکنه. این تغییر IP شاید برای برخی مشکل ساز باشه (مخصوصا تریدرها). برای تغییر Proxy IP از طریق خود پنل انجام بدید، به این ترتیب که اعمال میکنید و ساب رو آپدیت میکنید و تمام. اما توصیه میکنم از روشی که در ادامه توضیح دادم استفاده کنید چون:

> [!CAUTION]
> اگر از طریق پنل Proxy IP رو اعمال کنید و اون IP از کار بیافته، باید یه IP جایگزین کنید و ساب رو آپدیت کنید. معنیش اینه که اگر کانفیگ اهدا کرده باشید و Proxy IP رو تغییر بدید دیگه فایده‌ای نداره چون یوزر ساب نداره که کانفیگ رو آپدیت کنه. بنابراین توصیه میشه از این روش فقط برای مصرف شخصی استفاده کنید. اما خوبی روش دوم که در ادامه میگم اینه که از طریق داشبورد کلادفلر انجام میشه و نیازی به آپدیت کردن کانفیگ‌ها نداره.
<br>

این دو تا لینک رو باز کنید (داخل کد ورکر خط 12 و 13 هم گذاشتم) یه تعدادی IP نشون میده که میتونید کشورشون رو هم چک کنید و یه دونه انتخاب کنید.

>[Proxy IP](https://www.nslookup.io/domains/cdn.xn--b6gac.eu.org/dns-records/)

>[Proxy IP](https://www.nslookup.io/domains/cdn-all.xn--b6gac.eu.org/dns-records/)

<p align="center">
  <img src="assets/images/Proxy_ips.jpg">
</p>

متن اول خط 14 به این صورت است:

```javascript
const proxyIPs = ['cdn.xn--b6gac.eu.org', 'cdn-all.xn--b6gac.eu.org', 'edgetunnel.anycast.eu.org'];
```

بعد که خواستید IP رو بذارید این شکلی میشه:
```javascript
const proxyIPs = ['8.218.149.193'];
```

ورکر رو `Save and Deploy` کنید.
> [!WARNING]
> فقط حواستون باشه تعداد این IP ها زیاده و ممکنه تعداد زیادیشون از کار افتاده باشن. باید تست کنید تا یه خوبشو سوا کنید.

> [!CAUTION]
> اگر از تک IP استفاده کنید احتمالا بعد یه مدت دوباره از کار میافته و خیلی سایتا باز نمیشن. باید از اول این مراحلو برید.



 
