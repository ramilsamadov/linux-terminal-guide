# 🐧 Linux Command Cheatsheet

A handy reference list of commonly used Linux commands with English explanations.

---

## 📁 File & Directory Commands

| **Command**                 | **Explanation (English)**                                                           |
| --------------------------- | ----------------------------------------------------------------------------------- |
| `pwd`                       | Shows the **current working directory path**                                        |
| `ls`                        | Lists **files and folders** in the current directory                                |
| `ls -l`                     | Lists in **long format** (with file size, date, permissions, etc.)                  |
| `ls -a`                     | Shows **all files including hidden** ones (those starting with `.`)                 |
| `ls -la`                    | Shows **detailed view and includes hidden files**                                   |
| `ls -R`                     | Lists **recursively** all files and folders from the current location               |
| `ls -r`                     | Lists files in **reverse order**                                                    |
| `ls -t`                     | Sorts by **modification time**, latest files shown first                            |
| `.folderexample`            | A folder that starts with `.` is a **hidden folder**                                |
| `cd`                        | Changes directory; without argument goes to **home directory**                      |
| `cd ..`                     | Moves **one folder up** (to the parent directory)                                   |
| `cd /root/Desktop/folder`   | **Absolute path** – goes to exact full path                                         |
| `cd root`                   | **Relative path** – moves to "root" inside current directory                        |
| `cd ~`                      | Goes to the **home directory**                                                      |
| `ls x/y/*.txt`              | Lists **all `.txt` files** in subfolder `y` under folder `x`                        |

---

## 📄 File Handling Commands

| **Command**                 | **Explanation (English)**                                                           |
| --------------------------- | ----------------------------------------------------------------------------------- |
| `touch file.txt`            | **Creates an empty file** called `file.txt`                                         |
| `file filename.txt`         | Displays the **file type** (e.g., text, binary)                                     |
| `cat filename.txt`          | Prints the **contents** of the file to the terminal                                 |
| `nano filename.txt`         | Opens file in **Nano editor** to view/edit                                          |
| `less file.txt`             | Views long files **page by page**, press `'q'` to quit                              |
| `cp source.txt dest.txt`    | **Copies** `source.txt` to `dest.txt`                                               |
| `cp -i source.txt dest.txt` | Copy with **confirmation prompt** if the destination exists (`-i` = interactive)    |

---

## 🖥️ Terminal & Keyboard

| **Command**      | **Explanation (English)**                           |
| ---------------- | --------------------------------------------------- |
| `clear`          | **Clears** the terminal screen                      |
| `setxkbmap tr`   | Sets the keyboard layout to **Turkish**             |
| **Case sensitivity** | Linux commands and filenames are **case-sensitive** (e.g., `File.txt` ≠ `file.txt`) |

---

## ⏱️ Command History

| **Command** | **Explanation (English)**                                |
| ----------- | -------------------------------------------------------- |
| `history`   | Shows all previously used commands in terminal           |
| `!!`        | **Repeats** the last command used                        |
| `!30`       | Runs the command with **ID 30** from the `history` list  |
