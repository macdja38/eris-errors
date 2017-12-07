Constants companion for eris including the error codes expressed by the .code property of an error.

This library allows for human readable and IDE completed error codes.

For example

```js
const EE = require("eris-errors");
const Eris = require("./index");
const eris = new Eris("token", {restMode: true});
eris.getRESTChannel("117454468076797959").catch(error => {
    if (error.code === EE.DISCORD_RESPONSE_UNKNOWN_CHANNEL) {
      // handle error
    }
});
```

A full list of implemented errors can be found [here](https://github.com/macdja38/eris-errors/blob/master/errors.js)
A full list of discord errors and their descriptions can be found [here](https://discordapp.com/developers/docs/topics/response-codes)