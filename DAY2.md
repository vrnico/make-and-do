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

### The prompts

**Spend the first five minutes on your own, then use these.** In that order. An AI that hands
you ten assumptions gives you ten things you don't believe, and you can't test a bet you never
made.

**A · What did I miss** *(the main one)*

```
Here's my project, and here are the assumptions I've written down so far.

The project: [paste]
My assumptions: [paste your list]

I'm sorting these into three layers:
  PROJECT   - is it possible, does anyone want it, is it interesting
  BUILDER   - my skills, my time, what I'm expecting AI to do for me
  MACHINE   - my computer, my tools, whether I can get at and keep my own code

Tell me which layer I've under-thought, and give me five assumptions I
have NOT written down that belong in it. Phrase each one as a claim that
could turn out false, not as a question.

Be blunt. If my list is all technical and I've assumed without checking
that anyone wants this, say so plainly.
```

**B · If the page is blank** *(interview mode)*

```
I'm building this over the next two weeks: [paste]

Interview me to surface the assumptions I'm making without noticing.
Ask ONE question at a time and wait for my answer before the next one.
Ten questions, roughly evenly split across three areas: the project
itself, me as a builder, and my computer and tools.

Don't summarise, don't reassure, and don't offer solutions. Just ask.
At the end, list the assumptions my answers revealed, in my own words
where you can.
```

**C · The machine layer** *(nobody knows how to introspect on this one)*

```
Here's my setup:
  Computer: [e.g. 2019 MacBook / Chromebook, can't install anything /
             Windows laptop, no admin rights]
  Where my code lives: [local folder / GitHub / Replit / I don't know]
  What I build with: [Claude Code / Cursor / ChatGPT + copy-paste / VS Code]
  How I get back to a working version if something breaks: [git / I don't]

What am I assuming about this setup that could cost me days in a two-week
sprint? Include the boring failure modes people don't think about until
they happen.

For each one, tell me whether it's cheap or expensive to fix, and whether
I should fix it now or design around it.
```


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

### The prompts

**Rank it yourself first.** These check your ranking and shrink your test. They don't do it for you.

**A · Check my ranking** *(the sort is the part people get wrong)*

```
Here are the assumptions my project depends on, ranked by what it would
cost me to be wrong:

[paste your list in your order]

Two questions.

1. Did I actually rank by cost of being wrong, or did I slip into
   ranking by how LIKELY each one is? Point out any I've placed low
   because it feels unlikely, when being wrong about it would end the
   project.

2. Push back if the one I've put at the top is the comfortable one
   rather than the dangerous one. The comfortable one is usually
   technical and specific. The dangerous one is usually about whether
   anyone wants this, or about how long things actually take.

Be blunt. I'd rather find out now than on day six.
```

**B · Shrink my test** *(the one everybody needs)*

```
The assumption I'm testing: [paste]
The test I've designed: [paste]

I have TWENTY MINUTES. Not an hour, twenty minutes.

Cut this down until it fits. Strip out anything that isn't directly
answering the question: no interface, no styling, no error handling,
no setup I could fake, no data I could hardcode.

Then tell me:
  - what the twenty-minute version actually is, step by step
  - what result would mean the assumption is FALSE
  - what I'm giving up by shrinking it this far, and whether that
    matters for what I'm trying to learn

If you don't think this can be tested in twenty minutes at all, say so
and tell me what the smallest honest first step is instead.
```

**C · This one feels untestable** *(for "will anyone want it")*

```
I'm trying to test this assumption and I can't work out how:

[paste the assumption]
The project: [paste]

It feels untestable to me, which probably means I'm imagining a big
formal test.

Give me three cheap, unglamorous ways to get evidence on this in under
an hour today. Things like: showing one person a mockup and watching
what they do, posting one sentence somewhere and seeing if anyone
replies, searching for whether the thing already exists and nobody uses
it, or phoning someone and asking.

For each, tell me what answer would count as the assumption FAILING.
Don't suggest surveys or interviews with more than one person.
```

---

## Exercise 3 · Build it and run it · 20 min

**Build the test and run it.** Not the feature. The ugliest thing that answers the question.

**Twenty minutes is deliberately not enough to build something good.** If your test doesn't fit
inside it, the test is too big, and that on its own is worth knowing.

You are not building today. **You are finding out.**

Write down what happened while it's fresh.

→ back to **`02-RISK.md`**

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

## Build log · 5 min, in class

One paragraph: **what you tested, what happened, what you decided.**

We do this on the clock, in the room, because as homework it never happens. In two weeks it's
the only record of what this actually took.

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
