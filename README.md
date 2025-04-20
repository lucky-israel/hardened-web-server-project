# ⚔️ Hardened Web Server Project (Week 1 – SysAdmin Cohort)

Hi! Welcome to my server project ,phew it was quite uneasy at first but was fun all the way Week 1 of the SysAdmin Cohort, and this repo is the frontline of my war on insecure servers.

In this project, I deployed and locked down a like a true DevSecOps mercenary.  
Objective? **# Secure Ubuntu Server Setup with LAMP Stack & SSL


**

---

## 💡 What I Did

This project contains the setup, configuration, and hardening steps I took to deploy a secure static/demo PHP website on an Ubuntu server hosted on Azure.

It includes Apache, PHP, MySQL, firewall rules, SSL via Let's Encrypt, and some of the configuration process.
---

## 🧠 Why This Matters

Installing apache and other web server vis easy but can evryone secure it.

---

## 🔐 Security Wins

- `X-Content-Type-Options: nosniff`
- `X-Frame-Options: DENY`
- `Content-Security-Policy: default-src 'self'`
- Directory listing? Disabled.
- Dangerous PHP functions? Nuked.
- MySQL wildcards? Denied.
- HTTP to HTTPS redirect? Always on.
- TLS 1.0/1.1? Buried.

---

## 📁 File Map

```txt
apache/       → Apache config, headers
nginx/        → Nginx (alternative)
mysql/        → DB setup & hardening
php/          → PHP hardening configs
firewall/     → UFW rules
ssl/          → TLS/SSL configs, Certbot notes
website/      → Demo site code
screenshots/  → SSL Labs results, terminal outputs
setup/        → Installation scripts & deployment notes
