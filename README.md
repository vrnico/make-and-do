# Make and Do

**A fortnight. Eight class days. One thing that runs by the end of it.**

Monday–Thursday, 9:00–10:30 Pacific, two weeks. This repo is where class lives — the day's
exercises, the prompts, and everybody's sprint record.

**Every morning, open the day's file.** That's the whole system.

---

## The eight days

| | | | What exists by the end of it |
|---|---|---|---|
| **[Day 1](DAY1.md)** | Mon | **Scope down** | One project named, demo-ready written, one genesis component, eight checkpoints |
| **Day 2** | Tue | Kill the riskiest assumption | The riskiest assumption is tested and you can say in one sentence whether it held |
| **Day 3** | Wed | The walking skeleton | The end-to-end path runs, however ugly |
| **Day 4** | Thu | **Show day** | Three people have used it without you talking, and you wrote down what they *did* |
| **Day 5** | Mon | Cut against what you saw | The backlog is cut to what fits, and the killed list is visible |
| **Day 6** | Tue | Make it legible | Someone starts it and reaches the first interesting moment without you saying a word |
| **Day 7** | Wed | Honest faking, and harden | It runs twice from cold, and the fake inventory is written |
| **Day 8** | Thu | **Show day** | Shown, working, driven by someone else — and a next-sprint decision with a number on it |

*Day files appear the morning of. Day 1 is up.*

---

## What the fortnight produces

**A prototype, a demo, a playable slice, an artist's proof — something real enough that it
works without you in the room.**

Not a finished product with a checkout button. That isn't reachable in two weeks and pretending
otherwise crushes the idea under impossible scope. Selling it is the next sprint's job.

---

## The four rules

**1 · Every day has a binary checkpoint.** Not "worked on the renderer" — *"the renderer draws
one frame."* A thing that either exists or doesn't by the end of the day. Percentage-complete is
a wish; it sits at 80% for nine days and then the sprint ends.

**2 · Thursdays are show days.** Someone who isn't you drives it, and you don't talk while they
do. The gap between the thing in your head and the thing on the screen is only visible in
somebody else's hands — and only if you stay quiet long enough to see it.

**3 · Build only the genesis part.** Buy, borrow or fake everything else. The thing that makes
your project yours is almost always one small component, and the reliable way to lose a fortnight
is to hand-roll the parts you could have taken off a shelf.

**4 · One build log a day.** One paragraph: what you made, what broke, what you decided. Five
minutes. In two weeks it's the only record of what this actually took.

---

## If something slips

In priority order. These are the ones that cost you the sprint:

1. **Day 3's walking skeleton.** Without an end-to-end path there's nothing to show on either
   Thursday, and the sprint fails silently on the last day instead of loudly on the third.
2. **Both Thursdays.** One is recoverable. Zero is not a sprint.
3. **Day 2's assumption test.** Cheap on Tuesday of week one. Ruinous in month five.
4. **Day 8's four questions.** The observed timeline is the most durable thing this fortnight
   produces. Get the numbers even if the prototype disappointed.

Everything else is catch-up-able in the Shipping Software hour.

---

## Your project

**You work locally.** Nothing you make goes into this repo — this is the handbook, you read it.
Your project lives on your own machine, and by the end of the fortnight, in your own GitHub repo.

Take a copy of the scaffold once, on Day 1:

```bash
git clone https://github.com/vrnico/make-and-do-template.git my-project
cd my-project
```

**No git installed?** Open
[the template](https://github.com/vrnico/make-and-do-template) → green **Code** button →
**Download ZIP**. Same folder, no account needed. Sort git out in the Shipping Software hour.

Inside it:

```
00-SCOPE.md         day 1 · the one thing + your demo-ready definition
01-MAP.md           day 1 · the four stages + your genesis component
02-CHECKPOINTS.md   day 1 · eight binary checkpoints + the riskiest part
03-FAKES.md         day 7 · what you're faking, and what you'll disclose
log/day1.md …       one paragraph a day
scratch/            yours. gitignored. never leaves your machine.
```

Your actual project goes in that same folder, in whatever shape it wants — a folder of code, a
Unity project, audio stems, one `index.html`. The markdown files are the record; the rest is
the work.

---

## Making it yours

You cloned this repo, so git still thinks the files belong to the class. Cutting that link and
starting your own history is three commands, and it's the **Shipping Software hour**, not the
class hour:

```bash
rm -rf .git
git init
git add -A && git commit -m "day 1"
```

Then an empty repo on GitHub and `git remote add origin …`. The
[template's README](https://github.com/vrnico/make-and-do-template#making-this-your-own-repo)
walks the whole thing.

**Nothing in the 90 minutes depends on any of this working.** If it fights you, bring it to the
Shipping Software hour — that's the hour built for it.
