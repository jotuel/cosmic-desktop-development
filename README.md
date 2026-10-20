# COSMIC Desktop Agent Skill

An Agent Skill conforming to the [agentskills.io](https://agentskills.io) and [Zed AI Skills](https://zed.dev/docs/ai/skills) specifications for System76 COSMIC Desktop application development.

This skill equips AI coding assistants (such as Zed Agent, GitHub Copilot, Claude Code, or Gemini) with the domain knowledge, architecture patterns, and automation/profiling scripts required to develop, test, and profile libcosmic applications.

## Installation

Install using the `skills` CLI:
```bash
npx skills add jotuel/cosmic-desktop-development
```

Or for Zed AI:
Clone or link this repository to your Zed skills directory (`~/.config/zed/skills/cosmic` or `.zed/skills/cosmic`).

## Skill Structure

The `cosmic` skill unifies development guidelines, UI automation, and performance profiling into a single skill utilizing progressive disclosure:

* **`SKILL.md`**: Core metadata frontmatter, routing instructions, and quick-reference rules.
* **`references/`**: Detailed domain knowledge and guides loaded on-demand:
  * [`references/development.md`](references/development.md): Architecture (MVU), libcosmic widget styling, theming, config management, and encrypted store troubleshooting.
  * [`references/ui-automation.md`](references/ui-automation.md): Automated Wayland interaction simulation (`wtype`) and screenshot inspection (`cosmic-screenshot`).
  * [`references/profiling.md`](references/profiling.md): CPU hotspots (`samply`) and heap memory profiling (`heaptrack`).
* **`scripts/`**: Executable helper scripts:
  * `scripts/test_ui.sh`: Automated Wayland UI navigation and screenshot capture.
  * `scripts/profile_run.sh`: Automated release-build profiling with `samply` or `heaptrack`.

---

## License
MIT
