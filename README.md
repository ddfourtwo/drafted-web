# Drafted — Claude plugin (web & Cowork)

Public mirror of the remote-connector [Drafted](https://drafted.live) plugin for
Claude on the web and in Cowork. It bundles the Drafted MCP connector
(`https://drafted.live/mcp`), the `drafted` skill, and eight slash commands.

Source of truth: the private `ddfourtwo/drafted` repo (`web-plugin/`).
Do not PR here — open issues at https://drafted.live.

## Install

**Claude (web) / Cowork:** two steps.

1. Settings → Customize plugins → Add → Add marketplace → `https://github.com/ddfourtwo/drafted-web` → install the **Drafted** plugin (skill + slash commands).
2. Settings → Connectors → find **Drafted** → **Connect**, then approve the sign-in (the Drafted tools).

Installing the plugin does not connect you automatically — do both. You'll sign in to Drafted (OAuth) on first use.

**Claude Code:**

```
claude plugin marketplace add ddfourtwo/drafted-web
claude plugin install drafted@drafted-web
```

## Commands

- `/drafted:onboard-drafted` — orient + bootstrap the harness
- `/drafted:ingest` — pull knowledge into the wiki
- `/drafted:create-skill` — author a reusable procedure
- `/drafted:create-project` — new project or from a template
- `/drafted:improve-wiki` — fix or sharpen knowledge
- `/drafted:improve-skill` — refine a procedure
- `/drafted:improve-project-harness` — turn a correction into a standing rule
- `/drafted:extract` — close the loop: file new knowledge, skills, structure

## Learn more

- Product: https://drafted.live
- How to use it: https://drafted.live/how-to
- Install (desktop / CLI): https://drafted.live/install

MIT © Mind Athletic BV
