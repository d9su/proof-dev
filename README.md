> **Warning**
> 
> This repo is being archived as I no longer have time to keep up with new features and support requests.
> If you're interested in taking it over, please email or [DM me](https://twitter.com/Dierkens03)

---

<h1 align="center">
  <img width="400" alt="proof" src="./packages/docs/src/media/proof.color.text.svg"/>
</h1>

<p align="center">
  <a href="#"><img alt="@proof-ui" src="https://img.shields.io/npm/v/@proof-ui/core?label=proof-ui"></a>
<!--   <a href="#"><img alt="CircleCI" src="https://img.shields.io/circleci/build/github/intuit/proof"></a><br> -->
  <a href="#"><img alt="TypeScript" src="https://img.shields.io/npm/types/typescript?label=%20"></a>
  <a href="#"><img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-Es6-red"></a>
  <a href="#"><img alt="License" src="https://img.shields.io/github/license/intuit/proof"></a></a><br>
  <a href="#"><img alt="issues" src="https://img.shields.io/github/issues/intuit/proof"></a>
  <a href="#"><img alt="Forks" src="https://img.shields.io/github/forks/intuit/proof?style=social"></a>
</p>




Storybook is a great tool for developing components -- and while simulated and snapshot based testing can get you _pretty_ far, there's no substitution for the real thing. `proof` is a tapable integration testing library for your stories.

## Usage

The quickest way to get started is to use the proof-cli.

```
npm i --save-dev @proof-ui/cli
```

Inspired by [ava](https://github.com/avajs/ava) proof exposes a concise API for authoring tests:

```javascript
import test, { assert } from '@proof-ui/test';

test({ kind: 'Components|Button', story: 'Basic' }, async ({ browser }) => {
  // Use the browser object to test your component
  assert(true === true);
});
```

Or mirror storybook to make it easy to cross-reference tests between files.

```javascript
import { proofsOf } from '@proof-ui/test';
import assert from 'power-assert';

const proofs = proofsOf('Components|Button');

proofs.add('Basic', async ({ browser }) => {
  // Use the browser object to test your component
  assert(true === true);
});
```

### Running your tests

Add proof as a test script in your `package.json`

```javascript
{
  "scripts": {
    "test": "proof"
  }
}
```

And call it

```bash
npm test
```

Proof will run against a local chrome instance by default, but can be configured to target any number of local, remote, or headless browsers.

## Configuration

Create a `proof.config.js` file in your package's root folder or use the `-c`, `--conf` option on the command line to specify a different one.

## Plugins

At it's core, `proof` uses [tapable](https://github.com/webpack/tapable) and exposes many hooks to allow complete control over the entire test life-cycle.

---

## Contributing and Usage

Please read the [contributing](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) document.

Clone the repo:

```
git clone https://github.com/intuit/proof.git
```

Go to the newly cloned repo, and download dependencies:

```
cd proof
yarn
```

Build the project:

```
yarn build
```
