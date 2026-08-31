# Make and Do

**Build one thing until it works without you in the room.**

Monday–Thursday, 9:00–10:30 Pacific. This repo is the handbook — each day's page appears here
the morning of it. You read it; your work stays on your own machine.

**→ [Day 1 · Scope down](DAY1.md)**

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

Your actual project goes in that same folder, in whatever shape it wants — code, a Unity
project, audio stems, one `index.html`. The markdown files are the record; the rest is the work.

---

## Making it yours

If you **cloned**, git still thinks the files belong to the class — cut that link first. If you
took the **ZIP**, there's no git in there at all, so skip the first line.

```bash
rm -rf .git          # only if you cloned
git init
git add -A && git commit -m "day 1"
```

Then an empty repo on GitHub and `git remote add origin …`. The
[template's README](https://github.com/vrnico/make-and-do-template#making-this-your-own-repo)
walks the rest.

**Nothing in the class hour depends on any of this working.** If it fights you, bring it to the
Shipping Software hour — that's the hour built for it.
