# recruitment-selection-process

Designs a human-owned candidate selection process with job evidence and structured decision gates.

It produces:

- **Candidate Selection Process:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Recruitment Selection Process playbook](https://www.andrewluxem.com/playbooks/recruitment-selection-process). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/recruitment-selection-process.git
cp -r recruitment-selection-process/skills/recruitment-selection-process ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r recruitment-selection-process/skills/recruitment-selection-process ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/recruitment-selection-process
/plugin install recruitment-selection-process@recruitment-selection-process
```

For clients that install from an archive, use the versioned [recruitment-selection-process v1.0.0 ZIP](https://www.andrewluxem.com/downloads/recruitment-selection-process-v1.0.0.zip).

## Invoke it

```text
Design the candidate selection process for this role
Use the recruitment-selection-process skill.
```

Naming the skill is always valid: `use the recruitment-selection-process skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/recruitment-selection-process/
  assets/candidate-selection-process-template.md
  LICENSE.md
  meta.yaml
  references/selection-process-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/recruitment-selection-process/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/recruitment-selection-process/LICENSE.md](skills/recruitment-selection-process/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.
