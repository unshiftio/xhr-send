# xhr-send

A cross-browser implementation for sending data over the supplied XHR
connection.

## Installation

```
npm install --save xhr-send
```

## Usage

The module requires 3 arguments:

- `xhr` The reference to your constructed `XMLHTTPRequest` instance.
- `data` The data that needs to be send.
- `fn` Completion callback that receives the error as first argument.

```js
var send = require('xhr-send');

send(xhr, 'data', function (err) {
  if (err) return console.error('failed to send because of reasons', err);

  console.log('send without any isseus.');
});
```

## License

MIT
