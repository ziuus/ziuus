# Noel Paul Tomy

**AI agent & systems engineer.** I build Linux desktop infrastructure in Rust, autonomous agent runtimes, and the tooling that makes both usable from a terminal.

Currently leading [Vanta](https://github.com/ziuus/vanta) — a keyboard-driven terminal dashboard in Rust with a sandboxed WASM extension architecture.

[Portfolio](https://ziuus.runs-on.dev) · [LinkedIn](https://www.linkedin.com/in/ziuus/) · [X](https://x.com/ziusdev) · [Email](mailto:noelyt101@gmail.com)

---

## Flagship

### [Vanta](https://github.com/ziuus/vanta) · Rust · `npm i -g @ziuus/vanta`

Terminal dashboard that replaces the usual stack of one-off tools. One pane, six modes — CPU, memory, disk, network, GPU, processes, plus clock, calendar and a media visualizer. ~3 MB binary, 2–5% CPU, 85+ releases, cross-platform.

The differentiator is the extension architecture: panels are sandboxed WASM modules, so the dashboard is extensible without recompiling. Most monitoring TUIs are static; this is a platform.

### [settings-tui](https://github.com/ziuus/settings-tui) · Rust · `npx settings-tui`

**The missing native control center for Linux.** Every graphical settings app on Linux is a GUI. `settings-tui` speaks to D-Bus, systemd, NetworkManager, BlueZ and PipeWire directly and exposes all of it as a keyboard-first terminal application — Wi-Fi scanning with signal/frequency/security detail, Bluetooth, audio mixer, power profiles, display, services.

What makes it defensible instead of a toy:

- **Transactional engine.** Every mutation runs `READ → MUTATE → READBACK → VERIFY`. Silent failures are the reason people don't trust terminal config tools.
- **Honest capability matrix.** `settings-tui -d` prints per-subsystem support with `[~] [*] [R]` badges. It tells you when your distro doesn't support something instead of pretending.
- **Works headless and over SSH** — the case no GUI settings app can serve.

The existing TUIs in this space (`nmtui`, `wifui`, `wiremix`) each cover exactly one subsystem. There is no unified equivalent, and the whole desktop-settings surface is dominated by the same three GTK/Qt apps.

---

## Tools

| | | |
|---|---|---|
| **[Waiting Game](https://github.com/ziuus/waiting-game)** · Tauri | Transparent full-screen overlay that lives on your desktop and lets you play while builds, CI, and installs run. Linux/macOS/Windows, packaged releases, [live demo](https://waiting-game-site.vercel.app). | ★2 |
| **[Restate MCP Gateway](https://github.com/ziuus/restate-mcp-gateway)** | Production MCP proxy middleware. Wraps tool calls in Restate's durable execution engine for automatic retries, journaling, concurrency shaping, and policy-gated human-in-the-loop approval. | |
| **[Quickshell Todo](https://github.com/ziuus/quickshell-todo)** · QML | Desktop-embedded Wayland task and calendar widget for Hyprland. 0.0% idle CPU, ~26 MB RAM, midnight rollover without restart. | ★3 |
| **[BATMAN](https://github.com/ziuus/batman)** · Shell | Single-file CLI for battery state and Lenovo-style conservation charging mode via sysfs. No dependencies, auditable, packaged as `.deb`. | |
| **[Lindy](https://github.com/ziuus/lindy)** · Tauri | Dual-boot file access. Auto-detects Windows NTFS/exFAT partitions and maps your Windows user folders into Linux without hand-editing fstab. | |
| **[FixVol](https://github.com/ziuus/FixVol)** · Android | Volume control for phones with broken hardware buttons, using the real SystemUI panel instead of a custom overlay. | ★1 |

---

## Also

**Agent infrastructure** — [Zervox](https://github.com/ziuus/Zervox) (autonomous Kubernetes incident remediation, OPA guardrails) · [OmniChat Harness](https://github.com/ziuus/omnichat-harness) · [Synapse](https://github.com/ziuus/Synapse) · [GOAT](https://github.com/ziuus/GOAT)

**Products** — [Orpaq AI](https://github.com/ziuus/orpaq-ai) · [Daily Workspace](https://github.com/ziuus/daily-workspace) · [VoxAssist](https://github.com/ziuus/voxassist) · [Appztore](https://github.com/ziuus/Appztore) · [Journey](https://github.com/ziuus/journey)

**Focus** — AI agents and LLM orchestration · Rust systems and developer tooling · Linux desktop and Wayland · Kubernetes, MCP, cloud infrastructure

---

<sub>Star counts are organic. Nothing here is bought, and nothing here is a client engagement.</sub>