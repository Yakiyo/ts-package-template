# TS + npm package template
<div align="center"><img src="https://github.com/Yakiyo/ts-package-template/actions/workflows/build.yml/badge.svg"> <img src="https://github.com/Yakiyo/ts-package-template/actions/workflows/lint.yml/badge.svg"></div>
<div align="center">
<a href="https://gitpod.io/from-referrer/"><img src="./image/gitpod.svg" alt="Open on gitpod https://gitpod.io/from-referrer/"></a>
</div>

This is a simple template repository I use for creating npm packages with typescript.

### Features:
- Write in Commonjs, Build in Commonjs which in turn can be imported in ESM too. (see [test.mjs](./test/test.mjs))
- [Eslint](https://eslint.org) & [Prettier](https://prettier.io/)
- Git [hooks](https://git-scm.com/book/en/v2/ch00/_git_hooks) using [Husky](https://www.npmjs.com/package/husky)
- Use [lint-staged](https://github.com/okonet/lint-staged) to lint and run prettier on staged files before commit
- [Github workflows](./.github/workflows) for building, testing, linting and running prettier.

## Usage
### Locally
[Generate](https://github.com/Yakiyo/ts-package-template/generate) from the template.

Clone it with git and install.
```bash
$ git clone https://github.com/<username>/<repo-name>.git

# use npm if u don't have pnpm
$ pnpm install
```
Edit [package.json](./package.json) as per your project.
Make your package. Remove everything in Readme from here to top. 

# My Awesome Package

Super awesome package description

## Install
```bash
$ npm install pkg-name
# or
$ yarn add pkg-name
# or 
$ pnpm add pkg-name
```
## Usage
```ts
// Commonjs require
const pkg = require('pkg-name');
// ES module import
import pkg from 'pkg-name';
```
## Author
**Package Name** © Author-name. Authored and maintained by Author-name.

Released under [MIT](https://opensource.org/licenses/MIT) License
