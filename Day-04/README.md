# 📅 Day 04 – Cybersecurity Lab Setup & GitHub Integration



## 🔔 Daily Objective

- Set up the cybersecurity lab environment using **VMware** and **Kali Linux**
- Connect **Kali terminal** to **GitHub** using **SSH authentication**
- Practice pushing project files from Kali to GitHub via terminal
- Install and configure **VS Code** on Kali Linux for code editing



## 🧠 New Topics Learned

- 🔐 **SSH Key Authentication with GitHub** from Kali Linux  
- 🧭 Navigating GitHub via terminal on a Linux environment  
- ⚙️ Initial Kali setup steps in VMware



## 🧪 New Methods

- Creating & adding SSH keys to GitHub  
- Cloning and pushing repos using SSH instead of HTTPS  
- Using terminal-based Git workflows inside a virtualized environment



## 💻 New Commands

```bash
# Generate SSH Key
ssh-keygen -t ed25519 -C "my_email@example.com"

# Copy SSH key to clipboard (manually open with cat on Kali)
cat ~/.ssh/id_ed25519.pub

# Push repo to GitHub via terminal
git init
git remote add origin git@github.com:username/repo.git
git add .
git commit -m "Initial commit"
git push -u origin main
