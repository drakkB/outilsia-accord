# Accord by OutilsIA

**Accord** is a free native Rust desktop & CLI cockpit that unifies, measures, cleans and synchronizes your **Model Context Protocol (MCP)** servers across all your AI CLIs on **Windows and WSL/Linux**.

Official download page & documentation: **https://outilsia.fr/telecharger-accord** · All OutilsIA apps: **https://outilsia.fr/telecharger**

## Highlights (`v0.4.0`)

- **Unified Windows + WSL MCP Matrix**: simultaneously reads Claude Code (Windows & WSL), Codex (Windows & WSL), Gemini / Antigravity, OpenCode, Cursor (Windows & Linux), and Grok Build.
- **Context-token weight analyzer**: probes stdio MCP servers (`initialize` + `tools/list`) to measure latency, tool count, and exact estimated context-window tokens per tool — plus fast TCP reachability (`UP` / `DOWN`) for HTTP MCP endpoints.
- **1-click drift alignment & non-destructive ON/OFF toggles**: aligns drifting servers across CLIs (with automatic `C:\...` ↔ `/mnt/c/...` translation and `wsl.exe` wrapping for Linux binaries on Windows Cursor), always creating `.bak_accord_*` backups with built-in 2-click rollback.
- **Win32 + WSL zombie process detector**: finds duplicate MCP processes and RAM usage, with dry-run preview and 2-click cleanup.
- **Secret-free `accord.toml` manifest**: exports your MCP stack without ever reading, logging, or exporting environment variable secret values.
- **Built-in read-only meta-MCP server (`accord --mcp-stdio`)**: 5 tools (`accord_doctor`, `accord_list_servers`, `accord_zombies`, `accord_measure_weight`, `accord_export_manifest`) with an anti-recursion guard so your AI agents can inspect running MCPs.

## Downloads (`0.4.0`)

- **Official page**: https://outilsia.fr/telecharger-accord
- **Windows x64 (ZIP · 3.5 MB)**: https://outilsia.fr/download/accord/0.4.0/windows
- **Windows x64 (Portable EXE · 7.7 MB)**: https://outilsia.fr/download/accord/0.4.0/windows-portable
- **Linux x64 (tar.gz · 5.5 MB)**: https://outilsia.fr/download/accord/0.4.0/linux
- **SHA-256 & manifest**: https://outilsia.fr/static/downloads/accord/0.4.0/SHA256SUMS.txt

> Note: Windows executables are not Authenticode-signed yet; verify checksums against `SHA256SUMS.txt`.

---

Built in France by Chris Drakkeng — **OutilsIA** ([outilsia.fr](https://outilsia.fr)), the software brand of [ScoreZenith](https://scorezenith.com).
