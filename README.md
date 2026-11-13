# Broken link checker (Claude skill)

Click through a website in a real browser and get a list of every link that errors or shows an empty page, with the page it is on. The skill hands the job to your own MyClawn cloud computer: a real browser that stays signed in, its own email address and files. It comes back with the answer, a screenshot of the final screen and a link to a screen recording.

## Example request

> Start at <your site URL>, follow the links on the first 40 pages you reach, and list every link that errors or shows an empty page. Give the broken link, the page it is on, and what you saw.

## What you get

- It answers with a list: broken link, the page it appears on, and what it saw.
- A screenshot of the final screen and a link to a screen recording.

## What it does not do

- It checks the pages it reaches in one run; it is not a monitor that runs on its own every night.
- It reports what a visitor sees. A link that only fails for logged-in users needs you to sign in once on the live screen.
- It lists problems; it does not edit your site.

## Install

Claude Code, as a personal skill:

```sh
mkdir -p ~/.claude/skills/broken-link-checker && curl -fsSL https://raw.githubusercontent.com/20vision/broken-link-checker-skill/main/SKILL.md -o ~/.claude/skills/broken-link-checker/SKILL.md
```

With the skills tool (installs into the current project):

```sh
npx skills add 20vision/broken-link-checker-skill
```

## Needs

The MyClawn Computer connector, signed in with your own MyClawn account. Setup and details: https://www.myclawn.com/docs/connectors?utm_source=github&utm_medium=repo&utm_campaign=broken-link-checker

Full description of this job, with the steps and the limits: https://www.myclawn.com/check-my-website-for-broken-links?utm_source=github&utm_medium=repo&utm_campaign=broken-link-checker

## Also listed

- https://www.skillsdirectory.com/skills/20vision-broken-link-checker
- https://www.agensi.io/skills/broken-link-checker
- All skills: https://github.com/20vision/skills

Made by 20Vision, the company behind MyClawn.
