# NW.js_mod

> Мысли о переходе на Электрон посещали меня, но я был быстрее.

Experimental and more compact modification of [NW.js](https://github.com/nwjs/nw.js) for my projects with aggressive size optimization and some features from [ungoogled chromium](https://github.com/ungoogled-software/ungoogled-chromium) and [cromite](https://github.com/uazo/cromite).

After the unsuccessful experience of using upx, I was curious to try to reduce the size of the binary file on my own, by eliminating many browser components and configuring the compiler for size optimization. This was a good reason to dig into the Chromium source code for interest.

The original idea also included attempt to add browser tabs for [circuitjs1](https://github.com/SEVA77/circuitjs1) but I abandoned this goal.

Selected NW.js version: **0.64.1**.

You can find the build instructions in my drafts: `info/build_*.txt`.

In the basic version (0.64.1-mod1) only the components provided in gn flags are disabled ([more details](/patches/args.gn)). Also `proprietary_codecs=false`, `symbol_level=0` and `v8_symbol_level=0`. Node-nw without icu and openssl. Unnecessary lines from locales have been cleared and `*.info` files have been deleted.

## Downloads:

Non-SDK binaries only!

- [Latest release](https://github.com/SEVA77/nw.js_mod/releases/latest)
- [All Releases](https://github.com/SEVA77/nw.js_mod/releases)

## Credits

* [Chromium project](https://www.chromium.org/Home) and developers
* [NW.js project](https://nwjs.io/) and developers
* [ungoogled-chromium](https://github.com/ungoogled-software/ungoogled-chromium) for some patches and utils
* [Cromite](https://github.com/uazo/cromite) for some patches

## License

NW.js_mod is published under [GNU GPL v3](./LICENSE).





