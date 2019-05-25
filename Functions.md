## Commands list

| Command(s) | Description | Arguments |
| --- | --- | --- |
| `/cal`<br>`/c` | Calculates a given expression. Can also use replies to use previous calculations as input, where the output of the previous calculation can be used in the new `/cal` command using the keyword `ans`.<br>*(Powered by [math.js](https://mathjs.org/))* | **Needed.**<br>`/cal 2+2` = 4 <br>`/cal 2^2` = 4 <br>`/cal pi` = 3.141592653589793<br>`/cal round(ans, 2)` (in reply to previous calculation) = 3.14<br>`/cal ans+2` (without replying to anything) will show "Syntax error".<br>`/cal yo mama` will show "Syntax error". |
| `/countdown`<br>`/cd` | Creates a refreshable countdown to a given time. | **Needed.**<br>`/countdown in 2 hours` will start a countdown to 2 hours from the time the message was sent. |
| `/curr` | Converts between currencies. A list of supported currencies is given [here](http://telegra.ph/List-of-supported-currencies-05-07).<br>*(Powered by [CurrencyLayer.com](https://currencylayer.com/))* | **Needed.**<br>`/curr 10 mvr usd` will convert 10 Maldivian Rufiyaa to US dollars.<br>`/curr .2 vnd` converts 0.2 Vietnamese đồng to a preset list of common currencies. |
| `/flip` | Flips a coin. Shortcut to `/rng d2`. | **Not accepted.** |
| `/forward`<br>`/f` | Forwards a message.<br>**The command must be sent as a reply to another message.** | **Not needed, but accepted.**<br>`/forward in 3 hours` will forward the replied-to message, 3 hours from when the command was sent.<br>`/forward` (without arguments) will do the same immediately. |
| `/help`<br>(`/start`) | Sends a prompt to use other commands, and a link to this page. Default `/start` command also does the same. | **Not accepted.** |
| `/hug`<br>(`/unhug`) | Provides a button to send or unsend virtual hugs. | **Not needed, but accepted.**<br>`/hug Dwayne Johnson` will provide a message customized for The Rock. |
| `/inspire` | Sends an inspirational message.<br>*(Powered by [inspirobot.me](http://inspirobot.me/))* | **Not accepted.** |
| `/meet`<br>`/mpt` | Selects the specified location as the bot's Live Location. Useful for groups using Live Location to meet up.<br>**The command must be sent as a reply to another location message.** | **Not needed, but accepted.**<br>`/meet at 7pm` will set that location as the bot's Live Location until 7pm.<br>`/meet` (without arguments) will do the same for the next 15 minutes by default. |
| `/minesweeper`<br>`/mines` | Starts a game of Minesweeper that uses inline buttons. The game is played on an 8×8 grid with 10 mines. | **Not accepted.** |
| `/mock` | Generates mOCkiNg tExt. Can also use replies to use others' text as input (provided you reply to a text message). | **Needed.**<br>`/mock Some text` will output "SoMe tExT" (cases switching every other character).<br>`/mock -r Some text` will output the text with cases switched randomly. |
| `/ping` | Checks if Kronos is listening. | **Not accepted.** |
| `/pray` | Sends prayer times for Maale for the current day by default. Can also provide prayer times for the next week for any island in the Maldives.<br>*(Powered by [SalatMV](https://play.google.com/store/apps/details?id=mv.salaf.salat))* | **Not accepted.** |
| `/rip` | Provides a button to pay respects to the deceased. | **Not needed, but accepted.**<br>`/rip my dignity` will provide a message customized for "my dignity". |
| `/rng` | Generates random numbers with input specified using [dice notation](https://en.m.wikipedia.org/wiki/Dice_notation). | **Not needed, but accepted.**<br>`/rng 20d98` will roll a 98-sided die 20 times.<br>`/rng` (without arguments) will roll 1d6 by default (a 6-sided die once). |
| `/shame` | Provides a button to shame someone. | **Not needed, but accepted.**<br>`/shame your cow` will provide a message customized for "your cow". |
| `/sticker` | Edits a photo to the dimensions needed to create a Telegram sticker. The returned file can then be forwarded to the [Stickers bot](http://t.me/Stickers).<br>**The command must be sent as a reply to another .jpg or .png file message (NOT a photo message).** | **Not accepted.** |
| `/strike`<br>`/s` | Generates ~~strikethrough text~~. Can also use replies to use others' text as input (provided you reply to a text message). | **Needed.**<br>`/strike example` will output ~~example~~. |
| `/vainglory`<br>`/vg` | Shows information for heroes in [Vainglory](https://www.vainglorygame.com/). | **Not needed, but accepted.**<br>`/vainglory san feng` will provide details for San Feng. |

## Other functions

| Trigger | Description |
| --- | --- |
| `F` or `Oof`<br>(case-insensitive) | Shortcut to `/rip`. Starts with 1 respect already paid by the sender. |
| `T`<br>(case-insensitive) | Sends any one of 29 [Limimin-themed stickers](http://t.me/addstickers/Limimin) at random. |
| `#<hashtag>` | Mentions a predefined list of users within a group, depending on `<hashtag>` and group used in. |
| `/r/<subreddit>` | Provides a link to the mentioned subreddit. Also works with `r/<subreddit>`. |
| `/u/<username>` | Provides a link to the mentioned Reddit user. Also works with `u/<username>`. |

## Admin commands

| Command(s) | Description | Arguments |
| --- | --- | --- |
| `/backup` | Backs up `/forward` queue, which will be imported again at next bot startup. Expected to be run before downtime. | **Not accepted.** |
| `/echo` | Echoes any text that is input. Can also use replies to use others' text as input (provided you reply to a text message). | **Needed.**<br>`/echo _Some_ *text*` will output "\_Some\_ \*text\*".<br>`/echo -m _Some_ *text*` will output "*Some* **text**". |