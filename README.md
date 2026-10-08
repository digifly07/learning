You can copy and paste the content below into a file named `ROADMAP.md`.

***

# 🚀 Web Development Roadmap for Beginners
**Focus:** Python Backend, Light Frontend, Linux Terminal, and SDLC.
**Philosophy:** Start hands-on immediately. Build one evolving app instead of many tiny scripts.

## 📅 Phase 1: The "Visible Win" (Weeks 1–2)
**Daily Routine:** 
- 15m Terminal $\rightarrow$ 15m Python $\rightarrow$ 30m App Building.

### Week 1: From Static Page to Python Server
| Day | Terminal (15m) | Python (15m) | App Milestone |
|:---:|---|---|---|
| **1** | `mkdir`, `cd`, `touch` | `print()` and running `.py` files | Create `index.html` $\rightarrow$ View in browser. |
| **2** | `pwd`, `ls`, `cat` | Variables and basic types | Add semantic HTML (headers, lists, links). |
| **3** | `cp`, `mv`, file paths | `input()` and string formatting | Create `style.css` $\rightarrow$ Style the page. |
| **4** | `mkdir -p`, `rm` (carefully) | `if/else` conditionals | Add an HTML `<form>` with a submit button. |
| **5** | `head`, `tail`, `grep` | Lists and `for` loops | Create a hard-coded "Example Task List" in HTML. |
| **6** | `venv` (create & activate) | Installing packages with `pip` | Setup Flask $\rightarrow$ Serve `index.html` via Python. |
| **7** | `Ctrl+C` (process control) | Reviewing imports and functions | Run the Flask server $\rightarrow$ Access via `localhost`. |

### Week 2: Interaction and Data
| Day | Terminal (15m) | Python (15m) | App Milestone |
|:---:|---|---|---|
| **8** | `grep` for project searches | Functions with arguments/returns | Create a second route (e.g., `/about`). |
| **9** | Command history & Tab completion | Dictionaries (key-value pairs) | Handle Form Submit $\rightarrow$ Print input in terminal. |
| **10** | `>` and `>>` redirection | `try/except` error handling | Add input validation (no empty tasks). |
| **11** | `find` and directory traversal | Template logic (loops/conditionals) | Use Flask templates to render a Python list of tasks. |
| **12** | File reading/writing via CLI | JSON module (`json.dump`, `json.load`) | Save/Load tasks from a `.json` file. |
| **13** | `git init`, `add`, `commit` | Code refactoring (clean naming) | First Git commit $\rightarrow$ Write a `README.md`. |
| **14** | `git log`, `git diff` | Writing basic logic tests | End-to-end test: Add, Save, and View a task. |

---

## 🛠️ Phase 2: Hardening the App (Weeks 3–6)
*Now that the app works, move from "making it work" to "making it right" (SDLC).*

### 1. Data Evolution (The Database)
- **Terminal:** Learn basic SQL CLI.
- **Python:** Learn SQLAlchemy or Flask-SQLAlchemy.
- **App:** Replace the `.json` file with **SQLite**. Implement a proper table for tasks.

### 2. Feature Expansion (CRUD)
- **Concepts:** Create, Read, Update, Delete.
- **App:** 
    - Add a "Mark as Complete" checkbox.
    - Add a "Delete" button for each task.
    - Add a "Filter" (Show All / Show Completed).

### 3. Light Frontend Polish
- **Concepts:** Basic JavaScript (DOM manipulation), CSS Flexbox/Grid.
- **App:** 
    - Use JS to show a confirmation alert before deleting.
    - Make the app responsive (works on mobile).

### 4. Software Development Life Cycle (SDLC)
- **Planning:** Use a Trello board or simple text file to list "Backlog" $\rightarrow$ "In Progress" $\rightarrow$ "Done".
- **Version Control:** Use Git branches for new features (`git checkout -b feature-name`).
- **Testing:** Write tests for your backend logic using `pytest`.

---

## 🌐 Phase 3: Deployment and Beyond (Weeks 7+)
- **Environment Variables:** Learn `.env` files to hide secret keys.
- **Production Server:** Move from the Flask dev server to **Gunicorn**.
- **Deployment:** Deploy the app to a platform like **Render, Railway, or Fly.io**.
- **Linux Hardening:** Learn basic SSH and how to manage a remote server.

## 📚 Resource Cheat Sheet
- **HTML/CSS/JS:** [MDN Web Docs](https://developer.mozilla.org/)
- **Python:** [Official Python Tutorial](https://docs.python.org/3/tutorial/)
- **Git:** [Pro Git Book](https://git-scm.com/book/en/v2)
- **Backend:** [Flask Documentation](https://flask.palletsprojects.com/)
