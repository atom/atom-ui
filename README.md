# :sparkles: Atom UI :sparkles:

This is Atom's UI library. Originally forked from Bootstrap `3.3.6`, then merged with some core styles and now tweaked to Atom's needy needs.

> Note: This package gets bundled with Atom and isn't meant to be used outside of the Atom editor. It depends on variables provided by Atom themes.


## Components

Here a list of [all components](https://github.com/atom/atom-ui/blob/master/atom-ui.less). Open the [Styleguide](https://github.com/atom/styleguide) package (`cmd-ctrl-shift-g`) to see them in action and how to use them.

![Styleguide](https://cloud.githubusercontent.com/assets/378023/15767543/ccecf9bc-2983-11e6-9c5e-d228d39f52b0.png)


## Contributing

Because Atom UI isn't a normal Atom package, the "auto-reload" of the Less files in Dev Mode isn't supported. In order to test your changes, do the following:

1. Clone this repo as a sibling to [atom/atom](https://github.com/atom/atom)
2. Change [this import path](https://github.com/atom/atom/blob/master/static/atom.less#L27) to `@import "../../atom-ui/atom-ui.less";`
3. Make some changes
4. Manually reload all styles with `ctrl-shift-cmd-r` (macOS)

If building Atom feels like too much effort, you can also also test (override) changes in your `styles.less` file or DevTools. Just be aware that the source order isn't the same. `atom-ui` gets loaded before all packages and themes.


## Feature requests

If you need something, feel free to open an issue and it might can be added. :v:
