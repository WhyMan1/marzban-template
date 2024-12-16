<p align="center">
  <a href="https://github.com/WhyMan1/marzban-singbox-template/tree/master/singbox" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://sing-box.sagernet.org/assets/icon.svg">
      <img width="160" height="160" src="https://sing-box.sagernet.org/assets/icon.svg">
    </picture>
  </a>
</p>
<h1 align="center"/>Sing-box Config Example for <a href="https://github.com/Gozargah/Marzban">Marzban</a></h1>

<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation Steps](#installation-steps)
- [Sing-box Download Link](#sing-box-download-link)

# Introduction
Sing-box is a rule-based proxy that allows you to configure program settings such as DNS, routing, and more from the server side. In this template, Sing-box is configured server-side to establish direct connections to local (internal) websites.  
One of the most notable features of the Sing-box client is its support for multiple platforms, including Android, iOS, macOS, and more.

# Features
- Connects to the fastest configuration.
- Directly accesses Iranian websites when the VPN is active.
- Blocks advertisements.  
And more.

# Installation Steps
1. Download the template file.
```sh
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/singbox/default.json
```
2. Run the following commands in your server terminal:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"' | sudo tee -a /opt/marzban/.env
```
Alternatively, add the following values to the .env file located in the /opt/marzban directory:
```sh
sudo nano /opt/marzban/.env
```
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"
```

3. Restart Marzban:
```sh
marzban restart
```

## Updating
To update the templates, simply repeat step 1.

# Sing-box Download Link
- Android:
   - [SFA AppCenter](https://install.appcenter.ms/users/nekohasekai/apps/sfa/distribution_groups/publictest)
   - [SFA Github](https://github.com/SagerNet/sing-box/releases)
   - [SFA Google Play](https://play.google.com/store/apps/details?id=io.nekohasekai.sfa)
- iOS:
  - [SFI](https://apps.apple.com/us/app/sing-box/id6451272673)
- macOS：
  - [SFM](https://apps.apple.com/us/app/sing-box/id6451272673)

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