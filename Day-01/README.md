# 🐧 Linux Command Practice - Project Tasks



## 📁 Task 1: File and Directory Management

### 📝 Scenario:
You're organizing files for a project.

1. Create a folder named `project`.
2. Go inside the `project` folder.
3. Create a file named `notes.txt`.
4. Later, you decide to delete the entire `project` folder.

### ✅ Solution:
```bash
# Step 1: Create a folder
mkdir project

# Step 2: Enter the folder
cd project

# Step 3: Create the file
touch notes.txt

# Step 4: Go back and delete the folder
cd ..
rm -r project
```

## 📂 Task 2: Viewing and Moving Files
### 📝 Scenario:

You write some text into a file called message.txt that says "Backup Completed". After verifying the content, you want to move it into a folder called backup.

```bash
# Step 1: Create the file with content
echo "Backup Completed" > message.txt

# Step 2: View the content
cat message.txt

# Step 3: Create the backup folder
mkdir backup

# Step 4: Move the file to the backup folder
mv message.txt backup/

```
## Task 3: Process and Disk Usage
###🖥️ Scenario:
Your system is running slow. You want to:

Check which processes are currently running.

See how much disk space is left on your machine.

```bash

# View running processes
top
# or
ps aux

# Check disk usage
df -h


```
