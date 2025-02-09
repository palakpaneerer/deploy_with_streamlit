# deploy_with_streamlit

# Command Prompt Command-List 
| Command | Description | Example Usage |
|---------|-------------|---------------|
| `cd` / `chdir` | Change directory or display the current directory | `cd C:\Users\Username\Documents` |
| `dir` | List files and directories in the current location | `dir C:\Users\Username\Documents` |
| `tree` | Display directory structure in a tree format | `tree C:\Users\Username\Documents` |
| `tree /f` | Display files along with directory structure | `tree /f C:\Users\Username\Documents` |
| `tree /a` | Use ASCII characters instead of extended characters for tree display | `tree /a C:\Users\Username\Documents` |
| `cls` | Clear the console screen | `cls` |
| `help` | Show a list of available commands or details of a specific command | `help dir` |
| `copy` | Copy files from one location to another | `copy file.txt C:\backup\file.txt` |
| `xcopy` | Copy files and directories, including subdirectories | `xcopy C:\source C:\destination /E /I` |
| `ren` / `rename` | Rename files or directories | `ren oldname.txt newname.txt` |
| `move` | Move files or rename directories | `move file.txt C:\new_folder\file.txt` |
| `del` | Delete files | `del file.txt` |
| `rmdir` / `rd` | Remove directories (use `/s` for non-empty directories) | `rmdir /s /q C:\folder_to_delete` |
| `mkdir` / `md` | Create a new directory | `mkdir C:\new_folder` |
| `type` | Display the contents of a text file | `type file.txt` |
| `more` | View text file contents one screen at a time | `more file.txt` |
| `attrib` | View or change file attributes | `attrib +R file.txt` |
| `ipconfig` | Display network configuration details | `ipconfig /all` |
| `where` | Locate the path of an executable file or command | `where notepad.exe` |
| `exe` | Execute a program from the command prompt | `C:\Program Files\App\app.exe` |
| `exit` | Close the command prompt | `exit` |

# Github Command-List
### Create Repositry
1. githubにてレポジトリを作成 (httpsのURLが表示されるのでそこに留まる。)
2. Personal access tokens (classic) を作成
3. `cd C:\Users\jinno\Desktop\scope_verify\myproject`
4. `git init`
5. `git add -A`
6. `git commit -m "first commit"`
7. `git branch -m "main"`
8. `git status`
9. `git remote add origin https://[user_name]:[access_token]@github.com/palakpaneerer/scope_verify.git`
10. `git push -u origin main`
* `git remote remove origin` # git remoteに誤ったgitをセットしてしまった場合

### Github push
1. `git add -A`
2. `git commit -m "[comment]"`
3. `git push`


# Make/Renew requirements.txt
`poetry self add poetry-plugin-export`  
`poetry export -f requirements.txt --output requirements.txt --without-hashes`  


# Versions
- Streamlit can use python until 3.12 as of 6th Feb 2025.




# Database setting  
myproject/  
│── database/             
|   ├── models.py        # Table Definition - SQLAlchemy  
│   ├── database.py      # Database Connection / Initialisation  
│   ├── crud.py          # Data CRUD manupulate  
│── app.py               # Entry Point  
│── data.db              # Automatically made after start app.py  

