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
.editor .cursor {
  color: #00FF00;
}
.name.icon[data-name*=".html"].icon-file-text:before {
  color: #408000;
}
.tab-bar .tab .title[data-name*=".css"]:before,
.tab-bar .tab .title[data-name*=".less"]:before,
.tab-bar .tab .title[data-name*=".sass"]:before,
.tab-bar .tab .title[data-name*=".scss"]:before,
.name.icon[data-name*=".less"].icon-file-text:before,
.name.icon[data-name*=".sass"].icon-file-text:before,
.name.icon[data-name*=".scss"].icon-file-text:before,
.name.icon[data-name*=".css"].icon-file-text:before  {
  color: #C21BFF;
}
.tab-bar .tab .title[data-name*=".html"]:before {
  color: #408000;
}
.tab-bar .tab.active,
.tab-bar .tab.active:before {
  border-bottom: solid 4px #555;
}
```
