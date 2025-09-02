<p align="center">
  <a href="https://github.com/oXIIIo/marzban-template/" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
    </picture>
  </a>
</p>
<h1 align="center"/>تمپلیت‌های sing-box برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>


<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>


# مقدمه
لیستی از تمپلیت‌های شخصی سازی شده برای مرزبان

# لیست تمپلیت ها
- [تمپلیت برای sing-box](https://github.com/WhyMan1/marzban-template/tree/master/singbox)
- [تمپلیت برای v2ray](https://github.com/WhyMan1/marzban-template/tree/master/v2ray)
- [صفحه سابسکریپشن](https://github.com/WhyMan1/marzban-template/tree/master/subscription)
- [صفحه خانه](https://github.com/WhyMan1/marzban-template/tree/master/home)


# مراحل نصب
برای نصب هر تمپلیت به صفحه مربوط به آن مراجعه کنید

# نصب همه
برای نصب همه تمپلیت های موجود دستورات زیر را در ترمینال سرور خود اجرا کنید:
1. دانلود فایل های تمپلیت
```sh
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/singbox/default.json
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/index.html
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/home/index.html
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت ها فقط کافیست مرحله 1 را تکرار کنید.

# Contributors

<p align="center">
Thanks to the all contributors who have helped improve Sing-box template:
</p>
<p align="center">
<a href="https://github.com/WhyMan1/marzban-template/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=WhyMan1/marzban-template" />
</a>
</p>
<p align="center">
  Made with <a rel="noopener noreferrer" target="_blank" href="https://contrib.rocks">contrib.rocks</a>
</p>

# حمایت از من

<a href="https://nowpayments.io/donation?api_key=WE3KFT5-2VKMNSF-N1P4YQ6-24N82ZA&source=lk_donation&medium=referral" target="_blank">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>
