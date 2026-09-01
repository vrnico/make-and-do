# Day 2 · Tuesday · Kill the Riskiest Assumption

**Every project is a stack of bets.** You're betting somebody wants this. You're betting you can
build it. You're betting your laptop will cooperate. Most of those bets are fine. One of them
isn't, and you can't see which one, because from where you're standing it looks like common
sense.

Today you find that one and you test it, while testing it is still cheap.

By the time you leave: **you can say in one sentence whether the scariest thing about your
project is true.**

---

## First · where your answers live

**Three lanes. All three are fine, and nobody is behind.**

**Git working?** You're in your project folder. Keep going.

**It isn't?** Put it aside. One text document, Notes, Google Docs, anything. Put the answers in
it and carry on. **The exercises are the sprint.** GitHub is a tool we're introducing alongside
it, not a gate you have to clear first.

**Can't install anything at all?** Chromebook, work laptop, no admin rights. You're not blocked,
you're on a different route:
[the template](https://github.com/vrnico/make-and-do-template) → **Use this template** →
**Create a new repository**, then press the **`.`** key on your new repo. Full VS Code in the
browser, commit from the Source Control panel, nothing installed.

Still stuck? [The setup walkthrough](https://www.youtube.com/watch?v=3jjcnuR1m9c) covers all of
it, and the Shipping Software hour is for exactly this. **Not the class hour.**

---

## What kind of builder are you?

Two axes. Across the bottom, **access**: what your machine will actually let you do. Up the
side, **appetite**: how much you want to be in the guts of it.

| | | Watch this bet |
|---|---|---|
| **Machinist** · more access, wants the guts | Doc Brown, Shuri | *"I have time to do this properly."* |
| **Assembler** · more access, wants it to work | Han Solo, Sayid | *"The service will still be there, and I could swap it."* |
| **Cartographer** · less access, wants the guts | Hermione, Jesse Pinkman | *"I have time to learn this AND fight my machine."* |
| **Director** · less access, wants it to work | Don Draper, Shiv Roy | *"The tool will keep doing this for me."* |

**Neither axis is better and there is no corner where the good programmers live.** Han Solo
flies the fastest ship in the galaxy and has no idea how the hyperdrive works. Hermione wants to
understand everything and has a library card, not a lab. **Wanting the guts and being able to
get at them are two different things.**

You build a certain way, on a particular machine, making a particular thing. Those three facts
together produce a bet you can't see.

---

## Exercise 1 · Ten assumptions · 15 min

**Write everything. Judge nothing.** You're not solving anything, you're emptying your head onto
a page.

**PROJECT** · what are you assuming about the thing?
Someone wants this. It's interesting to encounter. The data or API exists. The hard part is
possible at all. Your scope fits in eight days.

**BUILDER** · what are you assuming about yourself?
You'll figure out the code. AI handles that part. You can debug it when it breaks. You have time
to learn the unfamiliar bits.

**MACHINE** · what are you assuming about your setup?
You can get at your own code. Your AI tool works on this project. Things install. You have a way
back when something breaks. The platform won't become a box you can't get out of.

> **That third one is not a beginner category.** Yesterday, setup ate a third of this class. If
> your machine is the thing most likely to sink you, that is a finding, and it belongs on the
> list next to everything else.

Aim for ten. Bad ones count.

→ open **`01-BETS.md`**

---

## Exercise 2 · Sort, circle, build · 15 min

Two columns next to each bet: **how sure am I**, and **what happens if I'm wrong**.

**Then sort by the second one.** Not the first.

You do not rank these by likelihood. You rank them by **cost of being wrong**. Something with a
one-in-ten chance of ending the project beats something certain to annoy you for an afternoon.
Ranking by likelihood feels rigorous and mostly keeps you busy at the comfortable end of the
list.

**Circle the top one.** Then design the smallest test: something you could run in under an hour
that would genuinely change your plan if it failed.

**The test, not the feature.** Hardcode everything. One input. No interface.

> **The trap, and it catches everyone.** You will want to test the assumption you're confident
> about, because testing the frightening one risks ending the project on a Tuesday. Test the
> frightening one. If circling it didn't feel bad, you probably picked wrong.

→ open **`02-RISK.md`**

### The prompt

```
Here's what I'm building and my plan for the next two weeks:
[paste project + demo-ready definition + build plan]

List every assumption this plan depends on, across three layers:
the PROJECT (does anyone want it, is it possible, is it interesting),
the BUILDER (my skills, my time, what I'm expecting AI to do), and
the MACHINE (my computer, my tools, my ability to get at and keep
my own code).

For each: state it as a falsifiable claim, rate my likely confidence,
estimate the cost of testing it now, and describe what happens to the
sprint if it turns out false.

Sort by cost-of-being-wrong, highest first. Then design the cheapest
possible test for the top one, something I could run in under an hour
today, that would genuinely change my plan if it failed.

Push back if the top assumption I'd naturally test is the comfortable
one rather than the dangerous one.
```

---

## Run it · 26 min

**Build the test and run it.** Not the feature. The ugliest thing that answers the question.

You are not building today. **You are finding out.**

Write down what happened while it's fresh.

---

## The three that kill prototypes

Worth naming, because people almost never guess right about which one they have.

**Technical** · *"this is possible at all, by me, in this time."*

**Experiential** · *"this is actually interesting to encounter."* The most commonly ignored and
the most commonly fatal. **A thing can work perfectly and be boring, and no amount of polish
fixes boring.**

**Effort** · *"this takes the time I think it takes."*

---

## Today's checkpoint

**The riskiest assumption is tested, and you can say in one sentence whether it held.**

> **"I don't know yet" means the test was too big.** That's the only wrong answer available
> today, and it's a scoping problem, not an effort problem. Cut the test in half and run the
> smaller one.

**If it failed, change the plan today.** That's what the day is for and it is a success, not a
setback. A project that dies on a Tuesday cost you two days. The same project dying in month
five costs you the runway.

---

## Build log

One paragraph before you close the laptop: **what you tested, what happened, what you decided.**

→ open **`log/day2.md`**

---

## After class · Shipping Software hour

**Write down what you'd do if the assumption fails.** Even if it held today. Having the fallback
written removes most of the reason to avoid testing the scary thing next time, and it takes five
minutes.

**And if the tooling beat you today, this is the hour.** Bring the exact error and what machine
you're on. Two things worth knowing before you come:

- **`rm -rf .git` is a macOS and Linux command.** On Windows PowerShell it does nothing useful.
  Easier than remembering either: **delete the `.git` folder in your file explorer.** Turn on
  hidden files to see it. Same result, no shell.
- **You don't need a terminal at all.** VS Code's **Source Control** panel does Initialize
  Repository → commit → **Publish to GitHub** in three clicks, and it handles the login.

---

**Tomorrow:** the walking skeleton. A thin, ugly, end-to-end version of the whole thing, start to
finish, placeholder everything. It's the only structure that tells you the truth about your scope
while there's still a week to do something about it.

Bring what your test told you.
