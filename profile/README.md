# MachBox

MachBox is the home of the Mach suite. We build desktop-first tools for developers who live in terminals and ticket queues. 

The goal here is simple: build native apps that are actually fast. That means keeping execution local, prioritizing keyboard workflows, and refusing to wrap a slow web UI in an app frame and call it a day.

The tools in this suite share that architecture, but they don't share the exact same rules. We prefer to just be explicit about what requires an account and what doesn't.

---

## The Tools

### [Mach Triage](https://mach-triage.com) (Live)
A local command center for your work queue. It pulls Jira, Linear, and GitHub Issues into one fast, keyboard-driven desktop app so you can avoid browser tab chaos.
* **Model:** Commercial.
* **Account:** Required (for workspace sync and billing).
* **Execution:** Heavy lifting, search, and filtering happen locally on your hardware. 

### [Mach Terminal](https://github.com/MachBox-Dev/mach-terminal) (Late Beta)
A speed-first terminal emulator built on Tauri and Rust. It supports tabs, splits, and AI—but only if you want it to. 
* **Model:** Open Source ([Apache-2.0](https://github.com/MachBox-Dev/mach-terminal/blob/main/LICENSE)).
* **Account:** Never required for the core app.
* **AI:** Completely optional and off by default. Bring your own keys (they stay in your OS keychain) or point it at local Ollama. 

---

## Suite Architecture

```
                    ┌───────────────────────────────┐
                    │        MachBox (suite)        │
                    │ desktop-first, native speeds  │
                    └───────────────┬───────────────┘
                                    │
            ┌───────────────────────┴───────────────────────┐
            ▼                                               ▼
  ┌───────────────────┐                           ┌───────────────────┐
  │    Mach Triage    │                           │   Mach Terminal   │
  │ commercial app    │                           │ open core (OSS)   │
  │ account required  │                           │ no account needed │
  └───────────────────┘                           └───────────────────┘
```

---

## Links

| | |
| --- | --- |
| **Suite** | [machbox.dev](https://machbox.dev) |
| **Mach Triage** | [mach-triage.com](https://mach-triage.com) |
| **Mach Terminal** | [github.com/MachBox-Dev/mach-terminal](https://github.com/MachBox-Dev/mach-terminal) |
| **Terminal principles** | [PRINCIPLES.md](https://github.com/MachBox-Dev/mach-terminal/blob/main/PRINCIPLES.md) |
| **Terminal docs** | [README](https://github.com/MachBox-Dev/mach-terminal#readme) · [runtime contracts](https://github.com/MachBox-Dev/mach-terminal/blob/main/docs/runtime-contracts.md) |

---

## Contributing

We use the Developer Certificate of Origin (DCO) to keep the open-core licensing clean. Just sign your commits with git commit -s. Check the CONTRIBUTING.md in each repo for the ground rules before opening a PR.

If you find a vulnerability, please don't open a public issue. Use GitHub Security Advisories in the repo.
