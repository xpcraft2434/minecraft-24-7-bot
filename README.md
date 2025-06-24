# Minecraft Online Bot

A Minecraft bot that logs into your server and keeps it online 24/7. It prevents AFK kicks, auto-respawns, auto-reconnects, and supports basic chat commands. Inspired by features from popular open-source AFK/24-7 bots.

## Features
- Stays online 24/7 to keep your server active
- Prevents AFK kick by moving/jumping
- Auto-respawn on death
- Auto-reconnect on disconnect
- Night skipping (if bot has permission)
- Basic chat commands:
  - `;pos` — Get bot's current position
  - `;start` — Enable anti-AFK
  - `;stop` — Disable anti-AFK
- Supports cracked servers with auto-auth (register/login)

## Setup
1. Install [Node.js](https://nodejs.org/) (v14 or higher recommended)
2. Clone or download this repository
3. Run `npm install` to install dependencies
4. Edit `bot.js` and set your server IP, port, and bot username in the `config` section

## Usage
```bash
npm start
```

The bot will connect to your server and stay online. You can control it with chat commands in-game.

## Configuration
Edit the `config` object in `bot.js` to set:
- `host`: Your server IP
- `port`: Your server port (default: 25565)
- `username`: The bot's Minecraft username
- `autoNightSkip`: Set to `true` to skip night (requires permission)
- `antiAfk`: Set to `true` to enable anti-AFK
- `antiAfkInterval`: How often (ms) to perform anti-AFK actions

## Notes
- For cracked servers, the bot can auto-register/login (see `mineflayer-auto-auth`)
- To run 24/7, host the bot on a VPS or cloud service
- The bot will auto-reconnect if kicked or disconnected

## Credits
- [mineflayer](https://github.com/PrismarineJS/mineflayer)
- [mineflayer-auto-auth](https://github.com/PrismarineJS/mineflayer-auto-auth)
- [mineflayer-pathfinder](https://github.com/PrismarineJS/mineflayer-pathfinder)

## License
MIT 
