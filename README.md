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
const { Luppux, YamlDatabase, JsonDatabase } = require("luppux.js");
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
# Database Functions

// Docs; https://fivesobes.gitbook.io/five.db/jsondatabase
client.db.set()
client.db.has()
client.db.get() / client.db.fetch()
client.db.add()
client.db.substr()
client.db.push()
client.db.pull()
client.db.delete()
client.db.all()
client.db.findOneAndDelete()

# Prototypes

await Member.bannerURL(options) - options: {dynamic:Boolean,size:Number,format:String} // default:{format:"png",size:512}
Member.hasRole(roleId) // default:null
await User.bannerURL(options) - options: {dynamic:Boolean,size:Number,format:String} // default:{format:"png",size:512}
VoiceChannel.join(options) - options: {selfDeaf:Boolean,selfMute:Boolen} // default:{selfDeaf:false,selfMute:false}
Collection.array() 
Message.delete(ms) - ms: Number // default:null
Value.splitMessage(count) - count: Number // default:null
Array.listRoles(lastMessage) - lastMessage: String // default:"and"
Array.random()
Array.last()

```

# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=blue&repeat=false&width=435&lines=🪄+Example+For+v14)](#)

<h2>.bannerURL()</h2>

```js
// member.bannerURL() or user.bannerURL()

client.on("messageCreate",async(message) => {
if(message.content.includes(".banner")){

let embed = new EmbedBuilder()
.setImage(await message.member.bannerURL({dynamic:true,size:2048}))
.setDescription(`${message.author.tag}`)

message.reply({embeds:[embed});
}
})
```

<h2>.hasRole()</h2>

```js
client.on("messageCreate",async(message) => {

if(message.content.includes(".delete") && message.member.hasRole("roleId")){
message.channel.bulkDelete(100);

}
})
```

<h2>.join()</h2>

```js
client.on("ready",async() => {

let channel = client.channels.cache.get("voiceChannelId");
channel.join({selfDeaf:true,selfMute:false});

})
```

<h2>.delete()</h2>

```js
client.on("messageCreate",async(message) => {
if(message.content.includes("hi")){
message.reply({content:"Hi, How Are You?}).delete(5000);
}
})
```

<h2>.splitMessage()</h2>

```js
let numbers = "123456789....."
let value = numbers.splitMessage(5);
for (message of value) {
console.log(message); // first returning; "12345" , second returning; "678910"; 
}

```

<h2>.listRoles()</h2>

```js
let arrayRoles = ["928259219038302258","852103749228036136","341592492224806914"];
console.log(arrayRoles.listRoles("ands")); // return; <@&928259219038302258>,<@&852103749228036136> ands <@&341592492224806914>
```

<h2>.random()</h2>

```js
let usersId = ["928259219038302258","852103749228036136","341592492224806914"];
console.log(usersId.random()); // return; 852103749228036136
```

<h2>.last()</h2>

```js
let usersId = ["928259219038302258","852103749228036136","341592492224806914"];
console.log(usersId.last()); // return; 341592492224806914
```

<br> <br/>
# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=9D06E6&repeat=false&width=435&lines=Support+%26+Donate)](#)

[![Discord Banner](https://api.weblutions.com/discord/invite/luppux/)](https://discord.gg/luppux)
<br> </br>
<a href="https://www.buymeacoffee.com/beykant" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" width="120px" height="30px" alt="Buy Me A Coffee"></a>

<br> <br/>
# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=9D06E6&repeat=false&width=435&lines=😉+Contributors)](#)
<table>
  <tr>
  <td align="center"><a href="https://github.com/Bes-js"><img src="https://avatars.githubusercontent.com/u/89789101?v=4" width="100px;" alt=""/><br /><sub><b>Five So Beş</b></sub></a><br /><a href="Five So Beş" title="Luppux">⚕️</a></td>
<td align="center"><a href="https://github.com/luluwux"><img src="https://avatars.githubusercontent.com/u/87658293?v=4" width="100px;" alt=""/><br /><sub><b>Lulushu</b></sub></a><br /><a href="Lulushu" title="Luppux">⚕️</a></td>
<td align="center"><a href="https://github.com/Approval-Denial"><img src="https://avatars.githubusercontent.com/u/74969246?v=4" width="100px;" alt=""/><br /><sub><b>Approval</b></sub></a><br /><a href="Approval" title="Luppux">⚕️</a></td>
<td align="center"><a href="https://github.com/utw0"><img src="https://avatars.githubusercontent.com/u/74924310?v=4" width="100px;" alt=""/><br /><sub><b>Luhux</b></sub></a><br /><a href="Luhux" title="Luppux">⚕️</a></td>
  </tr>
</table>
<table>
  <tr>
  <td align="center"><a href="https://github.com/ertucuk"><img src="https://avatars.githubusercontent.com/u/68440024?v=4" width="100px;" alt=""/><br /><sub><b>ertu</b></sub></a><br /><a href="ertu" title="Luppux">⚕️</a></td>
<td align="center"><a href="https://github.com/kaanxsrd"><img src="https://avatars.githubusercontent.com/u/94650814?v=4" width="100px;" alt=""/><br /><sub><b>Lethh</b></sub></a><br /><a href="Lethh" title="Luppux">⚕️</a></td>
<td align="center"><a href="https://github.com/cranedevs"><img src="https://avatars.githubusercontent.com/u/125387403?v=4" width="100px;" alt=""/><br /><sub><b>Crane</b></sub></a><br /><a href="Crane" title="Luppux">⚕️</a></td>
<td align="center"><a href="https://github.com/pikushe"><img src="https://avatars.githubusercontent.com/u/89347562?v=4" width="100px;" alt=""/><br /><sub><b>Piku</b></sub></a><br /><a href="Piku" title="Luppux">⚕️</a></td>
  </tr>
</table>

<br> <br/>
<br> <br/>
# [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=9D06E6&repeat=false&width=435&lines=😑+Eris)](#)

<table>
  <tr>
  <td align="center"><a href="https://github.com/ArviSlayer"><img src="https://avatars.githubusercontent.com/u/69751083?v=4" width="100px;" alt=""/><br /><sub><b>Arvis</b></sub></a><br /><a href="Arvis" title="Luppux">⚕️</a></td>
  </tr>
</table>
