# ikenga-contribute

A contributor's copilot for [Ikenga](https://ikenga.dev) — a Claude Code skill that helps you:

- **Draft a well-formed issue** — reads the target repo's actual template field-set, gathers the details (auto-collecting env/version/OS for bugs), and assembles a filled body.
- **Run the full PR workflow** — branch naming, Conventional Commits, a Changesets reminder where the repo needs one, the repo's own tests, and a filled PR template.
- **Onboard as a package author** — orients you on archetype, then hands off to `ikenga-pkg-builder` for the scaffold.

Two invariants: it **consumes the project's published conventions** (never invents rules), and it **confirms before anything outward-facing** (it drafts; you send).

## Install

```bash
npx skills add ikenga-hq/ikenga-contribute
```

Or via the install script:

```bash
curl -sSL https://raw.githubusercontent.com/ikenga-hq/ikenga-contribute/main/install.sh | bash
```

Inside a running Ikenga shell, install it from the Ọba catalog.

## Use

Invoke `/ikenga-contribute` and say what you want — file an issue, open a PR, or build a pkg. The human-readable version of everything this skill automates is the [contributing guide](https://ikenga.dev/docs/contributing).

## Source

This repo is the distribution mirror. The canonical source lives in the [`ikenga-pkgs`](https://github.com/ikenga-hq/ikenga-pkgs) monorepo at `packages/skills/contribute/`.

Apache-2.0.
