# terminal-typer-js

A library for typing out text in a terminal like way.

You are probably better of using [Typer-js](https://www.npmjs.com/package/typer-js) for any real projects, it has a ton of more features.

The reasons I built this was because I wanted to learn some more JS.

# Usage

```javascript
let element = document.getElementById('terminal-text');
let tt = new TerminalTyper(element);
tt.instant('<p>Hello World</p>'); // Add text instantly
tt.type('<p>This text is typed out to the element</p>').then(async (tt) => { // Add typed text
  console.warn('tt.type() is done. Now sleep for one second.');
  tt.sleep(1000).then(tt => {
    console.warn('Slept for one second.');
  });
});
```

# Todo

- Convert to module
