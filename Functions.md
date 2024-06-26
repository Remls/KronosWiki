## Table of contents

- [Table of contents](#table-of-contents)
- [User functions](#user-functions)
  - [Commands](#commands)
  - [Text-based functions](#text-based-functions)
  - [Inline queries](#inline-queries)
- [Admin functions](#admin-functions)
- [Ningguang](#ningguang)

## User functions

### Commands

| Command(s) | Description | Arguments |
| --- | --- | --- |
| `/cal`<br>`/c` | Calculates a given expression. Can also use replies to use previous calculations as input, where the output of the previous calculation can be used in the new `/cal` command using the keyword `ans`.<br>*(Powered by [math.js](https://mathjs.org/))* | **Needed.**<br>`/cal 2+2` = 4 <br>`/cal 2^2` = 4 <br>`/cal pi` = 3.141592653589793<br>`/cal round(ans, 2)` (in reply to previous calculation) = 3.14<br>`/cal ans+2` (without replying to anything) will show "Syntax error".<br>`/cal hello` will show "Syntax error". |
| `/countdown`<br>`/cd` | Creates a refreshable countdown to a given time. | **Needed.**<br>`/countdown in 2 hours` will start a countdown to 2 hours from the time the message was sent.<br>`/countdown 90` will start a countdown to 90 minutes from the time the message was sent. |
| `/covid19`<br>`/c19` | Sends statistics about COVID-19 situation in Maldives. | **Not accepted.** |
| `/curr` | Converts between currencies. A list of supported currencies is given [here](http://telegra.ph/List-of-supported-currencies-05-07).<br>*(Powered by [CurrencyLayer.com](https://currencylayer.com/))* | **Needed.**<br>`/curr 10 mvr usd` will convert 10 Maldivian Rufiyaa to US dollars.<br>`/curr .2 vnd` converts 0.2 Vietnamese đồng to a preset list of common currencies. |
| `/delete` | Reply to a photo/video/sticker/GIF to have a 50% chance of deleting that message. | **Not needed.** |
| `/doubt` | Provides a button to doubt. | **Not needed, but accepted.**<br>`/doubt myself` will provide a message customized for "myself". |
| `/download`<br>`/dl` | Downloads from links.<br>The command may also be sent as a reply to another message with one or more links in it. | `/download <YouTube link>` prompts to choose between audio or video.<br>`/download <TikTok link>` downloads the TikTok video. |
| `/flip` | Flips a coin. Shortcut to `/rng d2`. | **Not accepted.** |
| `/forward`<br>`/f` | Forwards a message.<br>**The command must be sent as a reply to another message.** | **Not needed, but accepted.**<br>`/forward in 3 hours` will forward the replied-to message, 3 hours from when the command was sent.<br>`/forward 2` will forward the message in 2 minutes.<br>`/forward` (without arguments) will forward the message immediately. |
| `/help`<br>(`/start`) | Sends a prompt to use other commands, and a link to this page. Default `/start` command also does the same. | **Not accepted.** |
| `/hug` | Provides buttons to send or unsend virtual hugs. | **Not needed, but accepted.**<br>`/hug Dwayne Johnson` will provide a message customized for The Rock. |
| `/inspire` | Sends an inspirational message.<br>*(Powered by [inspirobot.me](http://inspirobot.me/))* | **Not accepted.** |
| `/meet`<br>`/mpt` | Selects the specified location as the bot's Live Location. Useful for groups using Live Location to meet up.<br>**The command must be sent as a reply to another location message.** | **Not needed, but accepted.**<br>`/meet at 7pm` will set that location as the bot's Live Location until 7pm.<br>`/meet 5` will set the Live Location for the next 5 minutes.<br>`/meet` (without arguments) will set the Live Location for the next 15 minutes (default). |
| `/minesweeper`<br>`/mines` | Starts a game of Minesweeper that uses inline buttons. The game is played on an 8×8 grid with 10 mines. | **Not accepted.** |
| `/nice` | Provides a button to nice. | **Not accepted.** |
| `/ping` | Checks if Kronos is listening. | **Not accepted.** |
| `/pray` | Sends prayer times for Maale for the current day by default. Can also provide prayer times for the next week for any island in the Maldives.<br>*(Powered by [SalatMV](https://play.google.com/store/apps/details?id=mv.salaf.salat))* | **Not accepted.** |
| `/pray_my` | Sends prayer times for Kuala Lumpur/Putrajaya for the current day by default. Can also provide prayer times for the next week for any zone in Malaysia.<br>*(Powered by [Waktu Solat](https://waktusolat.app/en))* | **Not accepted.** |
| `/rcg` | Generates a random Cyanide & Happiness comic.<br>*(Powered by [explosm.net](http://explosm.net/rcg))* | **Not accepted.** |
| `/rip` | Provides a button to pay respects. | **Not needed, but accepted.**<br>`/rip my dignity` will provide a message customized for "my dignity". |
| `/rng` | - Generates random numbers with input specified using [dice notation](https://en.m.wikipedia.org/wiki/Dice_notation).<br>- Randomly selects a list of heroes for a game of Vainglory. | **Not needed, but accepted.**<br>`/rng 20d98` will roll a 98-sided die 20 times.<br>`/rng` (without arguments) will roll 1d6 by default (a 6-sided die once).<br>`/rng vg` will select one hero at random.<br>`/rng vg7` will select 7 heroes at random. |
| `/shame` | Provides a button to shame. | **Not needed, but accepted.**<br>`/shame your cow` will provide a message customized for "your cow". |
| `/sticker` | Creates a sticker out of any photo, or a photo out of any sticker.<br>**_For stickers out of photos:_**<br>- **The command must be sent as a reply to a photo.**<br>- If you wish to preserve transparency, the photo must be sent as a **file message**. Only file messages of .JPG or .PNG format are supported.<br>- The created sticker is intended to be for one-time use (by forwarding to the chat you want to send the sticker to).<br>- If you wish to reuse the sticker, an `image_sticker-sized.png` file is provided that is the required resolution to be used in the [Stickers bot](http://t.me/Stickers). You can forward this file as-is to the Stickers bot when prompted, and add the sticker to one of your own packs.<br>- Similarly, an `image_emoji-sized.png` file is also provided, for use in creating custom emoji out of static images using the [Stickers bot](http://t.me/Stickers).<br>**_For photos out of stickers:_**<br>- **The command must be sent as a reply to a sticker.**<br>- The returned file is in .PNG format.<br>- **Known issue:** If this command is used on an animated sticker, you will get an invalid .PNG file. **Workaround:** You could change the extension of the .PNG file to .TGS yourself. The .TGS file is then reusable in chats, as well as input for the [Stickers bot](http://t.me/Stickers). | **Not accepted.** |
| `/time`<br>`/t` | Get current time in multiple cities. | **Not accepted.** |
| `/wordle` | Starts a game of [Wordle](https://www.nytimes.com/games/wordle/index.html). | **Not accepted.** |

### Text-based functions

| Trigger | Description |
| --- | --- |
| `F` or `Oof`<br>(case-insensitive) | Shortcut to `/rip`. Starts with 1 respect already paid by the sender. |
| `X`<br>(case-insensitive) | Shortcut to `/doubt`. Starts with 1 time already doubted by the sender. |
| `Y` or `Shame`<br>(case-insensitive) | Shortcut to `/shame`. Starts with 1 time already shamed by the sender. |
| `*(un)hug(s)*`<br>(case-insensitive) | Shortcut to `/hug`. Starts with 1 hug already sent (or unsent) by the sender. |
| `69`<br>(in any position ... ( ͡° ͜ʖ ͡°) ... of the message) | Shortcut to `/nice`. Starts with 1 nice already sent by the sender. |
| `T`<br>(case-insensitive) | Sends any one of 29 [Limimin-themed stickers](http://t.me/addstickers/Limimin) at random. |
| `#<hashtag>` | Mentions a predefined list of users within a group, depending on `<hashtag>` and group used in. |
| `/r/<subreddit>`<br>`/u/<username>` | Provides a link to the mentioned subreddit or Reddit user. Also works with `r/<subreddit>`/`u/<username>`. |

### Inline queries

Start the text message with `@<bot_username> <prefix>` in any chat to use inline queries. For example, to apply glitch effect to the text "hello", type in `@<bot_username> /g hello`.

| Query | Prefix<br>(case-insensitive) | Description | Options |
| --- | --- | --- | --- |
| Change font | `/f` | Changes font of any text provided. | **_Fonts available:_**<br>- Cursive<br>- Old English<br>- Times New Roman<br>- Times New Roman (italics) |
| Glitched text | `/g` | Applies g̓l̴i᷇t̯ͮc̭̿hͥ͡ effect to any text provided. | **_Strengths available:_**<br>- Weak<br>- Normal<br>- Strong<br>- Illegible |
| Mocking text | `/m` | Generates mOCkiNg tExt from any text provided. | **Alternating:** The cases are switched alternatingly (first uppercase, then lowercase, then uppercase, etc.).<br>**Random:** The cases are switched randomly. |
| Strikethrough | `/s` | Generates ~~strikethrough text~~ from any text provided. | **Full text:** Strikes through the entire text provided.<br>**Part of text:** Strikes through only the part(s) of the text enclosed by tildes (~). There must be an even number of tildes present in the text provided. |

## Admin functions

| Command(s) | Description | Arguments |
| --- | --- | --- |
| `/backup` | Backs up `/forward` queue, which will be imported again at next bot startup. Expected to be run before downtime. | **Not accepted.** |
| `/echo` | Echoes any text that is input. Can also use replies to use others' text as input (provided you reply to a text message). | **Needed.**<br>`/echo _Some_ *text*` will output "\_Some\_ \*text\*".<br>`/echo -m _Some_ *text*` will output "*Some* **text**". |
| `/log` | Fetch `output.log`, for debugging purposes. | **Not accepted.** |

## Ningguang

Helper bot for [Genshin Impact](https://genshin.hoyoverse.com/en) and [Honkai: Star Rail](https://hsr.hoyoverse.com/en-us/).

| Command(s) | Description | Arguments |
| --- | --- | --- |
| `/abyss` | View details about the current Spiral Abyss. | **Not accepted.** |
| `/banner`<br>`/pity`<br>`/wish` | Pity tracker for wishes. | **Not needed, but accepted.**<br>Send command for full helptext. |
| `/craft`<br>`/cr` | Check if you have enough items to craft. | **Needed.**<br>Send command for full helptext. | 
| `/domains`<br>`/dom`/`/sub`<br>`/bosses` | Sends info about domains and bosses. | **Not accepted.** |
| `/events`<br>`/ev` | Sends info about active events. | **Not accepted.** |
| `/power`<br>`/pow`<br>`/p` | Trailblaze power tracker (Honkai: Star Rail). | **Not needed, but accepted.**<br>Send command for full helptext. |
| `/resin`<br>`/res`<br>`/r` | Resin tracker. | **Not needed, but accepted.**<br>Send command for full helptext. |
| `/serenitea`<br>`/pot`<br>`/stp` | Serenitea Pot currency tracker. | **Not needed, but accepted.**<br>`/serenitea 420` will set your current currency value to 420.<br>`/serenitea` will return current status of your Serenitea Pot, as well as when max currency is expected to be hit. |
| `/set_tz` | Set your timezone. | **Needed.**<br>`/set_tz Asia/Singapore` will set your timezone to Asia/Singapore. |
| `/wiki` | Searches the wiki for a matching page.<br>*(Powered by [Fandom.com](https://fandom.com/) and [Honey Impact](https://genshin.honeyhunterworld.com/))*<br>Honey Impact search is also supported through inline queries. | **Not needed, but accepted.**<br>Supplying no search query provides a list of resources. |
