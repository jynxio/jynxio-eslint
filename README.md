## Archive

I like the loose writing style in the three.js source code, which is the reason I created this repository. However, unfortunately:

- I had difficulty porting this configuration to frameworks that use SFC, such as Vue and Astro;
- ESLint officially announced that [they will gradually deprecate all style-related formatters in the future](https://eslint.org/blog/2023/10/deprecating-formatting-rules/);

The former forced me to switch to Prettier because I wanted to maintain a consistent writing style across all projects without spending too much effort on this scaffolding. The latter forced me to completely abandon this repository.

I still like this loose writing style, so let it remain in history.

<br/>

## Overview

This is a loosely styled ESLint configuration that closely follows the style required by the [three.js](https://github.com/mrdoob/three.js/) source code. Please refer to the `.eslintrc.json` file for specific configurations.

When I wrote this ESLint configuration, the latest version number of ESLint official was `8.36.0`.

<br/>

## License

MIT
