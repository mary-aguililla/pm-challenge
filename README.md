# PM Challenge

A Claude Code skill that runs a blunt, opinionated 7-question critique on any PM doc, brief, or decision — then ends with a coaching question instead of just handing you the answer.

It's built to do two things: catch weak reasoning before you ship a brief, and build the muscle to catch it yourself next time.

## What it does

When invoked, the skill runs your work through a 7-question gauntlet:

1. **Problem Framing** — is this real user pain, or a solution in disguise?
2. **Evidence Check** — does the evidence support the specific claim being made?
3. **Success Definition** — is success a behavior change, or just "ship by [date]"?
4. **Trade-off Articulation** — what's explicitly *not* being done, and why?
5. **Risk & Assumption Surfacing** — what's the riskiest assumption, ranked?
6. **Smallest Test** — what's the cheapest way to learn if you're wrong before you build?
7. **Coaching Turn** — a Socratic question aimed at the weakest habit in the artifact, not a summary

Each dimension gets scored 1–5 against behavioral anchors (not gut feel), and — where a named principle applies — the critique cites the thinker it's drawing from.

## Usage

```
/pm-challenge [optional: file path or topic]
```

- No args → critiques whatever doc/plan is in the current conversation
- File path → reads and critiques that file
- Topic → challenges your thinking on it via Socratic conversation

## Files

- `SKILL.md` — the critique protocol, scoring rubric, and tone rules
- `references.md` — the reference library of thinkers the skill cites from

## Installation

Copy both files into `.claude/skills/pm-challenge/` in your project (or your global skills directory), matching the paths referenced in `SKILL.md`.

## A note on the references

This skill cites eight people whose public writing, podcasts, and interviews shaped how I think about product work: Cat Wu, Claire Vo, Shreyas Doshi, Marty Cagan, Teresa Torres, Julie Zhuo, Lenny Rachitsky, and Elena Verna.

**This project is not affiliated with, endorsed by, or built in partnership with any of them.** It's my own distillation of what I've learned from their blogs, books, podcasts, and interviews — linked back to the original sources in `references.md` so you can go straight to their work rather than take my paraphrase of it as the final word.

If their thinking resonates, follow them directly for more:

- [Cat Wu](https://www.linkedin.com/in/cat-wu/) — Head of Product, Claude Code and Cowork at Anthropic
- [Claire Vo](https://www.linkedin.com/in/clairevo/) — CPO at LaunchDarkly, founder of ChatPRD
- [Shreyas Doshi](https://www.linkedin.com/in/shreyasdoshi/) — former PM leader at Stripe, Twitter, Google, Yahoo
- [Marty Cagan](https://www.linkedin.com/in/cagan/) — Founder, Silicon Valley Product Group
- [Teresa Torres](https://www.linkedin.com/in/teresatorres/) — Product discovery coach, author of *Continuous Discovery Habits*
- [Julie Zhuo](https://www.linkedin.com/in/julie-zhuo/) — former VP Product Design at Facebook, author of *The Making of a Manager*
- [Lenny Rachitsky](https://www.linkedin.com/in/lennyrachitsky/) — writer, advisor, former Head of Supply Growth at Airbnb
- [Elena Verna](https://www.linkedin.com/in/elenaverna) — Head of Growth at Lovable, former growth leader at Dropbox, SurveyMonkey, Miro, Amplitude

## License

*(Add your preferred license here — MIT is the common default for a repo like this if you want it freely reusable.)*
