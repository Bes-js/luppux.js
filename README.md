<h6 align="center">
<img src="https://cdn.discordapp.com/attachments/946826067174375494/1108063676486918194/Luppuxx.png" width="500px" height="100px" alt="stats" align="center">
<h6/>

<a href="https://www.buymeacoffee.com/beykant" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" width="120px" height="30px" alt="Buy Me A Coffee"></a>

![npm version](https://img.shields.io/npm/v/luppux.js?color=blue&label=npm%20i%20luppux.js)
![npm info](https://img.shields.io/npm/dw/luppux.js?color=blue)


# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=FF0000&repeat=false&width=435&lines=%E2%9D%94+How+To+Install%3F)](#)

To Install the `luppux.js` module, open a console and write the code below.
<br> </br>
For **npm**
```console
npm i luppux.js
```

For **Yarn**
```console
yarn add luppux.js
```

# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=00EDFF&repeat=false&width=435&lines=%F0%9F%8E%AF+Describing)](#)

For **CommonJS**
```javascript
const { Luppux, YamlDatabase, JsonDatabase }= require("luppux.js");
Luppux({client:client,database:{type:YamlDatabase,databasePath:"./luppuxdb.yml"}});
```

For **ES6**
```javascript
import { Luppux, YamlDatabase, JsonDatabase } from "luppux.js";
Luppux({client:client,database:{type:YamlDatabase,databasePath:"./luppuxdb.yml"}});
```

# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=blue&repeat=false&width=435&lines=✨+Functions+And+Events)](#)

<a href="https://discord.gg/luppux" target="_blank">Click Here To Get Support!</a>
```javascript
# Function

await Member.bannerURL(options) - options: {dynamic:Boolean,size:Number,format:String}
Member.hasRole(roleId) //
await User.bannerURL(options) - options: {dynamic:Boolean,size:Number,format:String}
VoiceChannel.join(options) - options: {selfDeaf:Boolean,selfMute:Boolen}
Collection.array() //
Message.delete(ms) //
Value.splitMessage(count) //
Array.listRoles(lastMessage) //
Array.random() //
Array.last() //

```

# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=blue&repeat=false&width=435&lines=🪄+Example+For+v14)](#)
```js
const { VanityClient }= require("discord-url")
const urlClient = new VanityClient("Self Token","Guild ID",true)

urlClient.setVanityURL("luppux");

urlClient.on("VanitySuccess", async(response) => {
console.log(`URL ${response.vanityURL} Successfully Received!`);
})

urlClient.on('VanityError', async(error) => {
console.log(`An Error Occurred While Retrieving URL!\nError; ${error}`);
})
```

<br> <br/>
# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=9D06E6&repeat=false&width=435&lines=Support+%26+Donate)](#)

[![Discord Banner](https://api.weblutions.com/discord/invite/luppux/)](https://discord.gg/luppux)
<br> </br>
<a href="https://www.buymeacoffee.com/beykant" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" width="120px" height="30px" alt="Buy Me A Coffee"></a>
