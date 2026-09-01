# Prompts

Every paste-in prompt from class, in one place. Copy, fill the brackets, run.

**One rule for all of them: do five minutes on your own first.** These are built to audit your
thinking, not replace it. An AI that hands you ten assumptions gives you ten things you don't
believe, and you cannot test a bet you never actually made.

- [Day 2 · Ten assumptions](#day-2--ten-assumptions)
- [Day 2 · Sort, circle, design the test](#day-2--sort-circle-design-the-test)
- [Day 2 · Run the test in 15 minutes](#day-2--run-the-test-in-15-minutes)

---

## Day 2 · Ten assumptions

### A · What did I miss

*The main one. Write your list first, then get it audited.*

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

### B · If the page is blank

*It interviews you instead of answering for you.*

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

### C · The machine layer

*Nobody knows how to introspect on this one alone.*

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

## Day 2 · Sort, circle, design the test

**Rank it yourself first.** The sort is the part people get wrong, and it's the part worth
arguing with a robot about.

### A · Check my ranking

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

### B · Already in a Claude session?

*If it just built your list, it has the context. Use this instead.*

```
Take the list you just gave me and rank it by cost of being wrong, not
by likelihood.

Then tell me honestly: is my top one the comfortable assumption or the
dangerous one? The comfortable one is usually technical and specific.
The dangerous one is usually about whether anyone wants this, or how
long things really take.

If an assumption at the top can't be falsified by anything I could
actually do this month, say so and move it down. I need one I can get
evidence on.
```

---

## Day 2 · Run the test in 15 minutes

**The one to use.** Give it your top three, not your top one, so it can pick something you can
actually get evidence on inside the block.

```
Here are my top 3 assumptions, in the order I ranked them:

1. [paste]
2. [paste]
3. [paste]

The project: [one line]

I have 15 MINUTES. Pick whichever of the three I can actually get real
evidence on in that time, and tell me why you picked it over the other two.

Then write the smallest thing that answers it. Hardcode everything. One
input. No interface, no styling, no error handling, no setup I could fake.

Tell me what result would mean that assumption is FALSE.

If none of the three can be tested in 15 minutes, say so and give me the
smallest honest first step on number 1.
```

### If it says your test needs other people

**Read this before you accept that.** In class, the test that came back was *"get a stranger to
play it"*, which sounds impossible in fifteen minutes. There were fifteen people in the room at
the time.

**We make risk-avoiding assumptions too.** "That test is too hard" is itself a bet, and it's
usually the one protecting the assumption you least want to look at.

Ask it this:

```
You've told me this test needs other people, or more time than I have.

Before I accept that: what's the version of this test I could run in the
next 15 minutes using only people and things already in front of me right
now? Assume I have access to a room of other builders, my own phone, and
the internet.

If the honest answer is that it genuinely can't be shrunk, say so plainly
and tell me what the smallest first step is instead.
```
