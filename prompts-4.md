# 🐧 Linux Commands and Explanations

## 📦 Basic Commands

| **Command**                | **Explanation**                                                  |
|---------------------------|-----------------------------------------------------------------|
| `setxkbmap tr`            | Sets the keyboard layout to **Turkish**                         |
| `clear`                   | Clears the terminal screen                                       |
| `pwd`                     | Shows the **current working directory path**                    |
| `ls`                      | Lists **files and folders** in the current directory            |
| `cd`                      | Changes directory; without argument goes to **home directory**  |
| `cd ..`                   | Moves **one folder up** (to the parent directory)               |
| `ls -l`                   | Lists in **long format** (file size, date, permissions, etc.)   |
| `.folderexample`          | A folder starting with `.` is a **hidden folder**               |
| `ls -a`                   | Shows **all files including hidden ones**                       |
| **Case sensitivity**      | Linux commands and filenames are **case-sensitive**             |
| `cd /root/Desktop/folder` | **Absolute path** – goes to exact full path                     |
| `cd root`                 | **Relative path** – moves to "root" inside current directory    |
| `cd ~`                    | Goes to the **home directory**                                  |
| `ls x/y/*.txt`            | Lists **all `.txt` files** in subfolder `y` under folder `x`    |
| `ls -la`                  | Detailed view including hidden files                            |
| `ls -R`                   | Lists **recursively** all files and folders                     |
| `ls -r`                   | Lists files in **reverse order**                                |
| `ls -t`                   | Sorts by **modification time**, latest files first              |
| `touch file.txt`          | **Creates an empty file**                                       |
| `file filename.txt`       | Displays the **file type**                                       |
| `cat filename.txt`        | Prints the **contents** of the file                             |
| `nano filename.txt`       | Opens file in **Nano editor**                                   |
| `less file.txt`           | Views long files **page by page**, press `q` to quit            |
| `history`                 | Shows previously used commands                                  |
| `!!`                      | Repeats the **last command**                                    |
| `!30`                     | Runs the command with **ID 30** from `history`                  |

---

## 📄 File and Directory Operations

| **Command**                  | **Explanation**                                                      |
|-----------------------------|---------------------------------------------------------------------|
| `cp -i file.txt Notes/`      | Copies file to folder; asks if overwrite is needed                  |
| `mv file.txt file1.txt`      | Renames or moves file                                               |
| `mv file.txt Notes/`         | Moves file into folder                                              |
| `mkdir folder`               | Creates a new folder                                                |
| `mkdir -p folder1/folder2`   | Creates nested folders                                              |
| `rm file.txt`                | Deletes a file                                                    |
| `rm -rf Notes1`              | Recursively and forcefully deletes folder (⚠ dangerous!)          |
| `rm -i *.txt`                | Prompts before deleting each `.txt` file                           |
| `rmdir foldername`           | Deletes a folder only if it is **empty**                           |
| `find / -name a.txt`         | Searches for file named `a.txt`                                    |
| `man command`                | Opens manual page for command                                      |
| `help command`               | Shows help for a **built-in** shell command                        |
| `whatis cat`                 | Shows one-line description of a command                            |

---

## ⚙️ Environment Variables & Aliases

| **Command**                | **Explanation**                                                      |
|----------------------------|---------------------------------------------------------------------|
| `alias l='ls -l'`          | Creates a shortcut (alias) named `l`                               |
| `unalias l`                | Removes alias `l`                                                  |
| `echo $USER`               | Shows current username                                             |
| `echo $HOME`               | Shows user's home directory                                        |
| `env`                      | Lists all environment variables                                    |
| `echo $PATH`               | Shows path used to search commands                                 |

---

## 📄 Text Processing Commands

| **Command**                 | **Explanation**                                                    |
|-----------------------------|------------------------------------------------------------------|
| `head file.txt`             | Shows first 10 lines of file                                     |
| `tail file.txt`             | Shows last 10 lines of file                                      |
| `sort file.txt`             | Sorts lines in ascending order                                   |
| `sort -r file.txt`          | Sorts in descending order                                        |
| `uniq file.txt`             | Removes duplicate adjacent lines                                 |
| `uniq -c file.txt`          | Counts how many times each line occurs                           |
| `wc file.txt`               | Shows number of lines, words, characters                         |
| `nl file.txt`               | Adds line numbers to output                                      |
| `grep root /etc/passwd`     | Searches for "root" in file                                      |
| `grep -i root /etc/passwd`  | Case-insensitive search                                          |
| `locate foldername.txt`     | Finds file by name using index                                   |
| `updatedb`                  | Updates the `locate` index                                       |
| `tee output.txt`            | Writes output to a file **and** displays it                      |

---

## 📦 Archiving and Compression

| **Command**                     | **Explanation**                                                |
|--------------------------------|----------------------------------------------------------------|
| `tar -cvf file.tar folder/`     | Creates a tar archive                                         |
| `tar -czvf file.tar.gz folder`  | Compresses with gzip                                         |
| `tar -xvf file.tar`             | Extracts a tar archive                                       |
| `gzip file.txt`                 | Compresses a file                                           |
| `gunzip file.txt.gz`            | Decompresses a gzip file                                    |
| `unzip file.zip`                | Extracts a zip archive                                     |

---

## 🌐 Network Commands

| **Command**                    | **Explanation**                                                |
|-------------------------------|----------------------------------------------------------------|
| `ping google.com`              | Sends ping to a domain                                       |
| `ip a`                        | Shows network interfaces                                     |
| `netstat -tulpn`              | Shows open ports and listening services                      |
| `curl example.com`            | Fetches URL contents                                        |
| `wget file.zip`               | Downloads file from URL                                     |
| `scp file.txt user@host:/path`| Securely copies file to remote machine                       |
| `ssh user@host`               | Connects to remote system securely                           |

---

## 🔁 Process Management

| **Command**          | **Explanation**                                              |
|----------------------|--------------------------------------------------------------|
| `ps aux`             | Shows active processes                                       |
| `top`                | Real-time process viewer                                    |
| `kill 1234`          | Kills process with PID                                      |
| `sleep 100 &`        | Runs process in background                                  |
| `jobs`               | Shows background jobs                                      |
| `fg %1`              | Brings background job to foreground                         |
| `bg %1`              | Sends job to background                                     |

---

## ⏲️ Scheduling (cron)

| **Command**              | **Explanation**                                              |
|--------------------------|--------------------------------------------------------------|
| `crontab -e`             | Edits the crontab (task schedule)                            |
| `* * * * * cmd`          | Runs command every minute                                    |
| `@reboot script.sh`      | Runs script at system boot                                   |
| `systemctl list-timers`  | Lists all active timers (for `systemd`)                     |

---

## 🧠 Additional Notes

- Use `alias` and `unalias` to create command shortcuts.
- `grep`, `wc`, `sort`, and `uniq` are powerful for text file processing.
- `find` searches the filesystem; `locate` is faster but requires an updated database.
- `tee` writes output to both a file and the screen simultaneously.
- Use `man`, `--help`, and `whatis` commands to get help and documentation.
