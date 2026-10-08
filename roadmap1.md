# Beginner Web Development Plan

**Goal:** Build a small web app gradually, starting with a real webpage on Day 1.  
**Daily routine:** 15 minutes of terminal practice, 15 minutes of Python, and 20–30 minutes improving the app. Take longer when you need it; understanding matters more than speed.

## Days 1–7: From webpage to Python server

| Day | Terminal — 15 minutes | Python — 15 minutes | Web app |
|---|---|---|---|
| **1: First webpage** | Run `mkdir -p my-webapp && cd my-webapp && touch index.html`. Open `index.html` in a text editor. | Create `hello.py` containing `print("Hello, web!")`, then run it with `python3 hello.py`. | Add a title, heading, and paragraph to `index.html`. Open the file in your browser. **You have a webpage today.** |
| **2: HTML structure** | Practice `pwd`, `ls`, `cd`, and `cat index.html`. | Use variables and `print()` to make a tiny profile program. | Add headings, links, and a list to the page. |
| **3: CSS** | Create `style.css` with `touch style.css`. Practice `cp` and `mv` on a spare file. | Use `input()` and string variables to make a greeting program. | Link `style.css` from your HTML. Add colors, spacing, and a readable font. |
| **4: Forms** | Practice `mkdir`, `touch`, and relative paths such as `../`. | Use `if`/`else` to respond differently to user input. | Add a form with a text box and submit button. It won’t save anything yet. |
| **5: Lists and layout** | Use `cat`, `head`, and `tail` to inspect files. | Learn lists; make a short to-do list and print each item with a loop. | Improve the page layout and add a visible example task list. |
| **6: First backend** | Create a virtual environment with `python3 -m venv .venv`, then activate it with `source .venv/bin/activate`. | Install Flask with `python -m pip install flask`. Write a tiny script that imports Flask. | Move the page into a `templates` folder. Create a Flask route that serves it. |
| **7: Run the app** | Practice starting and stopping a process; stop the development server with `Ctrl+C`. | Review functions and imports by reading your Flask app. | Run the Flask development server and open its local address in your browser. Your page now comes from Python. |

### Day 1: Create your first webpage

Your project folder starts like this:

```text
my-webapp/
└── index.html
```

Add this to `index.html`:

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>My First Webpage</title>
  </head>
  <body>
    <h1>Hello, web!</h1>
    <p>This is my first webpage.</p>
  </body>
</html>
```

Open `index.html` in your browser. Also create and run a Python script:

```python
print("Hello, web!")
```

```bash
python3 hello.py
```

**Day 1 finish line:** See your webpage in the browser and successfully run a Python script from the terminal.

### Day 6: Minimal Flask app

By Day 6, your project folder will look like this:

```text
my-webapp/
├── app.py
├── templates/
│   └── index.html
└── .venv/
```

Create `templates/` and move `index.html` into it. Add this to `app.py`:

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def home():
    return render_template("index.html")

if __name__ == "__main__":
    app.run(debug=True)
```

With your virtual environment active, run:

```bash
python app.py
```

Open the local address shown in the terminal in your browser.

## Days 8–14: Make it interactive and save data

| Day | Terminal — 15 minutes | Python — 15 minutes | Web app |
|---|---|---|---|
| **8: Requests and routes** | Practice `grep` to find text in your files. | Write a function that accepts a value and returns a result. | Add a second route, such as `/about`. Learn that routes connect URLs to Python functions. |
| **9: Form handling** | Practice shell history and tab completion. | Learn dictionaries and key/value pairs. | Make the form submit to Flask. Read the submitted value and show it on the page. |
| **10: Validation** | Practice redirecting command output with `>` and `>>`. | Learn `try`/`except` and basic error handling. | Reject an empty task and display a helpful message. |
| **11: Templates** | Use `find` to locate files in the project. | Review lists, dictionaries, and loops. | Use a template loop to display tasks from Python instead of hard-coding them in HTML. |
| **12: Persistence** | Practice reading and writing files from the terminal. | Practice loading and saving a list as JSON. | Save tasks to a JSON file so they remain after the server restarts. |
| **13: Git** | Check Git is installed; practice `git status`, `git add`, and `git commit`. | Review your functions and rename unclear variables. | Make your first Git commit. Add a README explaining how to run the app. |
| **14: Review and test** | Practice `git log` and `git diff`. | Write a few simple tests for your task-handling functions. | Try the app from a fresh browser session. Fix a bug or improve a feature. |

## After Day 14

Continue improving the same app, adding one concept at a time:

1. Replace the JSON file with **SQLite**.
2. Add the ability to **edit and delete tasks**.
3. Improve the interface with a little **JavaScript**.
4. Learn **SQL**, automated testing, and deployment.
5. Deploy the app and document how to run it.

Keep the daily terminal and Python practice going, but connect each new skill to something the app needs.

## Useful habits

- Spend about one-third of your time learning concepts and two-thirds writing code.
- After a lesson, try recreating the idea without looking at the tutorial.
- Keep a note of commands and errors you had to look up.
- Make small commits as the app grows.
- Aim for a working, finished app rather than several half-finished projects.
