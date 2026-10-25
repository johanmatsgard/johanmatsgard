<picture><source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png"><img src="assets/banner-light.png" alt="Johan Matsgård: Head of Marketing who builds the software his team runs on" width="100%"></picture>

<p align="center">
<a href="https://www.linkedin.com/in/johanmatsgard/"><img src="https://img.shields.io/badge/LinkedIn-Johan%20Matsg%C3%A5rd-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://github.com/johanmatsgard/vaken"><img src="https://img.shields.io/badge/New-vaken%20for%20Claude%20Code-D97757?style=for-the-badge" alt="vaken"></a>
<a href="https://www.elvyenergy.com/design-system"><img src="https://img.shields.io/badge/Live-Elvy%20design%20system-9BBE3C?style=for-the-badge" alt="Elvy design system"></a>
</p>

I run marketing at [Elvy](https://www.elvyenergy.com/) in Stockholm, and I build most of the tools we use. The website I rebuilt converts **3.2× better** than the old one, and it keeps climbing. Next.js and Supabase on Vercel, all of it written with Claude Code.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/stats-dark.png"><img src="assets/stats-light.png" alt="6,300+ commits since May 2026, 1,700+ merged pull requests, 1,900+ test files, 3 products in daily use" width="100%"></picture>

<sub>Counted across vaken, Apollo and elvyenergy.com.</sub>

## 📈 elvyenergy.com: 3.2× the conversion

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/uplift-dark.webp"><img src="assets/uplift-light.webp" alt="Conversion rate compared to the old site: about 2.3× in July, 2.8× in September, 3.2× in October. Paid traffic: 3.7×." width="100%"></picture>

The new site more than doubled conversion in its first month. Then it kept climbing, one tested change at a time. Paid traffic now converts 3.7× better than the old site did. That is why the numbers above are so high: every commit is a try at getting one more visitor to ask for a quote.

<table>
<tr>
<td width="50%"><img src="assets/elvy-site.webp" alt="Scrolling through elvyenergy.com"><br><b>The site.</b> Swedish and English, with an onboarding flow that looks up your house from your address. <a href="https://www.elvyenergy.com/">Visit it</a></td>
<td width="50%"><img src="assets/elvy-ds.webp" alt="The public Elvy design system: tokens and components"><br><b>The design system.</b> Public, and it renders the real components. <a href="https://www.elvyenergy.com/design-system">Open it</a></td>
</tr>
</table>

<details>
<summary><b>How the site is built</b></summary>
<br>

- **Figma first.** The design system came first, then mockups built from it. Then it became code: tokens for colour, type, spacing, radii and shadows, and components that use only those tokens.
- **Styling is never invented.** All tokens live in one file. A lint rule blocks any value that is not a token, so no person or model can slip in a one-off colour or margin.
- **No CMS.** You ask an AI coding agent for a change and drop in the images. It edits the right file and opens a pull request with a preview link. Nothing goes live on its own.
- **One gate for every change.** Formatting, lint, type check, tests, contrast and document structure, and a check that the generated CSS still matches the tokens.
- **Measured honestly.** Brand-awareness traffic converts at about 0.2 %, so it would hide real gains. We read conversion with and without it, side by side.

Stack: Next.js (App Router), React 19, TypeScript, Tailwind v4, next-intl, React Email, Vercel. [Full write-up](https://github.com/johanmatsgard/elvy-web-case-study)
</details>

<details>
<summary><b>What happens after the form</b></summary>
<br>

A lead is only worth something if sales calls back fast. I wrote the spec for how Elvy handles new leads in HubSpot:

- Contact within five minutes.
- A task queue, so sales always knows who to call next.
- A 60-day follow-up flow for leads that go quiet.
</details>

## ⭐ vaken: a calm side pane for Claude Code

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/vaken-hero-dark.webp"><img src="assets/vaken-hero-light.webp" alt="vaken stops git reset --hard in Claude Code Desktop and waits for your OK" width="100%"></picture>

My first public plugin. It shows what needs you across all your sessions, how much of your plan is left, how full the context is, and what your agents do. It stops risky steps like `git reset --hard` when Claude Code would not ask first. It looks like part of the app, and keeps all its data on your computer.

<table>
<tr>
<td width="50%"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/vaken-needs-dark.webp"><img src="assets/vaken-needs-light.webp" alt="Needs you"></picture><br><b>Needs you.</b> Every session that waits for you, in one list.</td>
<td width="50%"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/vaken-limits-dark.webp"><img src="assets/vaken-limits-light.webp" alt="Plan limits"></picture><br><b>Plan limits.</b> What is left, and when it resets.</td>
</tr>
<tr>
<td><picture><source media="(prefers-color-scheme: dark)" srcset="assets/vaken-context-dark.webp"><img src="assets/vaken-context-light.webp" alt="Context"></picture><br><b>Context.</b> How full the chat is, and a good moment to compact.</td>
<td><picture><source media="(prefers-color-scheme: dark)" srcset="assets/vaken-agents-dark.webp"><img src="assets/vaken-agents-light.webp" alt="Agents"></picture><br><b>Agents.</b> What every helper does, and what it costs.</td>
</tr>
</table>

<details>
<summary><b>How it's built</b></summary>
<br>

- **Native first.** Every size and colour is measured from Claude Code Desktop in points and kept in one tokens file. A check fails the build on any raw number.
- **Safety guards.** It reads each tool call before it runs. Deletes, force-pushes and wipes stop and wait for your OK when Claude Code would not ask first.
- **Private by design.** No account, no server. Everything stays in a local file on your computer.
- **Tested in CI.** Every pull request runs the checks on Mac and Windows before it can merge.
</details>

**[Install vaken](https://github.com/johanmatsgard/vaken)** · [Guide](https://github.com/johanmatsgard/vaken/blob/main/docs/guide.md)

## 🚀 Apollo

<img src="assets/apollo.webp" alt="Apollo running on demo data" width="100%">

Elvy's internal marketing platform, designed as a ship's computer. It pulls Meta, TikTok, Google and LinkedIn into one view next to the company's real numbers, and gives recommendations the team marks as implemented, skipped or watching. <sub>Demo data only.</sub>

<details>
<summary><b>How it works</b></summary>
<br>

- **One source of truth.** Signed customers and other real numbers come straight from Firestore. Nobody types numbers in by hand.
- **No unfair rankings.** Meta, TikTok, Google and LinkedIn count conversions in different ways. Apollo will not rank them against each other on those numbers.
- **Every recommendation needs a verdict.** Implemented, skipped or watching. Otherwise ideas pile up and nobody remembers what we did.
- **Writes in Elvy's voice.** Drafts press releases and debate articles.
- **Built in loops.** Claude Code runs one loop per kind of work (ship, data, brain, adoption). Changes land on a preflight branch first, and I merge to main myself.

Stack: Next.js 16, Supabase (EU), Inngest, Anthropic SDK, Vercel. [Full write-up](https://github.com/johanmatsgard/apollo-case-study)
</details>

## 🧪 Methods and models

<table>
<tr>
<td width="50%"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/loop-dark.png"><img src="assets/loop-light.png" alt="Design loop: CONVERT, VOICE and CRAFT loops feed a review card"></picture><br><b>Design loop.</b> How the site's conversion keeps climbing. Claude Code loops design new screens from the design system, then fork a new idea after two cycles. <a href="https://github.com/johanmatsgard/design-loop">How it works</a></td>
<td width="50%"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/huskartan-dark.png"><img src="assets/huskartan-light.png" alt="Huskartan: public data sources feed a house score and a PDF report"></picture><br><b>Huskartan.</b> Scores Swedish houses on heating, timing and solar from public data, with one PDF report per address. <a href="https://github.com/johanmatsgard/huskartan-case-study">How it works</a></td>
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

**Now:** a full read of our recorded sales calls (Sonnet reads, Opus reviews), and [testing Jev on Swedish comments](https://github.com/johanmatsgard/jev-svenska-triage).
