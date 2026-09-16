# FlowIoC-template-blank

A blank Unity project with [FlowIoC](https://github.com/FlowArc/FlowIoC) already in it. Start a
game from this instead of from Unity's own template: the render pipeline is set up, the framework's
setup modules are installed, and the first scene runs.

## Start a project

1. On GitHub press **Use this template**, or clone the repository and point it at a remote of your
   own.
2. Open the folder with the Unity version named in `ProjectSettings/ProjectVersion.txt`. Unity Hub
   picks it when you add the folder.
3. Press Play in the first scene of **File ▸ Build Profiles**' scene list.

Nothing in the project depends on the repository's name. The product's name lives under
**Edit ▸ Project Settings ▸ Player**, like in any Unity project.

## What is inside

- **URP**, with the mobile and PC renderer assets under `Assets/Settings/`.
- **FlowIoC core**, installed from the OpenUPM scoped registry declared in
  `Packages/manifest.json`, at the release the template was last brought up to. Update it from
  **Window ▸ Package Manager ▸ In Project**; the framework refreshes every file it generates on the
  next compile.
- **The setup modules** FlowIoC installs on its first open, under `Assets/Modules/`. Each module
  carries a `MODULE.md` card that says what it is for, and `Assets/Plugins/FlowIoC/MODULES.md`
  lists them all. Further ready-made modules install from **Tools ▸ FlowIoC ▸ Module Library**.
- **Rules and skills for AI assistants** - `AGENTS.md`, `CLAUDE.md` and `.claude/skills/` - written
  and kept current by the package.
- `com.unity.pipeline`, so the Editor can be driven from a terminal with the `unity` CLI. Drop it
  from the manifest if you do not work that way.

## Where to read next

- **Tools ▸ FlowIoC ▸ Wiki** - the framework's Help window, inside the Editor.
- `AGENTS.md` - the architecture rules, the same ones an assistant follows.
- The [FlowIoC repository](https://github.com/FlowArc/FlowIoC) - the full documentation and the
  changelog.

Create modules, commands, models and views from **Tools ▸ FlowIoC** rather than by hand: the
namespace and code-style tooling depends on the shape those generators produce.

## What is deliberately not here

No third-party assets, no sample scene, no packages a blank project does not need. Add what a game
needs on the day it needs it.
