# node-headless-chromium
Install precompiled versions of the Chromium/Chrome [headless shell](https://cs.chromium.org/chromium/src/headless/app/headless_shell.cc) using npm or yarn. Yay.

*Warning*: This is a work-in-progress


## Installation

```bash
yarn add headless-chromium
```


## Supported Platforms

Currently works on:

- [x] Linux Ubuntu x64
- [ ] Windows

## CLI Usage

```bash
headless-chromium
```

## Programatic Usage

```js
import { path, spawn } from 'headless-chromium'

// will print something similar to /Users/marco/.../headless-shell
console.log(path)

// start headless chromium
await spawn(options)

```


## Limitations / Known Issues
- binaries are prebuilt which means you trust that I didn't insert any malicious code into the chrome binaries.
- Building the chrome binary requires accepting the EULA for fonts. By using this package, you agree to also accept the EULA for fonts.


## Previous Art
- https://github.com/Medium/phantomjs
- https://github.com/electron-userland/electron-prebuilt
- https://github.com/kanekotic/any-prebuilt



https://chromium.googlesource.com/chromium/src/+/master/docs/mac_build_instructions.md
http://www.zackarychapple.guru/chrome/2016/08/24/chrome-headless.html
