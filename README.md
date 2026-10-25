<picture><source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png"><img src="assets/banner-light.png" alt="Johan Matsgård. Brand, growth and the AI behind them. C-level marketing leader at Elvy, 20 years in growth and brand as founder, CEO and advisor." width="100%"></picture>

<p align="center"><a href="https://www.linkedin.com/in/johanmatsgard/">LinkedIn</a> · <a href="https://github.com/johanmatsgard/vaken">vaken</a> · <a href="https://www.elvyenergy.com/design-system">Elvy design system</a></p>

**I build AI systems that run growth, and I lead them like an engineering team.** I have led growth, brand and digital for 20 years. For twelve of them I was co-founder and Nordic CEO of Digital Fans, a growth and automation agency. With Digital Fans and NORD DDB I have worked with brands in food, energy, cars, telecom, media and payments, like McDonald's, Vattenfall, Volkswagen, Telenor, MTG and Verifone. I was also Director of Growth Strategy and Head of Digital Transformation at NORD DDB. Today I lead marketing at C-level at Elvy in Stockholm, and I have advised Nordic Equity Group and its portfolio companies since 2018.

Most marketers brief engineers. I direct the agents that write the code, and I own the result. Since May: elvyenergy.com, now 4.5× the old site's conversion; Apollo, the AI marketing crew I build for our team; and vaken, open-source mission control for Claude Code. More than 6,300 commits from many agents running in parallel, planned and reviewed by me.

### Featured

<table>
<tr>
<td width="33%"><a href="#elvyenergycom-45-the-conversion-run-as-code"><img src="assets/featured-elvy.webp" alt="elvyenergy.com: 4.5× the conversion"></a></td>
<td width="33%"><a href="#apollo-a-small-team-with-the-reach-of-a-big-one"><img src="assets/featured-apollo.webp" alt="Apollo: a small team with the reach of a big one"></a></td>
<td width="33%"><a href="#vaken-mission-control-for-claude-code"><img src="assets/featured-vaken.webp" alt="vaken: mission control for Claude Code"></a></td>
</tr>
</table>

