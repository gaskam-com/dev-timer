dev-timer / [Exports](modules.md)

# Dev-Timer

![npm](https://img.shields.io/npm/v/dev-timer)
![GitHub top language](https://img.shields.io/github/languages/top/BOT-maKeR-0000/dev-timer)
![npm](https://img.shields.io/npm/dw/dev-timer)
![npm bundle size](https://img.shields.io/bundlephobia/min/dev-timer)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/BOT-maKeR-0000/dev-timer/main)
![GitHub issues](https://img.shields.io/github/issues/BOT-maKeR-0000/dev-timer)
![GitHub Repo stars](https://img.shields.io/github/stars/BOT-maKeR-0000/dev-timer)
![NPM](https://img.shields.io/npm/l/dev-timer)

Dev Timer is a very simple library to help you implement timings in your code. It's designed to stay precise over time.

> ⚠️ This library is currently in Alpha release, it contains a lot of known bugs. Expect many breaking changes. (You should target a specific version)

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

You can easely install it using the command below :

> ⚠️ This library is not yet compatible with imports with script tag.

### npm

```
npm i dev-timer
```

NodeJS usage
```js
const { Timer } = require("dev-timer");
```

### ESM

Dev Timer can be imported as ES modules for browsers that support it. The specifics differ depending on the CDN, but here's a pattern for including the ES module where supported, and falling back to a UMD version for older browsers.

HTML5
```html
<script type="module" src="index.js"></script>
```

JS ( index.js )
```js
import { Timer } from "https://unpkg.com/dev-timer@0.2.10/ES/Timer.js";
```

## Usage

You can find the documentation [here](https://github.com/BOT-maKeR-0000/dev-timer/wiki).
To find more examples, please refer to [examples folder](https://github.com/BOT-maKeR-0000/dev-timer/tree/main/examples) or [step by step examples](https://github.com/BOT-maKeR-0000/dev-timer/wiki/examples).

### Basic Example :

```js
const { Timer } = require('dev-timer');

// Create a new timer instance with a 15 seconds duration
const timer = new Timer(15000); 

timer.start(); // Start the timer

// Add a callback to be called when the timer ends
timer.onEnd = ()=>{
    console.log('Timer ended');
}
```

## Credits

This project was mainly created by me... so... But I would like to thank [Patafix](https://github.com/PatafixPLTX) who helped me to create this README.

But this project was only possible thanks to TypeScript, Javascript, npm and Github <3

## License

Dev Timer's code is licenced under [BSD-3 Clause Licence](https://opensource.org/license/bsd-3-clause/).
You can find the licence file [here](https://github.com/BOT-maKeR-0000/dev-timer/blob/main/LICENSE) too.