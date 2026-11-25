<p align="center"><img src="https://raw.githubusercontent.com/Codenvi/Codenvi/main/docs/assets/codenvi-icon.png" width="96" alt="Codenvi"></p>

<h1 align="center">Codenvi</h1>

<p align="center">
  Drive Claude Code on your Windows PCs from your Android phone.<br>
  Free, open source and end-to-end encrypted.
</p>

<p align="center">
  <a href="https://codenvi.github.io/Codenvi/">Website</a> ·
  <a href="https://github.com/Codenvi/Codenvi">Repository</a> ·
  <a href="https://github.com/Codenvi/Codenvi/tree/main/docs">Documentation</a> ·
  <a href="https://github.com/Codenvi/Codenvi/issues">Issues</a>
</p>

---

## What is Codenvi?

Send a prompt from your phone to a project on one of your PCs. The PC runs the Claude Code CLI you installed and signed in to yourself, commits the result to a `codenvi-dev` branch and sends the answer back.

- **End-to-end encrypted.** Prompts, replies, project names and commit messages are encrypted with a key only your PC and phone hold. Your server only relays ciphertext.
- **Self-hosted, one owner.** You run your own small server. No accounts, no shared service.
- **No open ports on your PCs.** The Windows and Android apps both connect outbound.
- **Safe by design.** A compromised server can't produce a valid encrypted prompt, so it can't run commands on your PCs.

```
Android app ──HTTPS/WSS──▶ your VPS (nginx → Node.js → PostgreSQL) ◀──HTTPS/WSS── Windows app ──▶ claude -p
```

## Get started

1. Deploy the server to your own VPS.
2. Run `Codenvi.exe` on each Windows PC.
3. Install the Android app and pair it from the PC.
4. Register a project folder and send your first prompt.

Step-by-step instructions are in the [README](https://github.com/Codenvi/Codenvi#getting-started) and the [self-hosting guide](https://github.com/Codenvi/Codenvi/blob/main/docs/self-hosting.md).

## Contribute

Bug reports, ideas and pull requests are welcome. Start with the [contributing guide](https://github.com/Codenvi/Codenvi/blob/main/CONTRIBUTING.md). Please report security problems privately, as described in the [security policy](https://github.com/Codenvi/Codenvi/blob/main/SECURITY.md).

---

<sub>Codenvi is an independent open-source project under the MIT License. It is not affiliated with, endorsed by, or sponsored by Anthropic, PBC. "Claude" and "Claude Code" are trademarks of Anthropic, PBC. Codenvi runs the official Claude Code CLI that you install and sign in to yourself; it never sees or stores your Claude credentials.</sub>
