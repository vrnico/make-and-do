# Day 3 · Wednesday · The Walking Skeleton

**Build a thin, ugly version of the whole path before you make any part of it good.**

Not the best feature finished. The entire path, start to end, existing in its worst possible
form. A way in, a thing that happens, a way out.

By the time you leave: **someone can start it and reach the end, without you sitting next to
them.**

**Every prompt from today lives in [PROMPTS.md](PROMPTS.md).**

---

## The framework

Alistair Cockburn, *Crystal Clear*, 2004:

> A walking skeleton is a tiny implementation of the system that performs a small end-to-end
> function. It need not use the final architecture, but it should link together the main
> architectural components.

Two words are doing the work: **tiny**, and **end to end**.

The reason is not tidiness. **A skeleton is the only structure that tells you the truth about
your scope, and it does it while there's a week left.** Building feature by feature, you feel
fine right up until the last day, and then you find out the pieces don't connect and there is
nothing to show. With a skeleton you always have something to show. It just gets better.

If anything in this fortnight slips, this is the number one non-negotiable. Above both show days.
Without an end-to-end path there is nothing to show on either Thursday, and **the sprint fails
silently on the last day instead of loudly on the third.**

---

## The three parts

| | |
|---|---|
| **A way in** | a title card · a page that loads · the command you type |
| **A thing that happens** | one interaction · one result · not the feature set, one instance of it working |
| **A way out** | an ending screen · a result on the page · a close button |

**The way out is the one everybody leaves off**, and it's the one that turns a pile of screens
into a path.

