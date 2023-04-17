# @aws-testing/java-sdk

This packages is automatic publishing as a single Jar of [AWS SDK for Java](https://github.com/aws/aws-sdk-java-v2)

It checks daily for a newly released version and automatically publish it to NPM with matching version number.

To get path of `AwsSdkJava.jar` use:

```js
import { createRequire } from 'node:module';
const require = createRequire(import.meta.url);

const sdkJarPath = require.resolve('@aws-testing/java-sdk')
```

Powered by [GitHub Action](../../.github/workflows/npm-publish-aws-sdk.yml)
