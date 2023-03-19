<p align="center"><br><img src="https://avatars.githubusercontent.com/u/105555861" width="128" height="128" /></p>
<h3 align="center">File Opener</h3>
<p align="center"><strong><code>@capawesome-team/capacitor-file-opener</code></strong></p>
<p align="center">
  Capacitor plugin to open a file with the default application.
</p>

<p align="center">
  <img src="https://img.shields.io/maintenance/yes/2023?style=flat-square" />
  <a href="https://github.com/capawesome-team/capacitor-file-opener/actions?query=workflow%3A%22CI%22"><img src="https://img.shields.io/github/actions/workflow/status/capawesome-team/capacitor-file-opener/ci.yml?branch=main&style=flat-square" /></a>
  <a href="https://github.com/capawesome-team/capacitor-file-opener"><img src="https://img.shields.io/github/license/capawesome-team/capacitor-file-opener?style=flat-square" /></a>
<br>
  <a href="https://www.npmjs.com/package/@capawesome-team/capacitor-file-opener"><img src="https://img.shields.io/npm/dw/@capawesome-team/capacitor-file-opener?style=flat-square" /></a>
  <a href="https://www.npmjs.com/package/@capawesome-team/capacitor-file-opener"><img src="https://img.shields.io/npm/v/@capawesome-team/capacitor-file-opener?style=flat-square" /></a>
  <a href="https://github.com/capawesome-team"><img src="https://img.shields.io/badge/part%20of-capawesome-%234f46e5?style=flat-square" /></a>
</p>

## Maintainers

| Maintainer | GitHub                                    | Social                                        |
| ---------- | ----------------------------------------- | --------------------------------------------- |
| Robin Genz | [robingenz](https://github.com/robingenz) | [@robin_genz](https://twitter.com/robin_genz) |

## Demo

A working example can be found here: [robingenz/capacitor-plugin-demo](https://github.com/robingenz/capacitor-plugin-demo)

| Android | iOS |
| ---------- | ---------- |
| <img src="https://user-images.githubusercontent.com/13857929/185747140-7e59ca70-96c9-4d67-a3b3-8fd9c7eb1546.gif" width="324" /> | <img src="https://user-images.githubusercontent.com/13857929/185747133-62a2b5e5-ff6f-4b30-871c-4c3609db7829.gif" width="266" /> |

## FAQ

1. **Which platforms are supported?**  
   This plugin supports Android and iOS.
1. **Which Capacitor versions are supported?**  
   This plugin supports Capacitor 4.
1. **What do I do when I have a feature request?**  
   Please submit your feature request [here](https://github.com/capawesome-team/capacitor-file-opener/issues/new/choose). We will then review it and possibly put it on our roadmap.
1. **What do I do when I have found a bug?**  
   Bug reports have top priority. Please submit your bug report [here](https://github.com/capawesome-team/capacitor-file-opener/issues/new/choose). We will take a look at it as soon as possible.

## Installation

If you are an [Insider](https://capawesome.io/insiders/#what-is-insiders), see [Getting started with Insiders](https://capawesome.io/insiders/getting-started/?plugin=capacitor-file-opener) and follow the instructions to install the plugin.

If you are **not** an Insider, please install the package from the public npm registry:

```bash
npm install @capawesome-team/capacitor-file-opener
npx cap sync
```

## Configuration

No configuration required for this plugin.

## Usage

```typescript
import { FileOpener } from '@capawesome-team/capacitor-file-opener';

const open = async () => {
  await FileOpener.openFile({
    path: 'file:///var/mobile/Containers/Data/Application/22A433FD-D82D-4989-8BE6-9FC49DEA20BB/Images/test.png'
  });
};
```

## API

<docgen-index>

* [`openFile(...)`](#openfile)
* [Interfaces](#interfaces)

</docgen-index>

<docgen-api>
<!--Update the source file JSDoc comments and rerun docgen to update the docs below-->

### openFile(...)

```typescript
openFile(options: OpenFileOptions) => Promise<void>
```

Open a file with the default application. 

Only available on Android and iOS.

| Param         | Type                                                        |
| ------------- | ----------------------------------------------------------- |
| **`options`** | <code><a href="#openfileoptions">OpenFileOptions</a></code> |

**Since:** 0.0.1

--------------------


### Interfaces


#### OpenFileOptions

| Prop           | Type                | Description                                                                    | Since |
| -------------- | ------------------- | ------------------------------------------------------------------------------ | ----- |
| **`path`**     | <code>string</code> | The path of the file.                                                          | 0.0.1 |
| **`mimeType`** | <code>string</code> | The mime type of the file. If not specified, the mime type will be determined. | 0.0.1 |

</docgen-api>

## Changelog

See [CHANGELOG.md](https://github.com/capawesome-team/capacitor-file-opener/blob/main/CHANGELOG.md).

## License

See [LICENSE](https://github.com/capawesome-team/capacitor-file-opener/blob/main/LICENSE).
