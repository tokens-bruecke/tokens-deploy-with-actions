# Automate design tokens deployment with Github actions

An example repo for design tokens auto-deploy. The repo is using Github actions, [Style Dictionary](https://github.com/amzn/style-dictionary) and tokens-bruecke [style dictionary utils](https://github.com/tokens-bruecke/sd-utils).

## How it works

In Figma, when you're using [TokensBrücke](https://www.figma.com/community/plugin/1254538877056388290/TokensBr%C3%BCcke) and push your design tokens to Github, the Github action will be triggered and will generate the design tokens for you. The design tokens will be available in the `lib` folder.

In `build.js` you can see how the tokens are generated. The `build.js` file is using the `tokens-bruecke` utils to generate the `style-dictionary` package to generate the tokens.

In `.github/workflows/build-tokens.yml` you can see the Github action that is triggered when you push your tokens to Github.

## Refs

- [TokensBrücke Figma plugin](https://www.figma.com/community/plugin/1254538877056388290/TokensBr%C3%BCcke)
- [TokensBrücke Style Dictionary utils](https://github.com/tokens-bruecke/sd-utils)
- [Style Dictionary](https://github.com/amzn/style-dictionary)
