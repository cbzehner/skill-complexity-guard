# Complexity Guard

Keep engineering work scoped, boring, and maintainable. The skill is a standing check against speculative abstractions and code that solves problems no one has yet.

## Use It For

- Writing or reviewing code
- Planning architecture changes
- Running an overengineering or simplification sweep

## Install

Clone the repo and run the installer:

```bash
git clone https://github.com/cbzehner/skill-complexity-guard.git
cd skill-complexity-guard
./install.sh all
```

Install targets:

- `./install.sh claude` installs to `~/.claude/skills/complexity-guard`
- `./install.sh codex` installs to `~/.codex/skills/complexity-guard`
- `./install.sh agents` installs to `~/.agents/skills/complexity-guard`
- `./install.sh opencode` installs to `~/.config/opencode/skills/complexity-guard`
- `./install.sh all --copy` copies files instead of symlinking

Manual install works too: symlink or copy `skills/complexity-guard` into your agent's skills directory.

## Agent Support

This repo uses the plain `skills/complexity-guard/SKILL.md` layout. Claude Code and Codex also get small plugin manifests at `.claude-plugin/plugin.json` and `.codex-plugin/plugin.json`.

Other agents can read the same `SKILL.md` file. If a host does not support a frontmatter field or tool name, ignore that field and follow the workflow text.

## Layout

```text
.claude-plugin/plugin.json
.codex-plugin/plugin.json
install.sh
skills/complexity-guard/SKILL.md
README.md
LICENSE
```

## Public Notes

These repos are public. Keep private repo names, secrets, customer data, raw logs, cookies, and absolute filesystem paths out of examples.

## License

MIT
