# BatCave

BatCave is an independent skill stack for Claude Code, Codex, OpenCode, Antigravity, and other agent harnesses.

Tell `batcave-mode` your goal and it invokes the workflow that fits: reproduce and root-cause a bug, sketch a design with `architect`, race candidates in `arena`, review a diff with `interrogate`, cut prose with `unslop`. It keeps code concise, simple, and verified, and it reports what it checked.

## What it contains

- Skills: Markdown instructions the agent reads. Public ones appear as `/batcave:<name>` slash commands.
- Agents: `batcave:batcave-agent` and `batcave:comment-sicko`, plus one agent per reasoning-effort level.
- A SessionStart hook that injects the batcave-mode routing mandate unless your `batcave-models.md` sheet turns it off.
- A Pi extension that supplies the subagent, question, and wake-up tools, `/loop`, and the same routing mandate when the repository is installed as a Pi package.
- Local scripts for watching and shipping pull requests, orchestrating multi-phase plans, and auditing worktrees.

## Data handling

batcave has no server or telemetry. Anything its skills ask your agent to read, including session transcripts, goes to your model provider. Scripts run locally, and PR tools use your GitHub CLI login.

## Links

- [Skills, slash commands, runtime setup, and model configuration](https://github.com/Abhiman67/batcave/blob/main/docs/reference.md)
- [Issues and support](https://github.com/Abhiman67/batcave/issues)
- [Security policy](https://github.com/Abhiman67/batcave/blob/main/SECURITY.md)

## License

MIT for this port and its additions, © 2026 Abhishek Chhandak. Original batcave © 2026 Lauren Tan; imported cursor-team-kit skills © 2026 Cursor. See [NOTICE.md](https://github.com/Abhiman67/batcave/blob/main/NOTICE.md).
