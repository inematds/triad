# [soul.md](http://soul.md) — Hermes template

*A fill-in template for Hermes Agent. Drop your details in. Hand to Hermes. Reap.*

> 🪶 **How to use this**
>

> Duplicate this page. Replace every italic grey hint with your real answer. Save the filled-out version as `~/.hermes/soul.md` — Hermes will load it on every task. The deeper you fill it in, the more useful Hermes becomes.
>

Hermes works best when it has a deep model of who you are — your business, your money, your routine, your voice. [**Soul.md](http://Soul.md) is where that lives.** The fields below are prompts, not rules. If a section doesn't apply, skip it. If you want to add your own, do.

> 💡 **Be specific.** *"I run a YouTube channel"* is okay. *"I run a YouTube channel about [topic] — [X] subscribers, [Y]× monthly cadence, sponsors land in Stripe under '[entity]'"* is what makes Hermes actually useful.
>

---

## 🧑 Identity

The basics. So Hermes never has to ask twice.

- **Name:** *your full name (e.g. Alex Carter)*
- **Based in:** *city, country · timezone (e.g. Berlin, DE · CET)*
- **Role:** *what you do · how you'd introduce yourself*
- **Public-facing:** *channels you publish on (e.g. LinkedIn, Substack, X)*
- **Brand voice:** *3 adjectives that describe how you write*

## 🎯 Mission & goals

What you're actually trying to build. Hermes uses this to weight every suggestion toward what matters.

- **This year's headline goal:** *One sentence. If you nailed it, the year would be a success. No softeners.* Example: `Launch the SaaS. Hit $20k MRR by December.`
- **The three pillars below it:** *Three concrete focus areas that ladder up to the headline. Each in one line.*
- **What's NOT in scope:** *The shiny distractions you've already decided to say no to. List 3–5.*

---

![The business](https://i.imgur.com/5AsJXe5.jpeg)

The business

## 🏢 The business

Numbers Hermes can reason about. Update these monthly — Hermes will notice if they're stale.

- **Legal entity:** *company name · jurisdiction · structure*
- **Revenue model:** *how you make money (e.g. SaaS subs, agency retainers, courses)*
- **Monthly revenue:** *$X · trend % MoM*
- **Monthly costs:** *$Y · where the money goes*
- **Runway:** *months at current burn if revenue dropped to 0*
- **Bank / payment:** *where the money lives (e.g. Stripe under X Ltd, Wise USD)*
- **Tax year:** *jurisdiction · start month – end month*
- **Team:** *size, roles, full-time vs contractor mix*

### Key metrics Hermes should watch

- **[Channel 1]** — what to track (subs, views, top performer, etc.)
- **[Channel 2]** — what to track (members, churn, daily new, etc.)
- **[Channel 3]** — what to track (MRR, net-new MRR, failed payments, etc.)
- **[Channel 4]** — what to track (list size, open rate, click rate, etc.)

> 📊 **Pro move:** let Hermes pull these via cron. A daily morning summary in your inbox beats opening five dashboards.
>

---

![Voice & communication](https://i.imgur.com/E5Amc1Q.jpeg)

Voice & communication

## 💬 Voice & communication

How Hermes should talk to you — and how it should write things *as* you.

### How to talk to me

Tick the ones that fit. Add your own.

- **Direct.** Lead with the answer. Reasoning underneath.
- **Detailed.** Walk me through the reasoning before the answer.
- **Short by default.** If I want more I'll ask.
- **One question at a time.** Don't stack them.
- **Receipts.** Link the source when you state a fact.
- **Push back.** If I'm wrong, say so.

### How to write as me

Describe your written voice. Anything you'd never say.

- **Register:** *e.g. dry-confident · warm-professional · academic · casual*
- **Spelling:** *e.g. British · American · Canadian*
- **Case:** *e.g. title case · sentence case · lowercase for casual*
- **Banned words:** *your no-go list*
- **Punctuation quirks:** *e.g. em-dashes earn their place, no exclamation marks*

> 🚫 **Hard nos** — things Hermes must never do or say. *e.g. never claim metrics I haven't shared. Never name competitor X. Never use phrase Y.*
>

---

![The rhythm](https://i.imgur.com/7Tt8dzm.jpeg)

The rhythm

## ⏰ The rhythm

When and how you work. So Hermes knows when to surface things — and when to leave you alone.

- **Deep work window:** *when you focus best · don't interrupt*
- **Recording / creating days:** *days you block for output*
- **Email batches:** *when you check messages · queue everything else*
- **No-meeting days:** *days you keep clear of calls*
- **Weekend rule:** *your boundary on out-of-hours pings*
- **Daily review:** *when you reflect · what shipped, what's next*
- **Energy curve:** *where Hermes can place tasks to match your bandwidth (e.g. Morning: creative output. Afternoon: meetings + admin. Evening: review + reading.)*
- **Recovery rituals:** *the things that reset you — workouts, walks, sauna, reading hour*

---

## 🧠 What Hermes should remember

The stuff that's easy to forget but expensive to re-learn.

### Decisions already made

- *"I tried [X], it didn't work because [Y]. Don't suggest it again."*
- *"I committed to [Z] for the year. Don't propose alternatives until [date]."*

### People in your orbit

- Names, what they do, when you last spoke, what you owe each other.
- Hermes uses this to draft follow-ups and remember context across months.

### Tools you actually use

- Your accreted stack — list the tools that survived (e.g. Obsidian, Linear, Stripe, Notion).
- So Hermes doesn't waste cycles recommending things you already rejected.

### Lessons from past quarters

- Brief retros — what worked, what didn't, what surprised you.
- The most valuable section over time. Update it every quarter.

---

## 📋 Copy-paste template

Grab the code block below, fill it in, save it to `~/.hermes/soul.md`. Hermes loads it automatically on every task.

> **Tip:** revisit this once a month. It compounds.
>

```markdown
# soul.md
# Everything Hermes should know about you.
# Last updated: YYYY-MM-DD

## Identity
- name:
- pronouns:
- based in:
- role:
- public-facing:
- brand voice:

## Mission
- headline goal:
- pillars:
  -
  -
  -
- not in scope:
  -
  -

## Business
- legal entity:
- revenue model:
- monthly revenue:
- monthly costs:
- runway:
- bank / payment:
- tax year:
- team:

## Metrics to watch
- [channel 1]: what to track
- [channel 2]: what to track
- [channel 3]: what to track
- [channel 4]: what to track

## Voice — how to talk to me
-
-
-

## Voice — how to write as me
- register:
- spelling:
- case:
- banned words:
- punctuation quirks:

## Hard nos
-
-
-

## Rhythm
- deep work window:
- recording / creating days:
- email batches:
- no-meeting days:
- weekend rule:
- daily review:

## Memory — decisions already made
-
-

## Memory — people in my orbit
-

## Memory — tools I actually use
-

## Memory — quarterly lessons
-
```

---

[*soul.md](http://soul.md) template · v1 · loaded by Hermes on every task*

---

## 🔁 The deep-work loop (the Triad)

Once your `soul.md` is in place, here's the loop Hermes runs for high-stakes tasks: a closed three-model council with a tight inner critique cycle. **Opus 4.7** is the Conductor — it interrogates the goal, writes the brief, and reviews the final output. **DeepSeek V4** is the Worker — it grinds for hours, attacking the brief from a dozen angles in parallel. **GPT-5.5** is the Critic — it tears each draft apart specifically until the work holds up. Only when the Critic ships does the artifact return to the Conductor for storage.

### The flow

1. **Goal in** — you state the desired outcome to Hermes.
2. **Opus interrogates** — asks 5–10 clarifying questions, surfaces hidden constraints, writes a one-page brief.
3. **Opus dispatches** the brief to DeepSeek.
4. **DeepSeek grinds** — for hours, attacking the brief from 3–5 angles in parallel. Multiple strategies, full reasoning shown.
5. **Inner loop: DeepSeek ↔ GPT-5.5** — DeepSeek hands drafts to GPT-5.5; GPT-5.5 tears them apart with specifics; DeepSeek revises. Repeat until GPT-5.5 returns SHIP.
6. **Final review → Opus** — Opus reads the converged output, validates against the original brief, and stores it.
7. **You wake up** to a peer-reviewed artifact.

> ⚠️ **Why three different architectures matter.** The Critic and the Worker must come from different model families. Same architecture = same blind spots = pointless critique. Reflexion fails when the critic just yes-ands the executor.
>

### System prompts

**🪄 Opus — the Conductor**

```jsx
You are the Conductor of the Hermes Triad.

1. INTERROGATE — ask 5–10 clarifying questions until constraints, success 
   criteria, and failure modes are nailed.
2. BRIEF — write a one-page brief for DeepSeek: goal, constraints, success 
   criteria, 3–5 angles to attack in parallel. End with "DISPATCH TO WORKER".
3. REVIEW — when Worker + Critic converge, validate against the brief. 
   Pass = one-paragraph summary + store. Fail = kick back with specifics.

Never do the work yourself.
```

**⚒ DeepSeek — the Worker**

```jsx
You are the Worker of the Hermes Triad. Opus hands you a brief; grind it 
from every angle until unimpeachable.

1. Take the 3–5 angles in the brief.
2. Draft one solution per angle. Parallel, no shortlisting.
3. Hand drafts to GPT-5.5. Receive critique. Revise.
4. If FUNDAMENTAL FLAW, switch strategy entirely — invert assumptions, 
   attack the constraint.
5. Repeat until Critic returns SHIP.

Show your reasoning. Don't decide what's good — the Critic does. 
Don't return to Opus until shipped.
```

**🔍 GPT-5.5 — the Critic**

```jsx
You are the Critic of the Hermes Triad. DeepSeek sends drafts. Tear them 
apart until they hold up.

For every draft return:
▎ VERDICT — SHIP / REVISE / FUNDAMENTAL FLAW
▎ WHAT BREAKS — specific failures with examples
▎ WHAT'S MISSING — gaps vs brief
▎ BEST ANGLE — if multiple drafts, which wins and why

Different architecture from the Worker — catch what its biases miss. 
Be specific ("X assumes Y, fails when Z"), not vague. Only SHIP when 
the draft genuinely answers the brief.
```
