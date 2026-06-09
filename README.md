# Ticket-bot-Discord

> **⚠️ This repository is archived and no longer maintained.** The bot was built with discord.py v1 and uses the reaction-based interaction model, which has been superseded by Discord's native buttons and slash commands (discord.py v2+). The code is preserved as-is for reference.
>
> **For forkers:** if you want to modernise this bot, look into [discord.py v2](https://discordpy.readthedocs.io/en/stable/) with `discord.ui.Button` and slash commands via `@app_commands`. The ticket system logic itself is still a valid reference.

---

Ticket message reactive discord bot using cogs.

Based on: [ifisq/discord-ticket-system](https://github.com/ifisq/discord-ticket-system)

Built with [discord.py](https://discordpy.readthedocs.io/).

## Features

- Reaction-based ticket creation — post a message users can react to, which opens a private channel
- Support team management — add/remove roles from the support team
- Role mentions on new tickets — ping the right people automatically
- Ticket transcripts — on close, sends a `.txt` file of the full conversation to all participants
- Clean ticket closing command

## Commands

| Command | Description | Access |
|---|---|---|
| `create_ticket` | Posts the ticket creation message in the current channel | Admin |
| `close` | Closes the ticket channel | Support team |
| `addsupport <role_id> [mentionRole=true]` | Adds a role to the support team | Admin |
| `delsupport <role_id>` | Removes a role from the support team | Admin |
| `addmentionrole <role_id>` | Adds a role to be mentioned on new tickets | Admin |
| `delmentionrole <role_id>` | Removes a role from the mention list | Admin |

## Tech stack

- Python
- discord.py (v1)

## License

[MIT](LICENSE)
