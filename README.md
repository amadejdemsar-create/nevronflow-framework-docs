# NevronFlow Framework — Docs

Visual explorer and installer for the NevronFlow framework.

> **Source code lives in a private repository:** [amadejdemsar-create/nevronflow-framework](https://github.com/amadejdemsar-create/nevronflow-framework) (collaborator access required).
> **This repository is public** and hosts only the HTML docs + install prompt.

## What is NevronFlow?

A Claude Code development framework for the NevronCore hospitality platform:

- **16 rules** covering multi-tenant safety, backend/frontend/PWA/TV style guides, testing, app store compliance, analytics contribution
- **20 agents** for implementation (backend, frontend, PWA, TV, PMS, mobile, etc.) and judgment (feature-planner, diagnostician, analytics-architect, etc.)
- **23 skills** invoked as `/nf:*` slash commands
- **1 hook** that enforces delegation at the tool-call level

## How to install

Visit the [docs site](https://amadejdemsar-create.github.io/nevronflow-framework-docs/) (or open `index.html` directly in this repo), click **"Install into nevron-core"**, and paste the copied prompt into a new Claude Code session.

The install prompt:
1. Searches your filesystem broadly for your local `nevron-core` checkout
2. Asks you to confirm the correct path (or supply one manually)
3. Describes exactly what it's about to install, asks for your approval
4. Clones the private framework repo (3 fallback methods: git / gh / GitHub MCP)
5. Backs up your existing `.claude/` with a timestamped suffix
6. Installs the framework, sets hook permissions
7. Asks about optional templates one by one
8. Cleans up, tells you to restart Claude Code

You must be a collaborator on the private framework repo for the clone step to succeed. If you are not yet a collaborator, the install prompt will detect the 404 and tell you to request access.

## Updates

When the framework evolves, this repo is updated with the latest HTML. Re-visit the docs site and re-run the install prompt; the installer backs up your existing `.claude/` first, so repeated installs are safe.

## Who has access to the framework itself

Access to the private framework repo is granted per person by the repo owner. Contact the Nevron engineering team for an invitation.
