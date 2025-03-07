<p align="center">
  <a href="https://github.com/oXIIIo/marzban-template/" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
    </picture>
  </a>
</p>
<h1 align="center"/>Sing-box Templates for the <a href="https://github.com/Gozargah/Marzban">Marzban</a> Panel</h1>

<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

# Introduction
A list of customized templates for Marzban.

# Template List
- [Template for Sing-box](https://github.com/WhyMan1/marzban-template/tree/master/singbox)
- [Subscription Page](https://github.com/WhyMan1/marzban-template/tree/master/subscription)
- [Home Page](https://github.com/WhyMan1/marzban-template/tree/master/home)

# Installation Steps
To install each template, visit its respective page.

# Install All
To install all available templates, run the following commands in your server terminal:
1. Download template files:
```sh
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/singbox/default.json
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/index.html
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/home/index.html
```
2. Run the following commands in your server terminal:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"' | sudo tee -a /opt/marzban/.env
```
Alternatively, add the following values to the .env file located in the /opt/marzban directory:
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"
```

3. Restart Marzban:
```sh
marzban restart
```

## Updating
To update the templates, simply repeat step 1.

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

# Support

<a href="https://nowpayments.io/donation?api_key=WE3KFT5-2VKMNSF-N1P4YQ6-24N82ZA&source=lk_donation&medium=referral" target="_blank">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>
