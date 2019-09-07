# discordmeme.js
meme.js is an api wrapper for discord bots which aims to provide memes and image gen.

**[Docs](https://solenoapi.netlify.com/memes)**

# Installing
[![NPM](https://nodei.co/npm/discordmeme.js.png)](https://nodei.co/npm/discordmeme.js/)

```js
npm i discordmeme.js
```

## Endpoints [Memes & Image Gen]
_________________________________________________
```
> meme - Provides random memes.
Required:- 
```
_________________________________________________
```
> joke - Provides random joke.
Required:- 
```
_________________________________________________
```
> clydify - Clydify your message.
Required:- text
```
_________________________________________________
```
> trigger - Trigger an image.
Required:- image
```
_________________________________________________
```
> gay - Add gayprideflag on any image.
Required:- image
```
_________________________________________________
```
> wasted - WASTED!
Required:- image
```
_________________________________________________
```
> invert - Invert an image.
Required:- image
```
_________________________________________________
```
> greyscale - Greyscale any image.
Required:- image
```
_________________________________________________
```
> convertImage - Convert text to image.
Required:- text
```
_________________________________________________
```
> qrcodegen - Generates QR Code.
Required:- text
```
_________________________________________________
```
> barcodegen - Generates barcode.
Required:- text
```
_________________________________________________

## NSFW
_________________________________________________

```
> porn - Get porn GIF.
```
_________________________________________________
```
> gonewild - Gonewild Image.
```
_________________________________________________
```
> anal - Get anal pic/GIF.
```
_________________________________________________
```
> pussy - Get image of pussy.
```
_________________________________________________
```
> fourk - Get 4K image.
```
_________________________________________________
```
> ass - Get image of ass.
```
_________________________________________________
```
> hanal - Get image of hanal.
```
_________________________________________________
```
> thigh - Get thigh's image.
```
_________________________________________________
```
> neko - Get picture of Neko.
```
_________________________________________________

## Example

1]
```js
const memer = require("discordmeme.js");

let triggered = await memer.trigger(avatar)
  
    const attachment = new Discord.Attachment(triggered, 'triggered.gif');
    message.channel.send(attachment);

```

2]
```js
const memer = require("discordmeme.js");

let qr = await memer.qrcodegen("Hello World!")
  
    const attachment = new Discord.Attachment(qr, 'qrcode.png');
    message.channel.send(attachment);

```

3]
```js
const memer = require("discordmeme.js");

let neko = await memer.neko()
  
    const embed = new Discord.RichEmbed()
    .setImage(neko)
    message.channel.send(embed);

```
