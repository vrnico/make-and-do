# Prompts

Every paste-in prompt from class, in one place. Copy, fill the brackets, run.

**One rule for all of them: do five minutes on your own first.** These are built to audit your
thinking, not replace it. An AI that hands you ten assumptions gives you ten things you don't
believe, and you cannot test a bet you never actually made.

- [Day 2 · Ten assumptions](#day-2--ten-assumptions)
- [Day 2 · Sort, circle, design the test](#day-2--sort-circle-design-the-test)
- [Day 2 · Run the test in 15 minutes](#day-2--run-the-test-in-15-minutes)
- [Day 3 · Draw the path, by hand](#day-3--draw-the-path-by-hand)
- [Day 3 · Build the empty steps](#day-3--build-the-empty-steps)
- [Day 3 · Somebody else walks it](#day-3--somebody-else-walks-it)

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
play it"*, which sounds impossible in fifteen minutes. **patrick firefly** pointed out that there
were fifteen potential playtesters sitting in the call at the time.

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

---

## Day 3 · Draw the path, by hand

**There is no prompt for this one.** You are the only person who knows what somebody is supposed
to do with your thing, and a path you did not write is an ending you will spend Thursday
defending to a stranger.

### The one exception · if the page is blank

*It interviews you. It does not answer for you.*

```
I'm building this over the next two weeks: [paste]

I can't work out what the first step of it is. Interview me until I can
say the path out loud myself.

Ask ONE question at a time and wait for my answer before the next one.
Work in this order:
  1. what a person is doing right before they encounter this
  2. what the very first thing they see or type is
  3. what one thing happens
  4. how they know it worked
  5. how it ends

Do NOT summarise, do NOT reassure, do NOT suggest features, and do NOT
write my path for me.

At the end, give me back my path as a numbered list, in my own words where
you can, and tell me which steps I never actually answered.
```

---

## Day 3 · Build the empty steps

**This is the block where the machine earns its place**, and it works on what you wrote by hand
in exercise 1. Run them in this order.

### A · Audit my path

*Start here. Your steps go in, an audit comes back. It is not allowed to rewrite them.*

```
I have written the end-to-end path for my project as a numbered list of
steps. Your job is to AUDIT that path. Do NOT rewrite it for me and do NOT
design my project.

The project, in one sentence: [paste]
My path: [paste your numbered steps, with HAVE / GAP / LATER marked]

Check it against one definition only: a walking skeleton is a tiny
implementation that performs a small end-to-end function, start to finish,
in its ugliest possible form.

Give me:

MISSING STEPS
Any step a real person would hit that I have not written down. Name each
one and say where in my list it belongs.

IS THERE AN ENDING
Does my path actually end, or does it just stop? If a stranger reached my
last step, would they know they were finished?

STEPS THAT ARE SECRETLY TWO STEPS
Anything I have written as one step that is really several. This is where
skeletons break.

STEPS THAT ARE ALREADY POLISH
Anything on my list that is not needed for the path to connect. Be blunt.
If I have written "style the page" as a step, say so.

TOO MANY
If I have more than seven steps, tell me which to cut for today and which
to bring back later.

Do NOT add features. Do NOT suggest anything that would make this better.
Only tell me whether the path connects, and where it doesn't.
```

### B · Sequencing or avoiding

**The one that matters today.** It is Day 2's finding pointed at Day 3's list. "I'll do that
later" is going to sound completely reasonable to whoever says it, which is exactly the problem.

```
Here is my end-to-end path, and here are the steps I decided to leave for
later today.

My path: [paste the numbered steps]
The steps I marked LATER: [paste]
Why I marked them later, in my own words: [paste]

Yesterday I learned that "that's too hard" can itself be an untested
assumption. Pressure-test my LATER list against that.

For each step I marked LATER, give me:

SEQUENCING OR AVOIDING
Is this genuinely work that has to come after other work, or am I routing
around the part I least want to look at? Say which, and why. Be blunt and
do not soften it.

WHAT THE PATH LOSES
What can a person NOT do while that step is a hole? If the answer is "reach
the end", say that first.

THE CHEAPEST FAKE
One line. The dumbest thing that could sit in that slot today so the path
connects. A hardcoded value, a button that just goes to the next screen,
one instead of many, a still image instead of the real thing.

Do NOT build the real version of any of these steps. Do NOT tell me the
fake is good enough permanently, it is a placeholder and I am writing it
down as one.

If a step genuinely cannot be faked and has to be built, say so plainly and
tell me the smallest real version of it.
```

### C · My steps as one file

*Only if your thing runs in a browser.*

It renders the path **you** wrote and is not allowed to add to it. **The last section is the
point:** everything it had to guess at is a part of your path you have not thought through yet.

The file it gives you goes at the top level of your repo, and it is the exact file GitHub Pages
serves. That is your link for tomorrow.

```
Here is the path I wrote for my project, in my own words:

[paste your numbered steps exactly as you wrote them]

Turn MY steps into one file called index.html. That is the whole job.

RULES
Use only the steps I wrote. Do NOT add steps, screens, features or copy
I did not write. Where a step of mine is vague, put my own words on the
screen verbatim rather than inventing something better.
No CSS beyond what it takes to be readable. No frameworks, no libraries,
no build step, no images, no fonts.
ONE file. It has to work by double-clicking it, with no internet.
Every screen needs a way to the next one, and the last screen needs a way
back to the start.

GIVE ME

THE FILE
One complete index.html I can copy straight out. Nothing to install.

WHAT'S FAKE IN IT
Every hardcoded value, dead button and placeholder you put in, as a list
I can paste straight into my fake list.

WHAT I DIDN'T SPECIFY
Everything you had to guess at because my path did not say. Be specific.
These are the steps I have not actually thought through yet.

Do NOT make it look good. Do NOT add a feature because it would be easy.
If my path has three steps, the file has three screens and no more.
```

---

## Day 3 · Somebody else walks it

**This block is people, not prompts.** You post yours in the room, you open somebody else's, you
walk it, and you say nothing. You cannot walk your own path honestly because you already know
where everything is.

### Only if nobody has walked yours yet

*A fallback for no partner, or for a thing that genuinely cannot be posted.*

```
I am going to walk you through my project one step at a time, as if you
were a stranger using it. Your job is to catch the moment the path stops.

Rules for you:
  - ask ONE question after each step, then wait for me
  - the two questions are always: what does the person SEE, and what do
    they DO next
  - stop me the moment I describe something that is not actually built
  - say "that step does not exist" out loud when it happens
  - do NOT suggest features, do NOT offer to write anything for me, and
    do NOT encourage me

Start by asking what the very first thing a person sees is.

At the end, give me:

WHERE IT STOPPED
The first step where the path broke, and what broke about it.

WHAT I DESCRIBED THAT ISN'T BUILT
Everything I narrated as though it existed when it doesn't.

WHAT A STRANGER WOULD HAVE HAD TO ALREADY KNOW
Anything I explained to you that the thing itself does not explain. This
is tomorrow's list.
```