Here is one, built in an afternoon, that is nothing but those three parts:
[foolsday.online](https://foolsday.online). A logo, a left arrow, a right arrow, and a close
button. Nothing on it is finished. All of it connects.

---

## If you can't run anything today

**This is a lane, not a fallback.** A walking skeleton is about whether the path connects, and a
path can connect on a table. Two forms, both of which can be handed to a stranger tomorrow:

**Index cards.** One card per step. On each card, three things: **what they see**, **what they
can do**, **what happens next.** Lay the cards in a row. Then walk it: finger on card one, move
to the end, saying each transition out loud. Wherever you can't say what happens next, that's a
gap, and it is the same gap the code version would have found.

Mark a card **`T`** where you don't know how that step would technically work. **Those cards are
your list, not your failure.** A paper walk finds missing steps and missing endings exactly as
well as code does. The only thing it can't test is whether the hard part is possible, and the
`T` marks are where that question lives.

**Or linked slides.** Google Slides, one slide per screen, hyperlink each button to the slide it
leads to, then hit present. Clickable, walkable, installs nothing, works on a Chromebook, and
you can send a stranger the link tomorrow.

Still fighting your setup? [The setup walkthrough](https://www.youtube.com/watch?v=3jjcnuR1m9c)
covers it, and the Shipping Software hour exists for exactly this. **Not the class hour.**

---

## Exercise 1 · Draw the path · 10 min

**Someone arrives. Something happens. It's over.** Write the steps in between, and number them.

The fewest steps it can be and still be the path. **Over seven and you've written the finished
product**, not the skeleton.

Next to every step, mark it:

- **HAVE** · it exists right now
- **GAP** · it doesn't
- **LATER** · you were planning to skip it today

Most people find they have step three and step five and nothing else. That's the finding, not a
problem.

**And put an end on it.** If your list doesn't end, it isn't a path yet.

→ open **`03-PATH.md`**

### The prompts

**Five minutes on your own first.** Neither of these will draw your path for you, on purpose. An
AI that invents your path invents an ending you don't want, and you spend Thursday defending it
to a stranger.

**A · Audit my path** *(the main one)*

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

**B · I can't name step one** *(interview mode)*

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

## What goes in the gap

Same three layers as Monday and Tuesday. Your gaps sort the same way, and the filler is different
for each.

| The gap | What goes in it today |
|---|---|
| **PROJECT** · the thing is genuinely hard | **Hardcode the outcome.** Type the answer in by hand and move on. |
| **BUILDER** · you don't know how yet | **The dumbest version you do know how to write.** A printed line is a step. |
| **MACHINE** · your setup won't run it | **Paper, slides, a browser tab.** Still walkable, still counts. |

**Keep a list of everything you fake.** Day 7 is an entire class about that list and you will not
remember any of this by next Wednesday.

---

## Later is a hole in the path

Yesterday the class found that **we make risk-avoiding assumptions too.** *"That test is too
hard"* is itself an untested bet, and it's usually the one protecting the thing you least want to
look at.

Today that same bet arrives in a different costume, and this is the one to watch for. **It won't
sound like avoidance. It will sound like sequencing.**

> *I'll do the networking later. I'll do the login later. I'll do the API later. I'll do the
> hard bit once the rest is working.*

Every one of those is a hole, and **the holes are the thing you're building this morning.**

The move is not to build the hard step. The move is to **put its dumbest possible fake in the
path today**, so the path connects, and the hard part becomes an upgrade instead of a gap. A
button that just goes to the next screen. One player instead of four. The answer typed in by
hand. A still image where the real thing goes.

Then write "faked" next to it. That isn't cheating. That's Day 7's homework getting done early.

---

## Exercise 2 · Build the empty steps · 15 min

**Go to the GAP and LATER steps. Not the step that's good.**

Every step must be **reachable from the one before it.** If step four doesn't exist, put in
whatever gets you from three to five.

| | |
|---|---|
| a grey box | a button that just goes to the next screen |
| hardcoded text | one player instead of four |
| a still image | the answer typed in by hand |
| `print("step 3")` | a link straight to the end screen |

**If a step takes you more than a couple of minutes, it's too good.**

> **The one to watch for.** Somebody will spend this hour making one screen beautiful while the
> path doesn't connect, and they will have **the best-looking nothing in the room** by Friday. It
> is almost always the person with the strongest taste, and the instinct that makes their work
> good is the exact instinct sinking their sprint.
>
> Ugly is the assignment for one hour. You get your taste back on Friday, and by then it will
> have something to sit on.

→ back to **`03-PATH.md`**

### The prompts

**A · Is this still polish**

```
I am building the ugliest possible version of one step in my path today.

The step: [paste]
What I plan to build for it: [paste]
What I am building with: [language / engine / tools]

Twenty minutes is the limit for this step. Cut it down.

Give me:

WHAT TO DELETE
Everything in my plan that is not required for this step to CONNECT to the
step before it and the step after it. Styling, error handling, structure I
am adding for later, data I could hardcode, anything I am making reusable.

THE UGLIEST VERSION
What is left after all of that is deleted, in one short paragraph. Not code
unless it is genuinely one or two lines.

CONNECTED OR NOT
Say plainly whether the ugliest version still lets a person get from the
previous step to the next one. That is the only thing this step has to do
today.

Do NOT make it better. Do NOT add anything I did not mention.
If my plan is already the ugliest version, say so in one line and stop.
```

**B · Sequencing or avoiding** *(the one that matters today)*

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

---

## Exercise 3 · Walk it · 15 min

**Start at step one. Go to the end.**

- Touch nothing.
- Explain nothing.
- Fix nothing on the way.

**Where it stops is the gap.** Write down *where* it stopped. Then fix the gap, not the step.

Then **walk it again from the start.** Twice, because the first time you're driving from memory
and you won't notice the things you already know.

→ back to **`03-PATH.md`**

### The prompt

**A · Walk it with me** *(works identically for a paper skeleton, just read the cards)*

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

---

## Today's checkpoint

**Someone can start it and reach the end.**

Not that it's good. Not that it's finished. That somebody can start it and get to the end
**without you sitting next to them.**

If that's true today, tomorrow works. If it isn't, tomorrow is you describing something to three
strangers, which is a much worse Thursday.

---

## Build log · 5 min, in class

→ open **`log/day3.md`**

- **WHAT CONNECTS** · step 1 to step _, end to end
- **WHAT YOU FAKED** · every placeholder, every hardcoded thing, every button that just goes to
  the next screen
- **WHAT BROKE** · where it stopped when you walked it

One paragraph. **The faked list is the one that matters** and it's the one you'll want on Day 7.

Then post it in the Matrix room: your path, however many steps it turned out to be, and a
screenshot of **your end screen.** The end screen is the interesting one, because it's the one
nobody had at nine o'clock this morning.

---

## After class

**Find your three people for tomorrow.** Text them tonight, not in the morning.

Not cohort-mates. **Strangers to the project.** Friends are fine; friends who have already heard
you describe it are not.

Tomorrow you hand it over and say nothing while they use it. Ten minutes each. You write down
what they *do*, not what they say.

---

**Tomorrow:** show day. The first contact with reality, and the day the sprint turns on.

Bring the thing that walks.
