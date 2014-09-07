# chameleon-dark-syntax theme

Atom syntax theme for HTML, CSS, LESS, SASS, SCSS, JavaScript and JSON. It is a syntax theme only, and will not affect the Atom UI (it works with both the Light UI scheme, and Dark UI scheme). Recommended using with <a href="https://github.com/jesseweed/seti-ui">seti-ui</a>.

### Installation

Run the following command:

```sh
apm install chameleon-dark-syntax
```

Then go to `Atom > Preferences > Themes` and in the `Syntax Themes` dropdown, select `Chameleon Dark` from the list.

![chameleon-dark-syntax theme for Atom](http://i.imgur.com/cTYmwsL.jpg)

### Optional customization for seti-ui theme

These are optional preferences to work with the <a href="https://github.com/jesseweed/seti-ui">seti-ui</a>.

Go to `Atom > Open Your Stylesheet` and in the css file, past the following styles:

```sh
.editor {
  // change cursor to alien green
  .cursor {
    color: #00FF00;
  }
}
// change seti-ui html tree icon to green
.name.icon[data-name*=".html"] {
  &.icon-file-text:before {
    color: #408000;
  }
}
// change seti-ui styles tree icon to purple
.name.icon[data-name*=".less"],
.name.icon[data-name*=".sass"],
.name.icon[data-name*=".scss"],
.name.icon[data-name*=".css"] {
  &.icon-file-text:before  {
    color: #C21BFF;
  }
}

.tab-bar .tab {
  // change seti-ui styles tab icon to purple
  .title[data-name*=".css"]:before,
  .title[data-name*=".less"]:before,
  .title[data-name*=".sass"]:before,
  .title[data-name*=".scss"]:before {
    color: #C21BFF;
  }
  // change seti-ui html tab icon to green
  .title[data-name*=".html"]:before {
    color: #408000;
  }
  // change seti-ui selected tab to gray
  &.active,
  &.active:before {
    border-bottom: solid 4px #555;
  }
}
// change tree view selected to gray
.focusable-panel:focus .selected:before {
	background: #555;
}

```
