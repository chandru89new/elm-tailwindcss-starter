# Elm + Tailwindcss starter pack

This is a small starter pack I use to start making apps using Elm as the frontend language and Tailwindcss as the styling framework.

It comes with these things:

- PostCSS: to process your styles and also to minify it when you build the css (using `cssnano`)
- Customized script to build, minify and optimize Elm source code when it's compiled to JS. (`yarn build`)
- PurgeCSS config in TailwindCSS so that styles you don't use from Tailwind are excluded from the final CSS build

## Get started

To get started immediately:
- clone the repo
- run `yarn` in terminal to download packages
- run `yarn build` to build the project
- serve the `./build/index.html` file (using some server like VS Code Live Server or SimpleHTTPServer)

## More things

All commands are terminal commands unless specified otherwise.

### To start the watcher for CSS and Elm files

(This is useful when you're developing something and want a quick writeCode-checkOutput-repeat workflow going.)

```
> yarn dev
```

**Note**: If `yarn dev` complains about permissions, you might want to do `sudo chmod +x ./watcher` so that the `watcher` file is set to be executable by you.

### Where to put all my styles?

In the `./styles/` folder.

### Building for "Production"

`yarn build` takes care of minification of CSS and JS output from Elm.
