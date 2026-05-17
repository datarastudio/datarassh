# DataraSSH

**A native SSH client for macOS and Windows — terminals, SFTP, port forwarding, and tmux, all in one polished desktop app.**

DataraSSH is part of the [Datara](https://datara.studio) suite of developer tools.

---

## Features

### SSH Connections
- Save and manage an unlimited number of SSH hosts
- Connect with **password**, **key file** (with or without passphrase), or **SSH certificate** authentication
- **Jump / bastion host** support — route connections through an intermediate server
- Automatic host fingerprint verification with a persistent trust store
- Test a connection before saving it
- Export and import host configurations
- Deep link support via the `datara-ssh://` URL scheme

### Terminal Emulation
- Full **PTY terminal** sessions with resize support
- Open **multiple independent terminal windows** per host simultaneously
- **Local terminal** — open a PTY on your own machine from the same interface
- Send input and resize events in real time

### tmux Integration
- Detect tmux availability on the remote server
- List, create, rename, and kill tmux sessions
- Attach to an existing session and split windows — directly from the UI

### SFTP File Manager
- Browse the remote filesystem with a full directory listing
- Read, write, create, rename, and delete files and directories
- Upload and download files with progress reporting
- Set permissions with `chmod` (including recursive, files-only, or directories-only modes)
- Change ownership with `chown` (recursive)
- Compress and decompress files: **zip**, **gzip**, **unzip**, **gunzip**, **untar**
- Browse your local filesystem alongside remote files for drag-and-drop style workflows

### Port Forwarding
- Create and start **local port forward** tunnels
- Save forwarding configurations per host for one-click reuse
- List and stop all active forwards

### Snippet Manager
- Save reusable SSH commands as named snippets
- Insert snippets into any open terminal

### Security
- All sensitive host data (passwords, key passphrases) is encrypted at rest
- App-level secure password lock with bcrypt verification
- IPC integration with DataraDB uses a loopback-only server with HMAC-derived tokens — no credentials are ever exposed

### Datara Suite Integration
- Optional **DataraDB integration** — DataraDB can read your saved SSH hosts directly so you can reuse them as SSH tunnels without re-entering credentials

---

## Platform Support

| Platform | Architecture |
|----------|-------------|
| macOS    | Apple Silicon (arm64), Intel (amd64) |
| Windows  | amd64, arm64 |

---

## Download

Pre-built installers are available on the [Releases](https://github.com/datarastudio/datarassh/releases) page.

- **macOS** — signed and notarized `.dmg`
- **Windows** — NSIS `.exe` installer (amd64 and arm64)

---

## Pricing

DataraSSH is **free**. There are no connection limits, no feature paywalls, and no subscription required.

---

## Part of the Datara Suite

DataraSSH works seamlessly alongside **DataraDB** — enable the integration in Settings and DataraDB will automatically discover your saved SSH hosts to use as database tunnels.

---

## License

DataraSSH is proprietary software. All rights reserved. © Datara.
