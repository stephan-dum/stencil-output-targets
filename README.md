⚠️This is just a fork of the original [@stencil/output-target](https://github.com/stenciljs/output-targets) repository! The purpose of this repo is to release a faster version of react-output-target till the [PR](https://github.com/stenciljs/output-targets/pull/847) is merged and released.


| Project               | Package                                                                                                              | Version                                                                                                                                            | Documentation                                        |
| --------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| React Output Target   | [`stencil-react-output-target`](https://www.npmjs.com/package/stencil-react-output-target)            | [![version](https://img.shields.io/npm/v/stencil-react-output-target/latest.svg)](https://www.npmjs.com/package/stencil-react-output-target)     | [README](./packages/react/README.md)                 |
| Types Output Target   | [`@stencil/types-output-target`](https://www.npmjs.com/package/@stencil/types-output-target)                         | [![version](https://img.shields.io/npm/v/@stencil/types-output-target/latest.svg)](https://www.npmjs.com/package/@stencil/types-output-target)     | [README](./packages/types/README.md)                 |
| SSR                   | [`@stencil/ssr`](https://www.npmjs.com/package/@stencil/ssr)                                                         | [![version](https://img.shields.io/npm/v/@stencil/ssr/latest.svg)](https://www.npmjs.com/package/@stencil/ssr)                                     | [README](./packages/ssr/README.md)                   |

# Introduction

Integrating web components into existing framework applications can be difficult at times. More about this can be read at https://custom-elements-everywhere.com/. To accommodate the various issues, the Stencil team has created output target plugins to make the process simpler.

Stencil offers output targets for React, Angular, and Vue.

## React

In your React project, you can use the following command to install the output target:

```bash
npm install stencil-react-output-target
```

Update the `stencil.config.ts` file to include the following:

```ts
import type { Config } from '@stencil/core';
import { reactOutputTarget } from 'stencil-react-output-target';

export const config: Config = {
  // ...
  plugins: [
    reactOutputTarget({
      // ...
    })
  ]
  // ...
}
```

Read more about using Stencil components in a React application in our [docs](https://stenciljs.com/docs/react).
