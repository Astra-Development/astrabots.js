<p align="center">
  <img src="https://astrabots.xyz/img/logo.png" width="300">
</p>

<p align="center">
  <b>Welcome to Astra Bot List</b>
</p>

<p align="center">
    <br/><br/>
    <a href="https://discord.gg/sQQFSnQhdt" target="_blank">
        <img src="https://img.shields.io/discord/793149744847257600?label=SUPPORT%20SERVER&style=for-the-badge" alt="Discord" />
    </a>
</p>

<p align="center">
  Astra Bot List is an open-source!nt branch may have newer additions/features, but is also potentially more buggy or even insecure. Use at your own risk. If you have any issues, check the FAQs first please.
</p>


## Installation
*If you have trouble with the installation, please feel free to visit our [discord](https://astrabots.xyz/dc) address.*
- `npm i astrabots.js`

```js
const astrabots = require("astrabots.js");
const dbl = new astrabots("TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.serverCount();
  // console.log("Server count posted")
  
  let hasVote = await dbl.hasVoted("714451348212678658");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("779641401482805289")
  console.log(search)
});
```
