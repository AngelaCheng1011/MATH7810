# GitHub, Codespaces & Lab ready

## What you will learn

1. What a **repo** is and how to work in **your own copy** (fork) on GitHub.
2. Use **Codespaces** (our online classroom computer) — and that the **first open is slow**.
3. Open a Jupyter notebook, pick the right **kernel**, and run a cell.
4. **Commit** and **Push** so your work is saved on **your** GitHub (portfolio habit).
5. **Sync fork** later when the instructor adds new week folders.
6. **Stop** your Codespace to save minutes.

---

## Start here: what is a **repo**?

### Repository (**repo**) — plain meaning

A **repo** is a **project folder on the internet** that holds course materials:

- notebooks (`.ipynb`)
- data files (`.csv`) when needed
- instructions (`README.md`)

**This course uses one labs repo** for the term: `MATH7810`. Your instructor adds new week folders over time; you keep **one fork** and **Sync** to get updates.

### Then: GitHub, fork, Codespace, Sync, Commit, Push


| Word                       | Plain meaning                                                                                                                     |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **GitHub**                 | The website that **hosts** repos.                                                                                                 |
| **Fork** (verb)            | Click **Fork** to **make your own copy** of the instructor’s repo under **your** account.                                         |
| **Fork** (noun)            | **Your fork** = **your own copy** on github.com. You work there; the instructor’s original stays unchanged.                       |
| **Codespace**              | A **classroom computer in the browser** with your fork already open — you run notebooks there.                                    |
| **Sync fork**              | Pull **new files** the instructor added (e.g. Week 2 notebooks) into **your** fork.                                               |
| **Save** (in the notebook) | Keeps edits on the **Codespace** while it is open (`File → Save`).                                                                |
| **Commit**                 | **Stamp this version on the Codespace** — a named snapshot (e.g. “Week 1 lab ready”). Still only on the Codespace until you Push. |
| **Push**                   | **Send** those stamped versions to **your fork on github.com**.                                                                   |
| **Stop Codespace**         | Turn off the cloud computer so you do not burn Codespaces minutes (180 hrs/month).                                                |


**Analogies**


| Idea          | Analogy                                                                      |
| ------------- | ---------------------------------------------------------------------------- |
| **Repo**      | One shared course folder online.                                             |
| **Fork**      | Duplicate the folder into **your** drive; you edit your duplicate.           |
| **Codespace** | A lab PC that already has the folder open — no USB, no “wrong Desktop path”. |
| **Sync fork** | Download the teacher’s new handouts into your duplicate folder.              |
| **Save**      | Save the file on that lab PC.                                                |
| **Commit**    | Stamp a named version **on the lab PC**.                                     |
| **Push**      | Upload those stamped versions to **your** online folder on GitHub.           |


---



## In class — fork and Codespace



### Step 1 — GitHub account (should already be done)

You should already have:

- a GitHub account  
- **2FA** on  
- applied for **GitHub Education** (Moodle checklist)

