# Day 1 · Monday · Scope Down

**The first scope is always too big.** Today it gets smaller — and the framework tells you
*which parts* to cut rather than just cutting proportionally.

By the time you leave: **one project named, a demo-ready definition written, one genesis
component identified, and eight binary checkpoints.**

---

## Exercise 1 · The one thing · 10 min

Write it as one paragraph.

1. **Name it.**
2. **What do they SEE the first time?**
3. **What can they DO?**
4. **What can they NOT do?**

**Part 4 is the one that matters.** It's the only part you can't quietly move on day six — which
is exactly why you're writing it on day one, before there's anything to defend it against.

> **Holding two projects?** You won't be able to write this. That's not you failing the exercise,
> that *is* the exercise. Pick the one you thought of first, not the sensible one.

→ `_TEMPLATE/00-SCOPE.md`

---

## Exercise 2 · The map · 10 min

**Every component of what you're making sits somewhere between "nobody has done this" and "you
can get it for free in five minutes."** Simon Wardley's idea, cut down to the one question that
matters this fortnight.

| Stage | |
|---|---|
| **Genesis** | Genuinely novel. Nobody's done this. |
| **Custom** | People have built this, but bespoke every time. |
| **Product** | You can buy it off a shelf. |
| **Commodity** | Free, everywhere, boring. |

**The rule: build only what's in Genesis. Buy, borrow or fake everything else.**

The thing that makes your project yours is almost always one small Genesis component. People
routinely spend their fortnight hand-rolling an auth system, a level editor or a page layout
they could have taken off a shelf, and run out of time before reaching the part nobody else
could have made.

Circle **one** genesis component: the one where, if you only shipped that, it would still be
recognisably the idea.

→ `_TEMPLATE/01-MAP.md`

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
```

---

## Heads down · 15 min

**Start the genesis component.** Not the repo, not the folder structure, not the build pipeline.
The scary bit.

It's going to be bad. You're not making it work — you're finding out what it's like.

---

## Exercise 3 · Eight days · 15 min

One checkpoint per class day. **A thing that either exists or doesn't** at the end of it.

Not *"work on the renderer"* → **"the renderer draws one frame."**
Not *"make progress on audio"* → **"one sound plays when you click."**

A percentage-complete estimate on creative work is a wish. It stays at 80% for nine days and
then the sprint ends. **A binary checkpoint is the only kind that tells you you're behind while
there's still time to do something about it.**

Two are already filled in — both Thursdays are show days, and that isn't negotiable.

Then name **the riskiest part**, and put it early. Whatever is most likely to not work is the
thing you do first, not the thing you save. Most prototypes that fail, fail because the hard
part was left for last.

→ `_TEMPLATE/02-CHECKPOINTS.md`

---

## Today's checkpoint

**The riskiest part is identified in writing, and you have started it.** Not planned it. Started
it.

> **Watch for this in yourself.** Somebody will have spent the whole hour on setup — repo,
> tooling, project structure, a build pipeline. That feels like progress and is the most reliable
> way to lose a fortnight. **The genesis component gets touched on day one or the sprint is
> already in trouble** — and the person doing it won't notice, because setup is genuinely
> satisfying and genuinely necessary and entirely beside the point right now.

---

## Build log

One paragraph before you close the tab: **what you made, what broke, what you decided.**

→ `_TEMPLATE/log/day1.md`

---

## After class · Shipping Software hour

**Take one Product or Commodity component off your list** by finding the thing you'll use
instead of building it. Every one you retire buys back build hours.

And if you want your folder in here properly, that's the hour to do it. Not during class.

---

**Tomorrow:** the riskiest assumption, and killing it cheaply before it costs you a fortnight.
Bring today's checkpoint and whether you hit it.
