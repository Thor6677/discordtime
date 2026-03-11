# Discord Timestamp Generator

A simple, fast web utility for generating [Discord timestamp tags](https://discord.com/developers/docs/reference#message-formatting-timestamp-styles) — no frameworks, no dependencies, just a single HTML file.

**Live site:** [discordtime.thunderborn.dev](https://discordtime.thunderborn.dev)

## What it does

Discord's `<t:unix_timestamp:format>` syntax displays times that automatically adjust to each user's local timezone and locale. This tool lets you build those tags without doing the Unix timestamp math yourself.

## Features

- **Three input modes**
  - Local Time (12hr) — enter a date and time in your timezone
  - UTC Time (24hr) — enter a date and time in UTC
  - From Now — specify an offset in days, hours, and minutes from the current time

- **Seven Discord format styles** with live previews
  | Code | Example output |
  |------|----------------|
  | `F`  | Saturday, December 17, 2022 12:34 PM |
  | `f`  | December 17, 2022 12:34 PM |
  | `R`  | 2 hours from now |
  | `d`  | 12/17/2022 |
  | `D`  | December 17, 2022 |
  | `t`  | 12:34 PM |
  | `T`  | 12:34:56 PM |

- **Copy button** — one click to copy the generated tag
- **Share Link** — shareable URL that restores the generated timestamp
- **Quick shortcuts** — Now / In 1 Hour / In 1 Day buttons
- **Timezone selector** — generate tags for any IANA timezone (Local Time mode)
- **Inline validation** — immediate feedback for invalid UTC times

## Usage

Open the site, pick a time mode, enter your date/time, choose a format, and click **Generate Timestamp**. Copy the result directly into Discord.

To share a specific timestamp with someone, click **Share Link** after generating.

## Development

The entire app is a single `index.html` file — no build step required.

```bash
# Clone and open locally
git clone https://github.com/Thor6677/discordtime.git
cd discordtime
open index.html   # or just drag it into a browser
```

Deployed via GitHub Pages with a custom domain configured in `CNAME`.