If not, create an account at [github.com](https://github.com) now, then continue — and finish 2FA / Education after class.

### Step 2 — Fork the instructor’s labs repo (**once for the term**)

1. Open the course repo your instructor shares:
  [https://github.com/taliawu17/MATH7810](https://github.com/taliawu17/MATH7810)
2. Click **Fork** (top right) → create under **your** username.
3. Check the URL: `yourusername/MATH7810` — **your** name must appear.

You now have **your own repo** for the whole term. Do **not** fork again each week.

### Step 3 — Start a Codespace from **your fork**

1. Open **your fork** (not only the instructor’s page).
2. Click green **Code** → tab **Codespaces** → **Create codespace on main**.
3. **Wait.** The first time often takes **1–5 minutes**. You may see “Setting up your codespace” — this is normal.
  - **Do not** expect it to open instantly.  
  - **Do not** keep clicking **Create** (that makes many Codespaces and wastes minutes).

GitHub will **automatically name** each Codespace (e.g. `fuzzy-pancake`). You do not choose the name.

**Next time you work:** open the **same** Codespace from **Code → Codespaces** (click its name). Reopening is usually faster than the first create, but can still take under a minute to a few minutes. Do **not** create a new Codespace every class unless the old one was deleted.

### Step 4 — Open this guide’s folder and a notebook

1. In the left file tree, open `week01` (this folder).
2. When your instructor adds `W01_Ch1_PythonBasics.ipynb`, open that `.ipynb`.
3. Click **Run** on a cell. When asked to **Select Kernel**:
  - Choose **Python Environments** (not “Jupyter Kernel”, not “Existing Jupyter Server”).
  - Then choose **Python 3.12.x** whose path looks like `/usr/local/.../python`.  
  - **Do not** choose **+ Create Python Environment**.  
  - If several “Python 3.12” lines appear, pick one under `/usr/local/` and continue.
4. Run the first cell for simple check:

```python
import numpy as np
import pandas as pd
print("Lab ready:", np.__version__, pd.__version__)
```

If Codespace asks to **Install/Enable** Python + Jupyter first, say yes, wait, then:

`Ctrl+Shift+P` (Windows) or `Cmd+Shift+P` (Mac) → type **Reload Window** → Enter → open the notebook again → Select Kernel as above.

### Step 5 — Green-light check (lab ready)

You are **lab ready** when you can:

- Open a `.ipynb` in Codespace (not as raw JSON text)  
- Select a **Python 3.12** kernel under `/usr/local/`  
- `import numpy` and `import pandas` without error



### Step 6 — Commit and Push (required habit)

Remember: **Commit** = stamp on the Codespace; **Push** = send to **your fork** on github.com. Commit alone does **not** update the GitHub website.

1. **Save** the notebook (`File → Save`).
2. Open **Source Control** (branch icon, left sidebar).
3. Write a short message (e.g. `Week 1 lab done`) → **Commit**.
   - If Codespace asks to **stage all changes and commit**, choose **Yes**.
4. Click **Sync Changes** / **Push**.
5. Refresh **your fork** on github.com — you should see the update **after Push**.

You only push to **your fork**, never the instructor’s original repo.

### Step 7 — Stop the Codespace

1. On github.com, open **your fork** → **Code** → **Codespaces**.
2. Find your Codespace → **⋯** (or stop control) → **Stop codespace**.
3. Close the browser tab.

Do **not** leave Codespaces running overnight — minutes are limited especially before Education is approved.

---



## Later weeks — Sync fork (same fork all term)

When the instructor adds new notebooks:

1. On github.com, open **your fork** of `MATH7810`.
2. Click **Sync fork** (if GitHub shows that your fork is behind).
3. Open **Code → Codespaces** and reopen your **existing** Codespace even if you **stopped** it earlier.  
   **Stop** only turns the machine off — it is still in the list. Prefer this over creating a new Codespace (saves minutes; keeps any work you had not pushed yet).
4. If the new week folder does not appear yet, **Pull** in the Codespace (Source Control → **⋯** → **Pull**, or in the terminal: `git pull`).
5. Work → **Commit** → **Push** → **Stop** Codespace.

You do **not** create a new fork each week.

---



## Troubleshooting


| Problem                                                   | What to do                                                                                                                                      |
| --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Codespace will not open / stuck on “Setting up”           | **Wait several minutes.** First setup is slow. Do **not** click Create repeatedly. If still stuck after ~10 minutes, refresh once or ask a TA.  |
| `.ipynb` looks like text (JSON) **on the GitHub website** | Do not edit there. Open a **Codespace**, then open the notebook.                                                                                |
| `.ipynb` looks like text (JSON) **inside Codespace**      | Install extensions (see below), then **Reload Window**.                                                                                         |
| Error: `markdown-it-renderer` / notebook editor           | Install **Python** + **Jupyter** + **Jupyter Notebook Renderers**, then **Reload Window**.                                                      |
| Prompt: install recommended **Python** extension?         | Choose **Yes** (Microsoft).                                                                                                                     |
| Error: cannot open … `jupyter-notebook`                   | Install **Jupyter** (Microsoft), Reload Window. Do **not** choose “Open in Text Editor” for class work.                                         |
| `ModuleNotFoundError: pandas` (or numpy)                  | Wait until Codespace **finishes building**. Then in the Codespace terminal: `pip install -r requirements.txt` → **Restart kernel** → try again. |
| Opened instructor’s repo by mistake                       | Open **your fork** (`yourusername/MATH7810`) and create/open Codespace **there**.                                                               |
| Lost my Codespace / everything feels new                  | You may have created a **new** Codespace. On your fork: **Code → Codespaces** → open the **existing** named one.                                |
| Many Python 3.12 options when selecting kernel            | **Python Environments** → a **Python 3.12** under `/usr/local/`. Skip **Create Python Environment**.                                            |
| Education still pending                                   | Still do this lab with a free account; tell the instructor if Copilot/minutes are limited.                                                      |




### Notebook shows as JSON, or renderer error (in Codespace)

1. Click **Extensions** (four squares on the left).
2. Install (publisher: **Microsoft**): **Python**, **Jupyter**, **Jupyter Notebook Renderers**.
3. `Ctrl/Cmd+Shift+P` → **Developer: Reload Window**.
4. Close the notebook tab → open the `.ipynb` again.
5. If still JSON: right-click → **Open With…** → **Jupyter Notebook**.
6. Still broken? `Ctrl/Cmd+Shift+P` → **Codespaces: Rebuild Container** (wait a few minutes).



### Where is “Reload Window”?

1. Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac).
2. Type `Reload Window`.
3. Click **Developer: Reload Window**.



### Select Kernel — what students usually see

**First screen:**


| Option                      | What to do                                |
| --------------------------- | ----------------------------------------- |
| **Python Environments**     | **Choose this**.                          |
| **Jupyter Kernel**          | Skip unless an instructor says otherwise. |
| **Existing Jupyter Server** | Skip.                                     |


**Second screen:**


| Option                               | What to do         |
| ------------------------------------ | ------------------ |
| **+ Create Python Environment**      | **Do not choose**. |
| **Python 3.12.x …** `/usr/local/...` | **Choose this**.   |


Why so many Pythons? Codespace lists every Python it finds. Prefer `/usr/local/`.

---
## What happens next

- Continue with `W01` **Python basics** (and **V1** vibe lab) when your instructor adds those notebooks.  
- Each later week: **Sync fork** → Codespace → work → **Commit + Push** → **Stop**.  
- Weekly labs are **practice** (not weekly Moodle uploads). The **individual case study** is still submitted on **Moodle**.

---

## Privacy note

Do not share your password, 2FA codes, or recovery codes. Instructors will never ask for your password.
