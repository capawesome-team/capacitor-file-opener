<p align="center"><br><img src="https://avatars.githubusercontent.com/u/105555861" width="128" height="128" /></p>
<h3 align="center">File Opener</h3>
<p align="center"><strong><code>@capawesome-team/capacitor-file-opener</code></strong></p>
<p align="center">
  Capacitor plugin to open a file with the default application.
</p>

<p align="center">
  <img src="https://img.shields.io/maintenance/yes/2022?style=flat-square" />
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

## Sponsorware

This project is available as **Sponsorware**.

> Sponsorware is a release strategy for open-source software that enables developers to be compensated for their open-source work with fewer downsides than traditional open-source funding models. ([Source](https://github.com/sponsorware/docs))

This means...

- New features will be published as soon as [our GitHub Sponsors goal](https://github.com/sponsors/capawesome-team) is reached.
- Any GitHub sponsor with a [sponsorware tier](https://github.com/sponsors/capawesome-team?frequency=recurring) gets **immediate access** to the latest updates.

## Terms

This project is licensed under the terms of the MIT license.  
However, we kindly ask you to respect our **fair use policy**:

- Please **don't distribute the source code** of the sponsors-only repository. You may freely use it for public, private or commercial projects, privately fork or mirror it, but please don't make the source code public, as it would counteract the sponsorware strategy.
- If you cancel your subscription, you're automatically removed as a collaborator and will no longer have access to the sponsors-only repository. However, **you may use the latest version that's available to you as long as you like**.

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

1. (⭐ Insiders only) Log in to GitHub package registry ([GitHub Docs](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry#authenticating-to-github-packages)) to get pre-access to the latest updates:

   ```
   $ npm login --scope=@capawesome-team --registry=https://npm.pkg.github.com

   > Username: USERNAME
   > Password: TOKEN
   > Email: PUBLIC-EMAIL-ADDRESS
   ```

1. (⭐ Insiders only) In the same directory as your `package.json` file, create or edit an `.npmrc` file to include the following line ([GitHub Docs](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry#installing-a-package)):
   ```
   @capawesome-team:registry=https://npm.pkg.github.com
   ```

1. Install the package:

   ```bash
   npm install @capawesome-team/capacitor-file-opener
   npx cap sync
   ```

   🆘 If you have any problems please [create a GitHub discussion](https://docs.github.com/en/discussions/quickstart#creating-a-new-discussion) in this repository.  
   ⚠️ **Attention**: Be careful not to disclose your npm auth token! If you have any questions (CI configuration etc.) please let us know.

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
