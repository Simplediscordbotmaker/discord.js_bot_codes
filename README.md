# discord.js bot codes
using discord.js will become a legendary

# config files (config.json)
```json
{
tokens: "your token"
}
```



# Startup bot (index.js)
```js
const Discord = require('discord.js');
const prefix = ">" // for you put anything
const { tokens } = require(`./config.json`); // json file you created it earlier

const client = new Discord.Client({
allowedMentions: {
parse: [`users`, `roles`],
repliedUser: true,
}
intents: [
"GUILDS",
"GUILD_MESSAGES",
"GUILD_PRESENCES",
"GUILD_MEMBERS",
"GUILD_MESSAGE_REACTIONS"
],

});

client.on("ready, () => {
console.log("ready!");
});

client.login(tokens)
```

## Online editors: Replit (Recommended), Heroku, Glitch, etc...
