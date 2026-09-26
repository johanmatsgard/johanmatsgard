Hi, I'm Johan, Head of Marketing at [Elvy](https://www.elvyenergy.com/) in Stockholm.

I run marketing and also build a fair amount of the tools we use. Mostly Next.js and Supabase on Vercel, written with Claude Code.

### elvyenergy.com

Elvy's website, and the biggest thing I've built so far. I started with a design system in Figma, mocked up the site from it, and then translated it into tokens and components with parameters that every page is built from. A lint rule bans any styling that isn't a token, so people and models alike stay inside the system.

There's no CMS. Content is changed by talking to an AI coding agent, which edits the files, uploads images and opens a pull request with a preview. Since everything is plain code with strict rules, the site isn't tied to one tool, and when a better model comes out it can start working on the site right away. There are Swedish and English versions, and an onboarding flow that looks up your house from your address.

The design system is public at [elvyenergy.com/design-system](https://www.elvyenergy.com/design-system). [How it's built](https://github.com/johanmatsgard/elvy-web-case-study)

### Apollo

Our internal marketing platform at Elvy. It pulls in ad data from Meta, TikTok, Google and LinkedIn, reads the company's own numbers from Firestore, our single source of truth, and gives recommendations the team marks as implemented, skipped or watching. It also refuses to compare channels on metrics they measure differently.

It's designed as a ship's computer with a bridge, rooms and a log, mostly because a tool people use a lot should be nice to open. I develop it with separate agent loops for different kinds of work, and nothing reaches the team before I've checked it in a preflight environment.

[How it works](https://github.com/johanmatsgard/apollo-case-study)

### Design loop

How I get from a design system to finished screens. Once the system is in place, I run loops in Claude Code that design and iterate solutions for what a page or app screen needs to achieve, using only parts from the system. Each run ends with a review card I steer from, and after two cycles it forks a new version built on a different idea. [How it works](https://github.com/johanmatsgard/design-loop)

### Huskartan

Scores Swedish houses on heating, timing and solar potential using public data from SGU, Boverket and roof imagery. [How it works](https://github.com/johanmatsgard/huskartan-case-study)

### Lead handling

I wrote the spec for how Elvy handles new leads in HubSpot: contact within five minutes, a task queue that tells sales what to do next, and a 60-day reactivation flow for leads that go quiet. Our tech team took it from there.

### Block Kit

Python prototype that uses addresses and geocodes to plan addressed direct mail through PostNord.

### In progress

A full read of our recorded sales calls. Sonnet goes through every call and Opus reviews what it found, with the aim of improving our ads, website and sales conversations.

Testing TypeSafe's Jev on Swedish social media comments: [jev-svenska-triage](https://github.com/johanmatsgard/jev-svenska-triage). If it holds up, the next step is using it in Apollo to decide which model handles which task, and to pre-sort incoming leads.

[LinkedIn](https://www.linkedin.com/in/johanmatsgard/)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/johanmatsgard/johanmatsgard/output/github-snake-dark.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/johanmatsgard/johanmatsgard/output/github-snake.svg" />
</picture>
