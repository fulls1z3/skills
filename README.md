# fulls1z3-skills

Agent skills packaged as one Claude plugin, for claude.ai and Claude Code.

| Skill | Does |
| --- | --- |
| [grilling](skills/grilling/SKILL.md) | stress-tests a plan or decision through question cards; run it with `/grilling` |
| [grill-with-docs](skills/grill-with-docs/SKILL.md) | runs the existing grilling interview with a project glossary and ADRs |
| [domain-modeling](skills/domain-modeling/SKILL.md) | clarifies project language and records consequential decisions |
| [improve-codebase-architecture](skills/improve-codebase-architecture/SKILL.md) | produces a visual architecture review and explores the selected candidate through question cards |
| [codebase-design](skills/codebase-design/SKILL.md) | supplies module design vocabulary and interface comparison techniques |

## Install

Claude Code:

```bash
claude plugin marketplace add fulls1z3/skills
claude plugin install fulls1z3-skills@fulls1z3-skills --scope user
```

claude.ai: add this repository as a plugin. The skill is then `fulls1z3-skills:grilling`.

Remove any older `grilling` skill first, so two versions do not compete.

## License

MIT, see [LICENSE](LICENSE). `grilling` is adapted from Matt Pocock's [grilling](https://github.com/mattpocock/skills/tree/main/skills/productivity/grilling) (MIT, copyright 2026 Matt Pocock) at commit `5beb35b040e3de97e54fa9e386d7e42d15c295c2`; its license is kept in [skills/grilling/LICENSE](skills/grilling/LICENSE).

The four additional skills use Matt Pocock's [engineering skills](https://github.com/mattpocock/skills/tree/abeeaf95660ba9e8b7c753eb38f441ca707a8823/skills/engineering). Each directory includes the upstream MIT license. The interview workflows use this plugin's question cards.
