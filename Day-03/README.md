# 📘 Cybersecurity & Python – Day 03 Documentation

## 📅 Daily Objective
 **Linux service commands**
- Understand how to install and use **SSH** and **Apache2**
- Host a simple **login page** using Apache
- Practice **remote access** using SSH with login credentials


## 📚 New Topics Learned
- What are system services in Linux and how to control them
- Introduction to **SSH (Secure Shell)** for remote system access
- Setting up and using the **Apache2 web server**
- Hosting static HTML content with Apache
- Creating a basic login page for local web server access

## 🛠️ New Methods
- Installing network services using APT
- Using `systemctl` to manage services (start, stop, enable, status)
- Connecting securely via SSH using credentials
- Deploying an HTML login form to Apache’s web root (`/var/www/html`)

---

## 💻Commands USED
```bash
# Service management
sudo systemctl status apache2        # Check Apache service status
sudo systemctl start apache2         # Start Apache service

# SSH installation and usage
sudo apt install openssh-server      # Install SSH server
sudo systemctl status ssh            # Check SSH status
ssh username@ipaddress              # SSH login

# Apache setup
sudo apt install apache2             # Install Apache web server


