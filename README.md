# hyper-reorderable-tabs

> [HyperTerm](https://hyper.is) tabs reordering support plugin

<div align="center">
    <img src="https://raw.githubusercontent.com/hectorqin/hyper-reorderable-tabs/master/hyper-reorderable-tabs.gif">
</div>

## Install

Add `hyper-reorderable-tabs` to the `plugins` list in your `~/.hyper.js` config file.

## Usage

Support Drag&drop [if this pr is merged](https://github.com/zeit/hyper/pull/3197), also support reordering with keyboard shortcuts is available.

To move active tab around, press `alt+left/right arrow` or `ctrl+alt+shift+left/right arrow`, or configure your own shortcuts using config (using [mousetrap](https://craig.is/killing/mice) supported keys):

```javascript
module.exports = {
  config: {
    ...
    hyperTabs: {
      // The height(unit px) of zone over tabs to drag the window
      navMoveable: 0,
      // The hotkeys of move tabs
      hotkeys: {
        moveLeft: 'command+[',
        moveRight: ['command+]', 'r i g h t']
      }
    }
    ...
  }
  ...
}
```

## Thanks

Modified from [hyperterm-tabs](https://github.com/patrik-piskay/hyperterm-tabs)
