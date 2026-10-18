# Windows installation — Claude Code

## Option A: install inside one project (recommended first)

1. Extract `elite-interface-design.zip`.
2. Open PowerShell in the project folder where you use Claude Code.
3. Run:

```powershell
New-Item -ItemType Directory -Force .claude\skills | Out-Null
Copy-Item -Recurse .\elite-interface-design .\.claude\skills\elite-interface-design
```

If you extracted the ZIP somewhere else, update the source path in `Copy-Item`.

4. Confirm the core file exists:

```powershell
Test-Path .\.claude\skills\elite-interface-design\SKILL.md
```

Expected result: `True`.

5. Start or restart Claude Code if needed, then ask it to use `elite-interface-design` on a small test task.

## Option B: install for all your projects

The usual personal directory is:

```text
%USERPROFILE%\.claude\skills\elite-interface-design\
```

In PowerShell:

```powershell
$dest = Join-Path $HOME ".claude\skills\elite-interface-design"
New-Item -ItemType Directory -Force $dest | Out-Null
Copy-Item -Recurse .\elite-interface-design\* $dest -Force
Test-Path (Join-Path $dest "SKILL.md")
```

Make sure the source path points to the extracted skill folder. Do not accidentally create an extra nested `elite-interface-design\elite-interface-design\` directory.

## Quick acceptance test

Prompt Claude Code:

```text
Use the elite-interface-design skill. Before changing files, inspect this repository and summarize its stack and constraints. Then create one responsive Arabic RTL dashboard prototype, preserving existing project conventions. Test the available build or checks and report exactly what passed and what could not be verified.
```

If Claude does not detect the skill, check the folder structure, confirm the `SKILL.md` file is at the exact path, and consult the current official Claude Code skills documentation for version-specific behavior.
