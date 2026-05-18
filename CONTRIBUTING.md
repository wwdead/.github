# Contributing to WWdead Community Projects

Thanks for wanting to contribute! This is a community-run collection of 
fan-made tools, userscripts, and projects for [Worldwide Dead](https://wwdead.com). 
Everyone is welcome here — whether you're a developer or just a player with 
a great idea.

---

## There are many ways to contribute

You don't need to know how to code to help out. Here's what you can do:

| Contribution type | Where to do it |
|---|---|
| Suggest a script or tool idea | Discord https://discord.com/channels/1420504434227806350/1476815676315533323 or GitHub Discussions |
| Report a bug | Report it on Discord channel specific to the script or GitHub Issues |
| Contribute map data or game info | Discord https://discord.com/channels/1420504434227806350/1476815676315533323 or GitHub Issues |
| Improve documentation | GitHub Pull Request |
| Write or fix a script | GitHub Pull Request |
| Review someone else's PR | GitHub Pull Request |

---

## Not on GitHub? No problem.

The easiest way to contribute is through our 
[Discord server](https://discord.gg/fwapYnMGFw):

A maintainer will make sure good ones make it to GitHub and will credit 
you by name when they do.

---

## For GitHub Users

### Reporting a Bug
1. Check [existing issues](../../issues) first to avoid duplicates
2. Click **New Issue** and choose the **Bug Report** template
3. Fill it out as completely as you can — screenshots are very helpful
4. Add the `bug` label

### Suggesting an Idea
1. Open a [Discussion](../../discussions) in the **Ideas** category
2. Describe what you want and why it would help players
3. The community can vote and comment before any dev work starts
4. If it gets traction a maintainer will convert it to an Issue

---

## For Developers

### Setting Up
1. Fork the repo you want to work on
2. Clone your fork: `git clone https://github.com/YOUR-USERNAME/REPO-NAME`
3. Create a branch for your work: `git checkout -b my-feature-name`
### Userscript Requirements

Every userscript must have a complete header block:

```javascript
// ==UserScript==
// @name         WWdead - Your Script Name
// @namespace    https://github.com/wwdead
// @version      1.0.0
// @description  A brief description of what this script does
// @author       YourGitHubUsername
// @match        https://wwdead.com/classic/*
// @grant        none
// ==/UserScript==
```

**Rules:**
- `@name` must start with `WWdead -`
- `@match` should target `https://wwdead.com/classic/*` unless there's a 
  specific reason to target other pages
- `@version` follows [semantic versioning](https://semver.org/) (1.0.0)
- `@author` should be your GitHub username

### Code Style
- Use plain JavaScript where possible — avoid external libraries unless 
  necessary
- Add comments explaining anything that isn't immediately obvious
- Keep scripts self-contained
- No minified code — keep it readable so others can learn from and 
  maintain it

### Testing Your Script
Before submitting, test in at least one of:
- ✅ Tampermonkey on Chrome
- ✅ Tampermonkey on Firefox
- ✅ Violentmonkey on Chrome or Firefox

Make sure your script:
- Only runs on WWDead pages
- Doesn't break any core game functionality
- Doesn't make unexpected network requests
- Works when installed fresh with no prior state

### Submitting a Pull Request
1. Push your branch to your fork
2. Open a Pull Request against `main`
3. Fill out the PR template completely
4. We aim to review all PRs within **7 days**

Your PR will be reviewed by a maintainer. They may request changes — 
that's normal and not a rejection. Once approved it'll be merged and 
you'll be credited in the changelog.

### Updating an Existing Script
- Bump the `@version` number appropriately
- Note the change in your PR description
- Minor fixes = patch version (1.0.0 → 1.0.1)
- New features = minor version (1.0.0 → 1.1.0)

---

## How We Credit Contributors

Every merged contribution gets credited. If you contributed via Discord 
and a maintainer created the Issue on your behalf, you'll still be 
named. No contribution goes unrecognized.

---

## Getting Help

- Post in the **Q&A** category on [GitHub Discussions](../../discussions)
- Ask  on the [Discord server](https://discord.gg/fwapYnMGFw)

We were all new once — no question is too basic.

