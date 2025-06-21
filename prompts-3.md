## 🧰 Useful Terminal Tools & Text Processing

| **Command**                         | **Explanation (English)**                                             |
| ----------------------------------- | --------------------------------------------------------------------- |
| `alias l='ls -l'`                   | Creates a shortcut (alias) named `l` to run `ls -l`                   |
| `unalias l`                         | Deletes the alias `l`                                                 |
| `echo "Hello World"`                | Prints "Hello World" to the terminal (works like `printf`)            |
| `echo "Hello" > file.txt`           | Writes "Hello" to `file.txt`, **overwrites** existing content         |
| `cat > x.txt`                       | Overwrites `x.txt` with new input from user (Ctrl+D to save)          |
| `ls -la ./foldername`               | Lists **all** files (including hidden) in `foldername` in long format |
| `` ls -la ./foldername | less ``    | Views the list with scrollable pagination using `less`                |
| `` ls | tee x.txt ``                | Lists current directory contents **and** saves output to `x.txt`      |
| `echo $USER`                        | Displays the current username                                         |
| `echo $HOME`                        | Displays the current user’s home directory                            |
| `env`                               | Lists all environment variables                                       |
| `echo $PATH`                        | Shows the directories used to search executable commands              |
| `whoami`                            | Shows the current logged-in username                                  |

---

## 📄 File Previewing & Counting

| **Command**                         | **Explanation (English)**                                            |
| ----------------------------------- | -------------------------------------------------------------------- |
| `head /folder/folder2/folder3/file` | Displays the **first 10 lines** of the specified file                |
| `head -n 5 file.txt`                | Shows **first 5 lines** of `file.txt`                                |
| `tail file.txt`                     | Shows **last 10 lines** of `file.txt`                                |
| `sort file.txt`                     | Sorts lines in `file.txt` in ascending (A–Z) order                   |
| `sort -r file.txt`                  | Sorts lines in descending (Z–A) order                                |
| `uniq file.txt`                     | Removes duplicate lines (only if they are adjacent)                  |
| `` sort file.txt | uniq ``          | Sorts and removes duplicates                                         |
| `uniq -c file.txt`                  | Counts occurrences of each line                                      |
| `uniq -u file.txt`                  | Shows lines that appear only once                                    |
| `uniq -d file.txt`                  | Shows only duplicate lines                                           |
| `wc file.txt`                       | Prints line, word, and character counts for `file.txt`               |
| `wc -l file.txt`                    | Line count only                                                      |
| `wc -w file.txt`                    | Word count only                                                      |
| `wc -c file.txt`                    | Character count only                                                 |
| `nl file.txt`                       | Displays file with line numbers                                      |
| `cat -n file.txt`                   | Same as `nl`, displays file with line numbers                        |

---

## 🔍 Search & Info Tools

| **Command**                | **Explanation (English)**                                            |
| -------------------------- | -------------------------------------------------------------------- |
| `grep root /etc/passwd`    | Searches for "root" inside the file `/etc/passwd`                   |
| `grep -i root /etc/passwd` | Case-insensitive search for "root"                                  |
| `locate foldername.txt`    | Searches for files by name using an indexed database                |
| `updatedb`                 | Updates the file location database used by `locate`                 |
| `man -k copy`              | Lists all man pages related to the keyword "copy"                   |
| `apropos copy`             | Same as `man -k`, shows commands related to "copy"                  |
| `whereis ls`               | Shows the location of the `ls` command binary, source, and man page |

---

### 📌 Tips

- `alias` helps create command shortcuts.  
- `echo > file` or `cat > file` overwrites contents.  
- `tee` lets you view and save output at the same time.  
- `sort`, `uniq`, `wc`, `grep` are powerful for text file processing.  
- `locate` is faster than `find`, but it requires `updatedb` to be run first.  
