```console
$ whoami
johan matsgård · cmo @ elvy · stockholm, se
```

I run marketing at [Elvy](https://www.elvyenergy.com/), a Swedish residential energy subscription company. I also build the software my team runs on. Most of it is written with Claude Code, deployed on Vercel, and reviewed by me before anyone else touches it.

```yaml
# ~/.johan.yml
role:        CMO @ Elvy
builds_with: Claude Code
ships_to:    Vercel
stack:       [Next.js 16, Supabase, Postgres, Inngest, Anthropic SDK, Python]
currently:   testing typed decisions with Jev (TypeSafe) in Swedish
```

---

### 🛰️ Apollo
Elvy's internal AI marketing platform, designed as a ship's computer. The crew works from the bridge, every decision lands in the log, and clearance levels decide who can do what.

- Meta, TikTok, Google and LinkedIn ads data in one place, with a guardrail that blocks comparisons between channels that don't measure the same thing
- A recommendations loop where every AI suggestion is marked **Implemented**, **Skipped** or **Watching**
- Progress tied to Elvy's real signed-customer count, pulled from the source system with no manual inputs
- Multi-brand auth with enforced 2FA (TOTP)
- WebGL and 3D on the surfaces where the tool should feel alive

Developed through purpose-built agent loops I run as slash commands in Claude Code:

```
docs/loops/
├── CORE.md
├── SHIP.md       # /apollo-ship
├── BRAIN.md      # /apollo-brain
├── DATA.md       # /apollo-data
├── BET.md        # /apollo-bet
└── ADOPTION.md   # /apollo-adoption
```

Nothing reaches the team without passing `preflight`, a permanent pre-launch environment on its own branch that only I promote to `main`.

→ [Read the case study](https://github.com/johanmatsgard/apollo-case-study)

### 🗺️ Huskartan
Scores Swedish homes on heating, timing and solar potential using public data (SGU well archive, Boverket energy declarations, roof and satellite data), so marketing reaches the right house at the right moment.
→ [Case study](https://github.com/johanmatsgard/huskartan-case-study)

### 📮 Block Kit
Python geocoding prototype that turns address data into blocks for addressed direct mail through PostNord.

### 🧪 Now
Testing whether Jev (TypeSafe) can moderate Swedish social comments well enough to act without a human, and whether its confidence knows when it can't.
→ [jev-svenska-triage](https://github.com/johanmatsgard/jev-svenska-triage)

---

<p>
  <img src="https://skillicons.dev/icons?i=nextjs,react,supabase,postgres,vercel,python,figma&theme=dark" alt="stack" />
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/johanmatsgard/johanmatsgard/output/github-snake-dark.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/johanmatsgard/johanmatsgard/output/github-snake.svg" />
</picture>

<sub>Marketer who ships.</sub>
