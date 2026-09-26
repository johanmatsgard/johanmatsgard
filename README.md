Hi, I'm Johan, CMO at [Elvy](https://www.elvyenergy.com/) in Stockholm.

I run marketing and also build a fair amount of the tools we use. Mostly Next.js and Supabase on Vercel, written with Claude Code.

### Apollo

Our internal marketing platform at Elvy. It pulls in ad data from Meta, TikTok, Google and LinkedIn, gives recommendations the team marks as implemented, skipped or watching, and tracks progress against the real signed-customer count. It also refuses to compare channels on metrics they measure differently.

It's designed as a ship's computer with a bridge, rooms and a log, mostly because a tool people use a lot should be nice to open. I develop it with separate agent loops for different kinds of work, and nothing reaches the team before I've checked it in a preflight environment.

[How it works](https://github.com/johanmatsgard/apollo-case-study)

### Design loop

An autonomous design process I run in Claude Code on Elvy's customer portal. Five loops each look at one part of the experience, every run ends with a review card for me to steer from, and after two cycles it forks a new version built on a different idea. [How it works](https://github.com/johanmatsgard/design-loop)

### Huskartan

Scores Swedish houses on heating, timing and solar potential using public data from SGU, Boverket and roof imagery. [How it works](https://github.com/johanmatsgard/huskartan-case-study)

### Lead handling

I wrote the spec for how Elvy handles new leads in HubSpot: contact within five minutes, a task queue that tells sales what to do next, and a 60-day reactivation flow for leads that go quiet. Our tech team took it from there.

### Block Kit

Small Python prototype that geocodes addresses into blocks for addressed direct mail through PostNord.

### In progress

A full read of our recorded sales calls. Sonnet goes through every call and Opus reviews what it found, with the aim of improving our ads, website and sales conversations.

Testing TypeSafe's Jev on Swedish social media comments: [jev-svenska-triage](https://github.com/johanmatsgard/jev-svenska-triage). If it holds up, the next step is using it in Apollo to decide which model handles which task, and to check generated copy against our brand rules before it goes out.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/johanmatsgard/johanmatsgard/output/github-snake-dark.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/johanmatsgard/johanmatsgard/output/github-snake.svg" />
</picture>
