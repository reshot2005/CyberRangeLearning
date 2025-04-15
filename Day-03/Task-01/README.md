## Apache Basic Authentication 

## 📌 Objective

To set up **Basic Authentication** Login page in Apache for a custom `index.html` page, such that users must enter valid credentials to access the protected content.

## ✅ Features

- Custom `index.html` page as homepage
- Password-protected access using Apache `.htaccess`
- User credentials securely stored using `.htpasswd`
- Authentication popup appears before accessing protected content
- Auto-logout on browser restart or when session expires



---

## 🛠️ Setup Steps

### Step 1: Create a Protected Directory

```bash
sudo mkdir /var/www/html/protected
```

### Step 2: Create a User for Authentication
```bash
sudo apt install apache2-utils
sudo htpasswd -c /etc/apache2/.htpasswd Shotx
```
### Step 3: Create .htaccess File Inside /protected
```bash 
sudo nano /var/www/html/protected/.htaccess
# Write the following 
AuthType Basic
AuthName "Restricted Area"
AuthUserFile /etc/apache2/.htpasswd
Require valid-user
```
### Step 4: Allow .htaccess Overrides in Apache Config
```bash
sudo nano /etc/apache2/apache2.conf
# Change to
<Directory /var/www/>
    AllowOverride All
# Restart
sudo systemctl restart apache2
```
### Step 6: Access the Apache server
```bash 
http://ipaddress/
```