- **[elvyenergy.com](#elvyenergycom-45-the-conversion-run-as-code)**: Every page is code. Every change is tested. Now 4.5× the old site's conversion.
- **[Apollo](#apollo-a-small-team-with-the-reach-of-a-big-one)**: Elvy's AI marketing crew. About 6× more output per person, our own estimate.
- **[vaken](#vaken-mission-control-for-claude-code)**: Open-source mission control for Claude Code. Long-session context about 70% smaller, and a stop before risky commands.

## elvyenergy.com: 4.5× the conversion, run as code

<img src="assets/elvy-hero.webp" alt="elvyenergy.com: 4.5× the conversion. A new site on a new design system, then one tested change at a time." width="100%">

<img src="assets/elvy-proof.webp" alt="4.5× the conversion, no CMS, one journey from first visit to the Elvy app, and one gate for every change." width="100%">

The new site, built on a new design system, went live on 10 July. I have run it end to end since: pages, SEO, conversion, content, tracking, and the links to Apollo and our sales tools.

Every change ships the same way: an agent edits the code, opens a pull request with a preview, and a gate checks it. Conversion more than doubled in the first month, then kept climbing. Today the site converts **4.5× better** than the old one.

- **No CMS.** Every page is code, managed through Claude Code. Marketing moves without waiting in a developer queue.
- **One journey.** Onboarding looks up the house from the address, so visitors start with their own home. The path runs on to the offer and the Elvy app.
- **One gate.** No change merges without lint, types, tests, contrast and a token check. Off-brand styling cannot slip in.
- **Built for campaigns.** Wired to Apollo: a new campaign gets its own landing page fast, tracked from day one.

<img src="assets/uplift-dark.webp" alt="Conversion rate: 4.5× the old site." width="100%">

<table>
<tr>
<td width="50%"><img src="assets/elvy-site.webp" alt="Scrolling through elvyenergy.com"><br><b>The site.</b> Swedish and English, with an onboarding flow that looks up your house from your address. <a href="https://www.elvyenergy.com/">Visit it</a></td>
<td width="50%"><img src="assets/elvy-ds.webp" alt="The public Elvy design system: tokens and components"><br><b>The design system.</b> Public, and it renders the real components. <a href="https://www.elvyenergy.com/design-system">Open it</a></td>
</tr>
</table>

<img src="assets/elvy-offer.webp" alt="Coming soon: your price, in minutes. Answer a few questions and an indicative offer for the full package appears." width="100%">

**Coming soon: your price, in minutes.** An auto-offer flow in the onboarding. After that, the whole way to a signed contract, online.

<details>
<summary><b>How the site is built and run</b></summary>
<br>

- **Figma first.** The design system came first, then mockups built from it. Then it became code: tokens for colour, type, spacing, radii and shadows, and components that use only those tokens.
- **Styling is never invented.** All tokens live in one file. A lint rule blocks any value that is not a token, so no person or model can slip in a one-off colour or margin.
- **No CMS.** You ask an AI coding agent for a change and drop in the images. It edits the right file and opens a pull request with a preview link. Nothing goes live on its own.
- **One gate for every change.** Formatting, lint, type check, tests, contrast and document structure, and a check that the generated CSS still matches the tokens.
- **Leads flow straight on.** Each lead from the onboarding flow goes to sales with the house data attached, and quiet leads get a planned follow-up in HubSpot.

Stack: Next.js (App Router), React 19, TypeScript, Tailwind v4, next-intl, React Email, Vercel. [Full write-up](https://github.com/johanmatsgard/elvy-web-case-study)
</details>

## Apollo: a small team with the reach of a big one

<img src="assets/apollo-hero.webp" alt="A small team. The reach of a big one. The Apollo ship flies from Earth toward the Moon." width="100%">

<img src="assets/apollo-proof.webp" alt="About 6× more output per person by our own estimate, spots things first, better calls, more reach." width="100%">

**Apollo makes a small team work like a big one: about 6× more output per person, by our own estimate.**

I build the tools our team needs, and Apollo is the biggest. It spots the angle before anyone asks, answers every customer in minutes, and reacts while a moment still matters. Every ad channel sits next to signed customers, so each call rests on real numbers, and every recommendation gets a verdict. As Elvy grows, the same team covers more ground, so we hire for ideas, not for routine. People keep the ideas, the bold tests and the customers.

<img src="assets/apollo-climb.webp" alt="Every week, more of marketing flies itself. Areas move from Apollo watches, to Apollo drafts, to Apollo runs it." width="100%">

### 1. It listens

<table>
<tr><td width="50%"><img src="assets/apollo-market.webp" alt="Spots the angle before anyone else"></td><td width="50%"><img src="assets/apollo-replies.webp" alt="Answers every customer, in minutes"></td></tr>
<tr><td width="50%"><img src="assets/apollo-sales.webp" alt="Turns every sales call into better marketing"></td><td width="50%"><img src="assets/apollo-meet.webp" alt="Every meeting ends with a plan"></td></tr>
</table>

### 2. It makes and sells

<table>
<tr><td width="50%"><img src="assets/apollo-studio.webp" alt="Makes the ads while the moment is hot"></td><td width="50%"><img src="assets/apollo-web.webp" alt="Writes the pages people search for"></td></tr>
<tr><td width="50%"><img src="assets/apollo-ads.webp" alt="Spends like an agency that never sleeps"></td><td width="50%"><img src="assets/apollo-follow.webp" alt="Follows up every lead at the right moment"></td></tr>
</table>

### 3. It tests and learns

<table>
<tr><td width="50%"><img src="assets/apollo-tests.webp" alt="Always has the next test running"></td><td width="50%"><img src="assets/apollo-calls.webp" alt="Makes the call, then keeps score"></td></tr>
<tr><td width="50%"><img src="assets/apollo-brain.webp" alt="One memory for the whole company"></td><td width="50%"><img src="assets/apollo-bridge.webp" alt="Flies the company toward one number"></td></tr>
</table>

### 4. The team goes further

<img src="assets/apollo-team.webp" alt="Hours back for the work that matters. Apollo takes the routine; people take the bets." width="100%">

<table>
<tr><td width="50%"><img src="assets/apollo-work.webp" alt="Plans everyone's day around the goal"></td><td width="50%"><img src="assets/apollo-brief.webp" alt="Tells leadership the story, every Thursday"></td></tr>
</table>


Marketing is the first part of Elvy where we let AI take us this far. We approach every other part of Elvy the same way.

<details>
<summary><b>Under the hood</b></summary>
<br>

- Meta, TikTok, Google and LinkedIn in one view, next to signed customers straight from the company's own data. Nobody types numbers in by hand.
- Channels that count conversions differently are never ranked against each other.
- Every recommendation gets a verdict: implemented, skipped or watching. Nothing is forgotten.
- Built in Claude Code loops (ship, data, brain, adoption) that I orchestrate. Every change is reviewed by hand before it ships.
- The new look: a calm night sky with Earth and the Moon, built to feel like a ship's computer.

Stack: Next.js 16, Supabase (EU), Inngest, Anthropic SDK, Vercel. [Full write-up](https://github.com/johanmatsgard/apollo-case-study)
</details>

## vaken: mission control for Claude Code

<img src="assets/vaken-hero.webp" alt="vaken: stays awake, so you don't have to. It stops git reset --hard and waits for your OK." width="100%">

<img src="assets/vaken-proof.webp" alt="About 70% smaller context on long sessions, a safety stop, done-checks, and private by design." width="100%">

<sub>How we measured "about 70% lighter": the median of 361 compactions of sessions larger than 150,000 tokens in my own Claude Code use, October 2026. Context before the compaction against the first request after it.</sub>

Run ten Claude Code sessions and still know exactly where each one stands. vaken stops risky commands like `git reset --hard` and waits for your OK when Claude Code would not ask first, with undo. It compacts long sessions at a calm moment, so the context ends up about 70% smaller. I designed and built it alone with agents I plan and review, and released it as open source: 160+ releases in its first two weeks. No server, no telemetry.

<table>
<tr><td width="50%"><img src="assets/vaken-needs.webp" alt="Know what needs you, at a glance"></td><td width="50%"><img src="assets/vaken-limits.webp" alt="Never hit your limit by surprise"></td></tr>
<tr><td width="50%"><img src="assets/vaken-context.webp" alt="Long sessions, about 70% lighter"></td><td width="50%"><img src="assets/vaken-safety.webp" alt="A stop before a risky step"></td></tr>
<tr><td width="50%"><img src="assets/vaken-agents.webp" alt="Every helper, in one list"></td><td width="50%"><img src="assets/vaken-trust.webp" alt="Done means done: proof checks and away mode"></td></tr>
</table>

<details>
<summary><b>How it's built</b></summary>
<br>

- **Native first.** Every size and colour is measured from Claude Code Desktop in points and kept in one tokens file. A check fails the build on any raw number.
- **Safety guards.** It reads each tool call before it runs. Deletes, force-pushes and wipes stop and wait for your OK when Claude Code would not ask first.
- **Private by design.** No account, no server. Everything stays in a local file on your computer.
- **Tested in CI.** Every pull request runs the checks on Mac and Windows before it can merge.
- **Built by one person.** More than 1,800 commits, made with Claude Code agents that I plan, run and review.
</details>

Install it in ten seconds:

```
claude plugin marketplace add johanmatsgard/vaken
claude plugin install vaken@vaken
```

[See vaken on GitHub](https://github.com/johanmatsgard/vaken) · [Guide](https://github.com/johanmatsgard/vaken/blob/main/docs/guide.md)

## Also at Elvy

**The Elvy app.** I helped design and build our customer app, and from here I take a much bigger part in it. I also lifted the website's design system into a kit, so the app and the customer portal share the site's look. More on the app here soon.

## How I work

<img src="assets/how-i-work.webp" alt="One person. Many agents. One gate. I plan, agents build in parallel across elvyenergy.com, Apollo, vaken and the design loop, a gate checks every change, and I review and ship." width="100%">

I work like a small engineering lead. I set the goal, split it into tasks, and run many Claude Code agents side by side. A gate checks every change, and I read each one before it ships. The same method built elvyenergy.com, Apollo and vaken.

<table>
<tr>
<td width="50%"><img src="assets/design-loop.webp" alt="A design team that never stops: CONVERT, VOICE and CRAFT loops feed a review card, then I steer or it forks a new idea"><br><b>Design loop.</b> A design team that never stops. Claude Code loops design new screens from the design system, test them against a goal, and fork a fresh idea after two cycles. It is how new pages for the site get designed. <a href="https://github.com/johanmatsgard/design-loop">How it works</a></td>
<td width="50%"><img src="assets/huskartan.webp" alt="Huskartan scores every house in Sweden: ground, energy and roof data feed a score and one PDF report per address"><br><b>Huskartan.</b> Built to score every house in Sweden. Public data tells which homes gain most from a new heating system, when they are likely to act, and how good the roof is for solar. One PDF report per address. <a href="https://github.com/johanmatsgard/huskartan-case-study">How it works</a></td>
</tr>
</table>

<details>
<summary><b>More on the design loop</b></summary>
<br>

A design system gives you the parts. The loop decides what a page should do with them. It starts from a goal, like getting a customer to book a visit, and designs answers using only parts from the system.

- **CONVERT** gets the key action done. **VOICE** checks copy and numbers. **CRAFT** adds the details that make it feel distinct.
- Each run ends with a review card: what changed, why, and what to try next. I read it and steer.
- After two cycles the version is frozen, and the loop must try a new idea, not a restyle.
- Judged on a phone first. Mock data only.
</details>

**Now:** reading every recorded sales call to learn what makes people sign (Sonnet reads, Opus reviews), and [testing an AI moderator on 100 Swedish social media comments](https://github.com/johanmatsgard/jev-svenska-triage).

Want to talk growth, brand or AI in a company? [Message me on LinkedIn](https://www.linkedin.com/in/johanmatsgard/).
