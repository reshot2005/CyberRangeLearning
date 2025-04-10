# 📘 Day 02: Linux Basics – Custom Commands & IP Info

Welcome to Day 01 of my Linux learning journey! 🚀  
The focus for today was on exploring **basic Linux commands**, particularly around **networking** and **custom command creation**.



## 📌 Daily Objective

> 🎯 Learn and practice **new Linux commands**, with a focus on **IP-related information** and creating **custom command-line utilities**.


## 📚 New Topics Learned

- Creating **custom commands** to fetch system IP addresses.
- Understanding the difference between **IPv4** and **IPv6** display formats.
- Using powerful text processing tools like:
  - `awk`
  - `grep`
- Filtering command outputs effectively.

## ⚙️ New Methods Explored

- Extracting specific fields using:
  ```bash
  awk '{print $2}'
  grep -v inet6
  ```
- Final output
```bash
    ifconfig | grep inet | grep -v inet6 | awk '{print $2}'
```
# 📝 Summary, 🔚 Conclusion & 💬 Personal Feedback



## 📝 Summary

Today’s session provided a hands-on intro to **network-related commands in Linux**, with a key takeaway being the **creation of custom command chains** to get meaningful output from verbose system tools.  
Learning to **filter and parse** output helped in making Linux work more like a programmable environment rather than just a terminal.



## 🔚 Conclusion

- ✅ Gained confidence using CLI tools like `awk` and `grep`.
- 🛠️ Understood the value of **combining small utilities** to create powerful command-line tools.
- 💡 Realized that Linux is not just about commands, but about **how you combine them**.



## 💬 Personal Feedback

> Today was exciting! I learned how to manipulate Linux output like a pro.  
> Creating a **custom IP command** using `ifconfig`, `grep`, and `awk` made me feel like I'm building my own tools.  
> Looking forward to digging deeper into shell scripting and automation in the upcoming days.


