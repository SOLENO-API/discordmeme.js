# discordmeme.js
meme.js is an api wrapper for discord bots which aims to provide memes and image gen.

# Installing
[![NPM](https://nodei.co/npm/discordmeme.js.png)](https://nodei.co/npm/discordmeme.js/)

```js
npm i discordmeme.js
```

## Endpoints
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