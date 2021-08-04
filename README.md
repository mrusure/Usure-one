
## Installation
*If you have trouble with the installation, please feel free to visit our [discord](https://discord.gg/m5vUJVztpt) address.*
- `npm i usure-api`

#### 1. Where can I get Usure.one api?
  Ans: [JavaScript](https://www.npmjs.com/package/disbots-xyz)

#### 2. How do I install it?
  Ans: JavaSciprt: npm i disbots-xyz or npm install disbots-xyz

#### 3. Does it have any GitHub Repository?
  Ans: Yes It Is [Here](https://github.com/mrusure/Usure-api)

#### 4. What is it's uses?
  Ans: To get the daily vote count, server count and information about your bot.
Examples:  avatar, botID, discriminator, shortDescription, prefix, votes, serverCount, ownerID, owner, co-owners, tags, longDescription, certificate etc.

#### 5. How can I get my bot's server count?
  `Ans: JavaScript:`
```js
const disbots = require("disbots-xyz");
const dbl = new disbots("TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.serverCount();
  console.log("Server count posted")

```

#### 6. How can I get my bot's vote count?
  `Ans:`
```js
let hasVote = await dbl.hasVoted("Your-bot-id");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("Your-bot-id")
  console.log(search)

```

#### 7. Full Example?
  `Ans:`
```js
const disbots = require("disbots-xyz");
const dbl = new disbots("TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.serverCount();
  console.log("Server count posted")
  
  let hasVote = await dbl.hasVoted("your-bot-id");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("Your-bot-id")
  console.log(search)

  /* SearchResults
  {
    avatar: '',
    botID: '',
    username: '',
    discrim: '',
    shortDesc: '',
    prefix: '? [changable]',
    votes: 25,
    ownerID: '',
    owner: '',
    coowners: [ '' ],
    tags: [ 'Moderation', 'NSFW', 'Music' ],
    longDesc: longDesc,
    certificate: 'Certified'
  }
  */
});

```
# Questions?
Come talk to us here:

[![Usure.one](https://discord.com/api/guilds/870401233771429908/embed.png?style=banner1)](https://discord.usure.one)
