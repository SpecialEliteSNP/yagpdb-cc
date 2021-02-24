# Fun Readme
In the fun folder you'll find `counting`, `qotd`, `x-word-story` and `funinfo`. The latter is an optional command that accesses data that's stored when using one of the other CCs.

---

## <u>Counting</u>
### Features:
- Many responses that you can change to your liking.
- Response emoji for correct count
- Optional warning when the latest correct count was changed that confused others
- Milestone notifications for every 100 and 1000
- Only uses **1** database entry

### Setup:
- Set the custom command restrictions to only run in your counting channel
- Set the trigger type to **Regex** and the trigger to: `\A`

### Usage:
- The count starts at 0
- Aftfer that, just type the right number and count together 😊

---

## <u>Question Of The Day</u>
### Features:
- Two-answer detection (will auto-delete)<sup>1</sup>
- A report of the previous QOTD gets send to a channel of choice

### Setup:
- Set the custom command restrictions to only run in your QOTD channel
- Set the trigger type to **Regex** and the trigger to: `\A`

### Usage:
- "@QOTD What is your favourite food?" or "What is @QOTD's fav movie?". As long as you mention your QOTD role, it will work.
- The bot will then remove that message and resend it. (So you don't get pinged when people reply to your message 😉)
- On the next QOTD, the bot will send a report to your report channel with some info on the previous QOTD.

>1 Certain roles can be ignored, e.g. Staff (so they can moderate) and Nitro Boosters.

---

## <u>X-Word-Story</u>
### Features:
- Defaults to **3**, but allows for more or less than 3 words
- It recognises words, provided that they are seperated by spaces
- Has an option to ignore roles. E.g. your staff roles so that they can moderate the story lines

### Setup:
- Set the custom command restrictions to only run in your x-word-story channel
- Set the trigger type to **Regex** and the trigger to: `\A`

### Usage:
- Just type the right amount of words and write a story together 😊

---

## <u>Funinfo</u>
### Features:
- Accesses the data from all commands in this folder and shows it in a nice embed.
- Changable embed colour, defaults to a nice purple

### Setup:
- Set the trigger type to **Regex** and the trigger to:  
`\A-funinfo(?:\s+(?:\d{17,19}|<@!?\d{17,19}>))?\z`
- If your prefix is not `"-"` then change `\A-fun...` to `\A!fun...` for a prefix of `"!"`

### Usage:
- Type `-funinfo <User: ID/Mention>` to see info about [*counting*](#counting), [*qotd*](#question-of-the-day) and [*x-word-story*](#x-word-story). The bot will respond with a nice embed showing the user's count, answers and story lines.