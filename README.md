# @sfn-testing/core

This packages is automatic publishing of Java version of [StepFunction Local](https://docs.aws.amazon.com/step-functions/latest/dg/sfn-local-jar.html)

It checks daily for a newly released version and automatically publish it to NPM with matching version number.

To get path of `StepFunctionsLocal.jar` use:

```js
import { createRequire } from 'node:module';
const require = createRequire(import.meta.url);

const jarPath = require.resolve('@sfn-testing/core')
```

Powered by [GitHub Action](./.github/workflows/npm-publish.yml)