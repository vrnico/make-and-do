# Day 2 · Tuesday · Kill the Riskiest Part

**You've named the thing. Today you find the part most likely to kill it — and you find out
cheaply, on a Tuesday, while finding out is still free.**

A project that dies today cost you two days. The same project dying in month five costs you the
runway. That's the whole trade, and it's why this is Day 2 and not Day 7.

By the time you leave: **the one part only you could build is named, and you can say in one
sentence whether the scariest thing about it actually works.**

---

## First — where your answers live

**Three lanes. All three are fine, and nobody is behind.**

**If git's working** — you're in your project folder. Keep going.

**If it isn't — put it aside.** One text document. Notes, TextEdit, Google Docs, a Word file, the
back of an envelope. Put the answers in it and carry on:

> *"If you just can't even with the GitHub stuff, put it aside for now, and make a single text
> document with answers to these questions."*

That's the ruling and it stands for the whole fortnight. **The exercises are the sprint. GitHub
is a tool we're introducing alongside it, not a gate you have to pass first.**

**If your machine can't run the tools at all** — Chromebook, work laptop, no admin rights — you're
not blocked, you're on a different route, and it's a route plenty of working developers use:

1. Go to [the template](https://github.com/vrnico/make-and-do-template) → green **Use this
   template** → **Create a new repository**. Free GitHub account, no install.
2. On *your* new repo, **press the `.` key.**
3. That's a full VS Code, in your browser. Edit the files, then commit from the Source Control
   panel on the left.

Nothing to install, nothing to unzip, and you own the repo at the end of it. If you need to
actually *run* code and can't install anything, say so in chat and we'll get you on something
browser-based — that problem is solved, it just isn't solved by a zip file.

---

## Still stuck on "what they can't do"?

It was the most-asked question yesterday, so here it is properly. **It's deliberately open, and
there are at least four honest readings.** Pick whichever one is true for your project:

| | |
|---|---|
| **User repellent** | Who this is *not* for, by design. You're keeping someone out on purpose. |
| **A technical guide** | The boundary of what you're going to build. What's out of scope. |
| **An impasse** | Where your build is genuinely stuck right now. An honest one. |
| **Foundational** | Something the user *should not* be able to do, and never will. |

> *"This is where our abstract interpretation as artists comes in handy… Yes and all of the
> above."*

If yours is still blank, ask which of those four the question is even asking about for you. The
answer is usually obvious once you've picked the reading.

**No project yet?** That's four of us and it's fine. Write the four-part answer for the worst idea
you've got — you need something to run today's exercises against, and you can swap it Wednesday.
What you can't do is spend the fortnight choosing. **If you're stuck between two:** *which one's
buyer can you name fastest?* "Buyer" means the person who'd miss it if it vanished — money is one
kind of answer, not the only one.

---

## Exercise 1 · The part only you could build · 10 min

**Every component of what you're making sits somewhere between "nobody has done this" and "you
can get it free in five minutes."**

| Stage | |
|---|---|
| **Genesis** | Genuinely novel. Nobody's done this. |
| **Custom** | People build this, but bespoke every time. |
| **Product** | You can buy it off a shelf. |
| **Commodity** | Free, everywhere, boring. |

**The rule: build only what's in Genesis. Buy, borrow or fake everything else.**

rpbostick put this better than the handbook did, yesterday at 10:34:

> *"95% of what we have is already in this path. Our computer, our OS, our basic software, our
> browser, and all the other tools we're using right now. Someone else built them. So for as much
> else as possible, do the same thing. Don't rebuild workable, affordable things that already
> exist."*

List the parts of your thing. Stage each one. Then **circle the single Genesis component** — the
one where, if you only shipped that, it would still recognisably be the idea.

Expect this to sting a bit. Most projects turn out to have exactly one Genesis component and a
long tail of things you could buy this afternoon. **That's a good result, not a bad one** — it's
the difference between a fortnight spent on the part that's yours and a fortnight spent on a
login form.

→ open **`01-MAP.md`**

### The prompt

```
I'm building the following in two weeks. Break it into components and place
each on a Wardley evolution axis: Genesis (novel), Custom (bespoke),
Product (off-the-shelf), Commodity (free/ubiquitous).

The project: [paste]
What I think makes it distinctive: [paste]

For each component: which stage, and if it's Product or Commodity, name two
specific existing things I could use instead of building it. Then tell me
which single Genesis component is the actual heart of this project — the
one where, if I only shipped that, it would still be recognisably the idea.
Be blunt if what I called distinctive is actually Custom.

Then: for that one Genesis component, what has to be TRUE for it to work
at all? List the assumptions as falsifiable claims, sorted by what it
would cost me to be wrong. Design the cheapest test for the top one —
something I could run in under an hour today.
```

---

## Exercise 2 · What has to be true · 10 min

Look at the component you circled and ask: **what has to be true for that to work at all?**

Write the assumptions down as things that could be *false*. Then rank them by **cost of being
wrong**, not by likelihood.

For a prototype the fatal one is almost always one of three, and people rarely guess right about
which they have:

1. **Technical** — *"this is possible at all, by me, in this time."*
2. **Experiential** — *"this is actually interesting to encounter."* The most ignored, and the
   most commonly fatal. A thing can work perfectly and be boring, and no amount of polish fixes
   boring.
3. **Effort** — *"this takes the time I think it takes."*

Then design **the cheapest possible test** for the top one. Under an hour. Something that would
genuinely change your plan if it failed.

> **The trap:** you will want to test the assumption you're confident about, because testing the
> frightening one risks ending the project on a Tuesday. Test the frightening one. That's what
> today is for, and a project that ends today is a *result*.

→ open **`02-RISK.md`**

---

## Heads down · 15 min

**Build the test. Not the feature.** The smallest thing that answers the question.

Hardcode everything. One input. No interface. If the question is "can I get this data at all,"
the test is a script that prints it to a screen once. If the question is "is this interesting,"
the test is showing one person a mockup.

You are not building today. You are finding out.

---

## Exercise 3 · Run it · 15 min

**Run the test and write down what happened.** One sentence: did it hold, or not?

If it failed — **change the plan today.** That is what the day is for and it is a success, not a
setback. Write what you're doing instead.

If it held — write what that lets you stop worrying about, and what the *next* riskiest thing is.

Then one line: **tomorrow, this will exist.** A checkpoint is a thing that either **exists** or
**doesn't** at the end of a day. Not *"work on the map"* → **"one pin appears on a page."**

→ open **`02-RISK.md`**

---

## Today's checkpoint

**You can say in one sentence whether the riskiest thing held.**

> **"I don't know yet" means the test was too big.** That's the only wrong answer available today,
> and it's a scoping problem, not an effort problem. Cut the test in half and run it again.

---

## Build log

One paragraph before you close the laptop: **what you tested, what happened, what you decided.**

→ open **`log/day2.md`**

---

## After class · Shipping Software hour

**Write down what you'd do if the assumption fails.** Having the fallback written removes most of
the reason to avoid testing it, and it takes five minutes.

**Take one Product or Commodity component off your list** — find the thing you'll use instead of
building it. Every one you retire buys back build hours.

**And if the tooling beat you today, this is the hour.** Not the class hour. Bring the exact error,
we'll sort it. Two things worth knowing before you come:

- **`rm -rf .git` is a Mac/Linux command.** On Windows PowerShell it does nothing useful. Easier
  than remembering either: **just delete the `.git` folder in your file explorer.** Turn on hidden
  files to see it. Same result, no shell.
- **You don't need a terminal at all.** VS Code's **Source Control** panel does Initialize
  Repository → commit → **Publish to GitHub** with three clicks, and it handles the login for you.

---

**Tomorrow:** the walking skeleton. A thin, ugly, end-to-end version of the whole thing —
start to finish, placeholder everything — because that's the structure that tells you the truth
about your scope while there's still a week to act on it.

Bring what your test told you.
