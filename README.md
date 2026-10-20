# The Jab

**A social media manager that lives in your terminal.**

The Jab is a free, open-source content agent for [Claude Code](https://claude.com/claude-code).
Type `/jab 1` and it plans your week of posts, writes them in your brand's
voice, checks them for AI slop, remembers everything it has posted before,
and hands you a CSV your scheduler can import in one go.

You review. You approve. It schedules. Every week it gets a little better,
because it learns from what you've already posted and from the numbers you
give it.

Built by [KlivIQ](https://www.kliviq.com), where it runs our own social media every week.

---

## What it does

- **Plans and writes the whole week.** Hooks, captions, carousel slides,
  image prompts and video shot lists, one pillar per day.
- **Writes hooks on purpose.** It picks from 12 hook types, generates 5–10
  options for every post and keeps the strongest.
- **Kills AI slop before you see it.** Clichés, empty motivation, repeated
  structures and "this could be any company" posts get rewritten
  automatically.
- **Remembers.** A memory folder logs every hook, topic, CTA and visual, so
  it doesn't repeat itself week after week.
- **Learns from results.** Paste in your analytics and it adjusts the next
  week's topics, hooks and CTAs.
- **Keeps you in charge.** Nothing is scheduled until you say "approved".
- **One-shot scheduling.** It outputs a scheduler-ready CSV (built and
  tested with Metricool's bulk import).

## Quick start

1. Install [Claude Code](https://claude.com/claude-code).
2. Download this repo (Code > Download ZIP, or `git clone`).
3. Fill in `brand-profile.md`. This is the only setup that matters; take 15 minutes over it.
4. Add your first week's dates and rough topics to `content-calendar.md`.
5. From your scheduler, download its CSV import template and save it in
   this folder as `scheduler-template.csv`. (Metricool: Planning > ⋯ >
   Import CSV > Download template.)
6. Open a terminal in this folder, run `claude`, then type:

   ```
   /jab 1
   ```

7. Read `review/week-1-review.md`, edit anything, then type `approved`.
8. Import `outputs/metricool-week-1.csv` into your scheduler. Done.

## Every week after that

`/jab 2`, review, `approved`, import. About 15 minutes.

Got numbers from last week? Paste them in before running `/jab` and say
"log these". The Jab will use them.

## Folder map

```
CLAUDE.md                 the agent's instructions (works for any business)
brand-profile.md          your business, voice and rules  ← fill this in
content-calendar.md       weeks, dates, topics            ← add weeks here
hook-generation-rules.md  12 hook categories and how to pick them
.claude/commands/jab.md   the /jab command
memory/                   what it has posted and learned
review/                   weekly drafts for your approval
outputs/                  approved, import-ready CSVs
```

## Tips

- Specific beats clever. The more real detail in `brand-profile.md` (real
  customer pains, real phrases, real banned words), the better the posts.
- Use your own photos and screenshots where you can. Real material beats
  any generated image.
- If a post sounds like AI, tell it why. That lesson goes into
  `memory/playbook.md` and it won't make the same mistake again.

## Licence

MIT. Use it, change it, share it. A link back to
[kliviq.com](https://www.kliviq.com) is appreciated, not required.

---

Want it set up for your business, connected to your tools, or turned into
something bigger? Talk to us at [kliviq.com](https://www.kliviq.com).
