# v0.3.4 (Thu Oct 20 2022)

#### 🐛 Bug Fix

- Expose enabled flag on applitools plugin [#80](https://github.com/intuit/proof/pull/80) (thomas_marmer@intuit.com)
- Expose enabled flag on applitools plugin (thomas_marmer@intuit.com)

#### Authors: 1

- Thomas Marmer ([@tmarmer](https://github.com/tmarmer))

---

# v0.3.2 (Thu Oct 13 2022)

#### 🐛 Bug Fix

- Allow applitools to resize browser using capabilities [#78](https://github.com/intuit/proof/pull/78) (thomas_marmer@intuit.com)
- Allow applitools to resize browser using capabilities. Fix issues with applitools test failures (thomas_marmer@intuit.com)

#### Authors: 1

- Thomas Marmer ([@tmarmer](https://github.com/tmarmer))

---

# v0.3.1 (Wed Oct 12 2022)

#### 🐛 Bug Fix

- Preemptively resize browser in ApplitoolsPlugin [#77](https://github.com/intuit/proof/pull/77) (thomas_marmer@intuit.com)
- Update applitools plugin to allow browsers to run some JS before screenshots are taken (thomas_marmer@intuit.com)

#### Authors: 1

- Thomas Marmer ([@tmarmer](https://github.com/tmarmer))

---

# v0.3.0 (Wed Jul 27 2022)

#### 🚀 Enhancement

- Update core dependencies [#76](https://github.com/intuit/proof/pull/76) (thomas_marmer@intuit.com)

#### 🐛 Bug Fix

- Update core dependencies and fix resulting errors (thomas_marmer@intuit.com)

#### Authors: 1

- Thomas Marmer ([@tmarmer](https://github.com/tmarmer))

---

# v0.1.4 (Tue Aug 11 2020)

#### 🐛 Bug Fix

- Add dep for selenium-webdriver (used by applitools) [#53](https://github.com/intuit/proof/pull/53) ([@adierkens](https://github.com/adierkens))
- Add dep for selenium-webdriver (used by applitools) ([@adierkens](https://github.com/adierkens))

#### Authors: 1

- Adam Dierkens ([@adierkens](https://github.com/adierkens))

---

# v0.1.3 (Tue Aug 11 2020)

#### 🐛 Bug Fix

- Update applitools version in the plugin [#52](https://github.com/intuit/proof/pull/52) ([@adierkens](https://github.com/adierkens))
- Update applitools to latest ([@adierkens](https://github.com/adierkens))

#### Authors: 1

- Adam Dierkens ([@adierkens](https://github.com/adierkens))

---

# v0.1.0 (Wed Jul 01 2020)

### Release Notes

_From #36_

**🔥 Breaking 🔥**
* Upgrades webdriverio to version 6 (up from 4). This includes changing the API for the `browser` object passed to tests. See https://v6.webdriver.io/ for API changes. 
* Removes the `@proof-ui/storybook` package and the configuration step. Stories are now gathered using storybook directly; and no changes or registration code is required from clients to run tests.
* Removes the inclusion of `power-assert` in favor of users providing their own assertion library. 

**Features**

* Add ability to change the name of the tests using the `test()` API. 


#### Internal Changes

- Updates all dependencies to latest versions
- Swap `xo` to `eslint`

Fixes #26 
Fixes #27

**Canary Release** - `0.0.21-canary.b590b95.0`

---

#### 🔨 Breaking Minor Change

- webdriverio upgrade [#36](https://github.com/intuit/proof/pull/36) ([@adierkens](https://github.com/adierkens))

#### 🐛 Bug Fix

- Fix types ([@adierkens](https://github.com/adierkens))
- Get applitools plugin working ([@adierkens](https://github.com/adierkens))
- Swap to eslint. run prettier on everything ([@adierkens](https://github.com/adierkens))

#### Authors: 1

- Adam Dierkens ([@adierkens](https://github.com/adierkens))
