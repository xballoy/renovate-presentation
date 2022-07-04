---
theme: ./theme
highlighter: shiki
drawings:
  persist: false
title: Migrate from Dependabot to Renovate
layout: intro

---

<div class="absolute top-10">
  <p class="font-700">
    Xavier Balloy | <Today />
  </p>
</div>

<div class="absolute bottom-10">
  <h1>Migrate from Dependabot to Renovate</h1>
  <p class="text-sm"><Version /></p>
</div>

---

# Dependabot

- Automation service that create PRs to keep your projects' dependencies up to date
- Native integration in GitHub (app)
- Does not work on other platforms (unofficial integration with GitLab) 
- Not a lot of configuration: 1 PR per dependency
- No native automerge: needs to use mergify (free for public project)
- Free

---

# Renovate

- Automation service that create PRs to keep your projects' dependencies up to date
- Support multiple platforms (GitHub, GitLab, BitBucket, Azure DevOps, Gitea)
- A lot of configuration options: scheduling, rules per package... 
- Run as a GitHub app, npm package or can be self-installed
- Native automerge
- Dependency Dashboard
- Free

---

# Migrate from Dependabot

1. Install the GitHub app: it will open a PR to configure Renovate
2. Delete .github/dependabot.yml and .github/mergify.yml if used only to merge Dependabot
3. Configure renovate.json
4. That's all!

--- 

# Demo time!

- [Configure Renovate PR](https://github.com/xballoy/dojo-typescript-bootstrap/pull/322)
- [My Renovate Setup](https://github.com/xballoy/dojo-typescript-bootstrap/blob/main/renovate.json)
- [Renovate PR example](https://github.com/xballoy/dojo-typescript-bootstrap/pull/326)

---

# Learn more

- [Renovate Docs](https://docs.renovatebot.com/)
