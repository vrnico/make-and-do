# Make and Do

**Build one thing until it works without you in the room.**

Monday–Thursday, 9:00–10:30 Pacific. This repo is the handbook — each day's page appears here
the morning of it. You read it; your work stays on your own machine.

**→ [Day 1 · Scope down](DAY1.md)**
**→ [Day 2 · Kill the riskiest part](DAY2.md)**

**→ [All the prompts, in one place](PROMPTS.md)**

---

## Your project

**You work locally.** Nothing you make goes in here. Your project lives on your machine, and by
the end of it, in your own repo.

Take a copy of the scaffold once:

```bash
git clone https://github.com/vrnico/make-and-do-template.git my-project
cd my-project
```

**No git installed?**
[**Download the ZIP**](https://github.com/vrnico/make-and-do-template/archive/refs/heads/main.zip)
— one click, no account. On Windows, right-click → **Extract All**; don't work inside the zip
preview or your edits won't save. Rename the unzipped folder from `make-and-do-template-main`
to whatever your project is called.

**Can't install anything at all?** Chromebook, work laptop, no admin rights — you're not blocked.
Open [the template](https://github.com/vrnico/make-and-do-template) → **Use this template** →
**Create a new repository**, then **press the `.` key** on your new repo. That's a full VS Code in
your browser, and you commit from the Source Control panel. Nothing installed.

**Or skip all of it.** Put the answers in a single text document — Notes, Google Docs, anything —
and carry on. **The exercises are the sprint.** GitHub is a tool we're introducing alongside it,
not a gate you have to clear first.

Your actual project goes in that same folder, in whatever shape it wants — code, a Unity
project, audio stems, one `index.html`. The markdown files are the record; the rest is the work.

---

## Making it yours

If you **cloned**, git still thinks the files belong to the class. Cut that link by **deleting the
hidden `.git` folder** — turn on "show hidden files" in your file explorer and delete it. That
works identically on every machine, which the shell commands do not: `rm -rf .git` is macOS/Linux
only and does nothing useful in Windows PowerShell.

If you took the **ZIP**, there's no git in there at all. Skip straight to:

```bash
git init
git add -A && git commit -m "day 1"
```

Then, in VS Code: **Source Control** → **Publish to GitHub**. One button — it makes the repo,
connects it, and pushes. The
[template's README](https://github.com/vrnico/make-and-do-template#making-this-your-own-repo)
has the by-hand version if you want it.

**Nothing in the class hour depends on any of this working.** If it fights you, bring it to the
Shipping Software hour — that's the hour built for it.
