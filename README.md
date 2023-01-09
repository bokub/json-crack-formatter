# JSON Crack Formatter

> A fork of the [JSON Formatter Chrome extension](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa) with a [JSON Crack](https://jsoncrack.com/) visualizer.

![2023-01-07_11-31](https://user-images.githubusercontent.com/17952318/211146746-26a73d2a-025e-4199-bda6-b579e4798f47.png)

## Features

- All features from [JSON Formatter](https://github.com/callumlocke/json-formatter)
- Visualize your JSON data in [JSON Crack](https://jsoncrack.com/)

**Some JSON documents for testing it on:**
https://callumlocke.github.io/json-formatter/

## Installation

**Option 1 (recommended)** – Install it from the [Chrome Web Store](https://chrome.google.com/webstore/detail/ioanjonjikjnimckmaobngpeheholkko).

**Option 2** – Install it from source (see below).

**N.B**: If you have installed [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa), you need to uninstall it.

### Development

**Requirements:** [Deno](https://deno.land/) (and [Node](https://nodejs.org/en/) for now).

**Initial setup:**

- Clone repo
- Run `pnpm i` to get TypeScript typings for chrome (or use `npm i` if you prefer)
- Optional: if using VSCode and you need to mess with the Deno build scripts, install the official Deno plugin and set `"deno.enablePaths": ["tasks"]`.

**To build it:**

- Run `bin/build`

**To build and rebuild whenever files change:**

- Run `bin/dev`

**To install your local build to Chrome**

- Open Chrome and go to `chrome://extensions`
- Enable "Developer mode",
- Click "Load unpacked",
- Select the `dist` folder you built above.
