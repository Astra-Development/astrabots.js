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
