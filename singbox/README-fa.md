<p align="center">
  <a href="https://github.com/WhyMan1/marzban-singbox-template/tree/master/singbox" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://sing-box.sagernet.org/assets/icon.svg">
      <img width="160" height="160" src="https://sing-box.sagernet.org/assets/icon.svg">
    </picture>
  </a>
</p>
<h1 align="center"/>sing-box config example for <a href="https://github.com/Gozargah/Marzban">Marzban</a></h1>

<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

## فهرست مطالب
- [مقدمه](#مقدمه)
- [ویژگی‌ ها](#ویژگی-ها)
- [مراحل نصب](#مراحل-نصب)
- [لینک دانلود sing-box](#لینک-دانلود-sing-box)

# مقدمه
سینگ باکس یک پروکسی مبتنی بر قوانین است که به شما این امکان را می‌دهد که تنظیمات مربوط به برنامه از قبیل DNS و مسیریابی و ... را از سمت سرور انجام دهید. در این template از سمت سرور، سینگ باکس  را به گونه‌ای تنظیم شده است که اتصال به سایت‌های ایرانی به صورت مستقیم انجام شود.
از مهم ترین ویژگی کلاینت sing-box پشتیبانی از پلتفرم های مختلف مانند اندروید، iOS، macOS و ... می باشد.

# ویژگی ها
- وصل شدن به سریع ترین کانفیگ
- وصل شدن مستقیم به وب‌سایت‌های ایرانی هنگامی که فیلترشکن روشن است
- بلاک کردن تبلیغات
و ...

# مراحل نصب
1. دانلود فایل template
```sh
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/singbox/default.json
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"' | sudo tee -a /opt/marzban/.env
```
یا از این طریق فایل را ادیت کرده و اضافه کنید
```sh
sudo nano /opt/marzban/.env
```
و مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت فقط کافیست مرحله ۱ را تکرار کنید.

# حمایت از من

<a href="https://nowpayments.io/donation?api_key=WE3KFT5-2VKMNSF-N1P4YQ6-24N82ZA&source=lk_donation&medium=referral" target="_blank">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>