## 🗂️ File Management & Navigation

| **Command**                  | **Explanation (English)**                                                                        |
| ---------------------------- | ------------------------------------------------------------------------------------------------ |
| `cp -i file.txt Notes/`      | Copies `file.txt` to `Notes/` folder. If `file.txt` already exists there, asks for confirmation. |
| `mv file.txt file1.txt`      | Renames (or moves) `file.txt` to `file1.txt`                                                     |
| `mv file.txt Notes/file.txt` | Moves `file.txt` into the `Notes/` folder                                                        |
| `mv openCv/ open`            | Renames folder `openCv` to `open`                                                                |
| `mkdir folder`               | Creates a new folder named `folder`                                                              |
| `mkdir -p folder1/folder2`   | Creates nested folders; makes `folder1` and inside it, `folder2`                                 |

---

## 🧹 Deleting Files & Folders

| **Command**        | **Explanation (English)**                                                                      |
| ------------------ | ---------------------------------------------------------------------------------------------- |
| `rm file.txt`      | Deletes the file `file.txt`                                                                    |
| `rm -rf Notes1`    | Recursively and forcefully deletes `Notes1` folder with all contents (⚠ dangerous!)            |
| `rm -i file.txt`   | Asks for confirmation before deleting `file.txt`                                               |
| `rm -i *.txt`      | Prompts before deleting each `.txt` file individually                                          |
| `rm -r foldername` | Recursively removes folder (works if it's not empty)                                           |
| `rm -f file.txt`   | Force deletes a file without asking                                                            |
| `rmdir foldername` | Deletes a folder only if it is **empty**                                                       |

---

## 🔍 Search & Help Commands

| **Command**                  | **Explanation (English)**                                                       |
| ---------------------------- | -------------------------------------------------------------------------------- |
| `find / -name a.txt`         | Searches **everywhere** for a file named `a.txt`                                |
| `find / -name a.txt -type f` | Searches for files (type: file) named `a.txt`                                   |
| `find / -name a.txt -type d` | Searches for directories (type: directory) named `a.txt`                        |
| `help command`               | Shows help for a **built-in shell command** (e.g., `help cd`, `help pwd`)       |
| `help pwd`                   | Shows brief help about the `pwd` command                                        |
| `pwd --help` or `pwd -h`     | Shows more detailed help for `pwd`                                              |
| `man command`                | Opens the **manual** page for any command (e.g., `man find`)                    |
| `whatis cat`                 | Shows a **short description** of the `cat` command                              |
| `exit`                       | Closes the terminal session                                                     |

---

### 💡 Tips

- `cp` = copy  
- `mv` = move or rename  
- `rm` = remove/delete  
- `mkdir` = make directory  
- `find` = search  
- `man` = manual  
- `whatis` = one-line manual  
- `--help` or `-h` = short help  
