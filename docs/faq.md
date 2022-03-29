# Frequently Asked Questions

### Q: How To Customise Message Display?
```js
// Syntax
conn.sendButton(
      jid, // jid of the user to send the message to
      text, // text to send
      foooter, // footer to send
      buffer, // buffer to send (optional), if you want to send button image, location, etc
      buttons, // buttons to send, example [['text1', 'id1'], ['text2', 'id2']]
      quoted, // quoted message to send (optional)
      options // options to send, example { asLocation: true }
)

// example 
conn.sendButton(m.chat, 'Hello world!', '@BochilGaming', null, [
      ['Hello', 'hello'], ['Bye', 'bye']
])
// example button location
conn.sendButton(m.chat, 'Hello world!', '@BochilGaming', 'https://github.com/BochilGaming', 
      [['Hello', 'hello'], ['Bye', 'bye']], 
      null, { asLocation: true }
)
```

### How to contribute?
1. Fork this repository
2. Change/edit/create what you want. for example you can add features, fix bug, etc
3. Test before making a pull req!!
4. Make a pull req!
5  If your pull req is already in acc/merge, you can delete your branch or you can create pull req again :)
