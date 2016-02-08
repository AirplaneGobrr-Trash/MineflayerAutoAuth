# AutoAuth

Minecraft bot auth in servers that don't use `online-mode=true` and require chat authentication. After extending bot will send auth data on `/register` and `/login` messages in chat. Extends [mineflayer](https://github.com/PrismarineJS/mineflayer).

## Install

`npm i mineflayer-auto-auth`

## Usage

```javascript
var mineflayer = require('mineflayer');
var bot = mineflayer.createBot({
  host: "localhost"
  port: 25565
});

require('mineflayer-auto-auth')(bot, 'password');
```

## API

### function(bot, password)

- bot {Object} - mineflayer's bot
- password {String} - password that will be used in login/registration

### function(bot, config)

- bot {Object} - mineflayer's bot
- config {Object} - must have `password` property and could have `logging` property

## License

MIT © [Konstantin Azizov](http://g07cha.github.io)