# elite-interface-design

A reusable Claude Code skill for original, high-quality UI/UX design and frontend implementation.

## Install for the current project

Copy this folder into your project's `.claude/skills/` directory so the final path is:

```text
your-project/
└── .claude/
    └── skills/
        └── elite-interface-design/
            ├── SKILL.md
            ├── README.md
            ├── references/
            └── examples/
```

On macOS/Linux, from the root of your project:

```bash
mkdir -p .claude/skills
unzip elite-interface-design.zip -d .claude/skills/
```

If the ZIP extracts into a folder named `elite-interface-design`, the path is correct. If it extracts files directly into `.claude/skills/`, move them into a folder named `elite-interface-design`.

On Windows PowerShell, from the project root:

```powershell
New-Item -ItemType Directory -Force .claude\skills | Out-Null
Expand-Archive -Path .\elite-interface-design.zip -DestinationPath .\.claude\skills -Force
```

Ensure `SKILL.md` ends up at `.claude/skills/elite-interface-design/SKILL.md`.

## Install as a personal skill

To make it available across projects, place the folder in your Claude Code personal skills directory, normally:

```text
~/.claude/skills/elite-interface-design/
```

On Windows, `~` resolves to your user profile. Check the current Claude Code documentation if your installed version uses a different location.

## Try it

In Claude Code, open a project and ask:

```text
Use the elite-interface-design skill. Review this project first, then design a distinctive, production-minded dashboard for [describe the product]. Preserve existing functionality, define a coherent design system, implement the interface, and test the main workflows. Report exactly what you verified.
```

For an HTML-only preview:

```text
Use elite-interface-design to build an Arabic RTL HTML/CSS/JavaScript prototype for a sales and inventory system. Frontend only, no backend. Make the visible controls functional, use realistic demo data, and provide run/preview instructions.
```

## What this skill does and does not do

- It supplies reusable design and implementation instructions plus reference checklists.
- It does not automatically install browser tools, design software, frameworks, or MCP servers.
- It does not guarantee that Claude can browse the web or visually inspect screenshots; those capabilities depend on the tools available in your environment.
- It does not replace project-specific requirements or testing.
- It cannot guarantee a “world-class” result automatically; it improves consistency by defining a workflow and review standard.

## Updating the skill

Edit `SKILL.md` or the reference files as your preferred design style evolves. Keep the core instructions concise and put detailed guidance in `references/`.
