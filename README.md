# fun-I-guess

A feature-rich WhatsApp bot powered by [Baileys](https://github.com/WhiskeySockets/Baileys), offering group games, utility commands, and experimental RPG elements.

---

## 🚀 Features

- **Group Games:** Play Hangman and more directly in your WhatsApp groups.
- **Session Management:** Start, list, and stop game sessions with simple commands.
- **Customizable Menu:** Choose from multiple menu styles, access owner-only commands, and reload commands on the fly.
- **RPG System (Experimental):** Dive into a text-based dungeon crawler with inventory, combat, and shops.
- **System Utilities:** Check bot/system info, uptime, and more.

---

## 💬 Commands

| Command                    | Description                            |
| -------------------------- | -------------------------------------- |
| `.say <text>`              | Bot repeats your text                  |
| `.ping`                    | Check bot latency                      |
| `.menu`                    | Show all available commands            |
| `.hangman`                 | Start a Hangman game in group chat     |
| `.listsessions`            | List all active sessions (owner only)  |
| `.stopsession <sessionId>` | Stop a session by ID (owner only)      |
| `.sysinfo`                 | Show system information                |
| `.setmenustyle <1\|2\|3>`  | Change menu style (owner only)         |
| `.reload`                  | Reload commands from JSON (owner only) |

---

## ⚙️ Setup

1. **Install dependencies:**
   ```bash
   npm install
   ```
2. **Configure the bot:**  
   Edit `config.json` to set your WhatsApp number, owner numbers, bot name, etc.
3. **Start the bot:**
   ```bash
   npm start
   ```
4. **Pair with WhatsApp:**  
   On first run, enter your WhatsApp number when prompted and follow the pairing instructions.

---

## 📁 File Structure

```
index.js                # Main bot entry point
lib/commands/           # Command handler modules
sessionStore.js         # In-memory session management
databases/morarpg/      # RPG data (items, players, dungeons, etc.)
config.json             # Bot configuration
```

---

## 🛠️ Development

- Add new commands in `lib/commands/` and register them in `lib/commands.json`.
- Owner commands are restricted to numbers in `ownerNumbers` in `config.json`.
- Supports hot-reloading of config and commands.

---

## 🙏 Credits

- Built with [Baileys](https://github.com/WhiskeySockets/Baileys) and [Baileys-mod](https://github.com/nstar-y/bail)
- RPG system inspired by classic dungeon crawlers
- Developer: Dtechy(damy84511@gmail.com)
- Github: [@Dammy8611](https://github.com/Dammy8611)

> **Note:** This project is for educational and personal use. Use responsibly and respect WhatsApp's terms of service.
