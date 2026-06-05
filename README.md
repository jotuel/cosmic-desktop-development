# COSMIC Desktop Agent Skills

A collection of Agent Skills conforming to the [agentskills.io](https://agentskills.io) and [Zed AI Skills](https://zed.dev/docs/ai/skills) specifications for System76 COSMIC Desktop application development.

These skills are designed to equip AI coding assistants (like Zed Agent, GitHub Copilot, or Gemini) with the precise domain knowledge and execution scripts required to develop, test, and profile libcosmic applications.

## Included Skills

### 1. `cosmic-development`
* **Description**: Best practices, guidelines, Model-View-Update (MVU) pattern, widget styling, and lazy store decryption troubleshooting for System76 COSMIC desktop development.
* **Installation**:
  ```bash
  npx skills add jotuel/cosmic-skills/cosmic-development
  ```

### 2. `cosmic-ui-automation`
* **Description**: Automate, navigate, and capture visual screenshots of native COSMIC/Wayland application layouts during UI/UX inspections.
* **Installation**:
  ```bash
  npx skills add jotuel/cosmic-skills/cosmic-ui-automation
  ```

### 3. `cosmic-profiling`
* **Description**: Profile performance, memory heap usage, and execution hotspots of native COSMIC/Wayland applications under automated load.
* **Installation**:
  ```bash
  npx skills add jotuel/cosmic-skills/cosmic-profiling
  ```

---

## Folder Structure

Each skill folder contains:
* `SKILL.md`: The core metadata frontmatter and agent instruction manual.
* `scripts/`: Executable utility scripts (like automated test runners or profilers) that the agent can execute directly under the sandbox.

---

## License
MIT
