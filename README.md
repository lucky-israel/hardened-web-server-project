# ⚔️ Hardened Web Server Project (Week 1 – SysAdmin Cohort)

Hey! I'm rolling deep into Week 1 of the SysAdmin Cohort, and this repo is the frontline of my war on insecure servers.

In this project, I deployed and locked down a LAMP/LEMP stack like a true DevSecOps mercenary.  
Objective? **# Secure Ubuntu Server Setup with LAMP Stack & SSL

This project contains the setup, configuration, and hardening steps I took to deploy a secure static/demo PHP website on an Ubuntu server hosted on Azure.

It includes Apache, PHP, MySQL, firewall rules, SSL via Let's Encrypt, and some of the configuration process.
**

---

## 💡 What I Did

- 🧱 Spun up a fresh Linux box (Ubuntu/Debian-based) on Azure cloud vm
- - 🔥 Installed & hardened Apache/Nginx — security headers, disabled directory listing, least-privilege perms
- 🛡️ Secured MySQL/MariaDB — used `mysql_secure_installation`, set up a tight user with zero escalation privileges
- 🧬 Configured PHP with maximum paranoia — stripped dangerous functions, fine-tuned error handling
- 🔒 Deployed Let's Encrypt TLS with `certbot`
- 🧨 Tuned SSL for modern protocols, strong ciphers, no legacy support — 
- 🌐 Deployed a tiny demo site to prove it's alive & secure
- 🔐 Hardened the OS firewall with UFW — allowed only 22 (SSH), 80 (HTTP), 443 (HTTPS) and ICMP for ping and DNS

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
