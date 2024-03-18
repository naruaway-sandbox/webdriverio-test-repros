# webdriverio-test-repros

This is to verify https://github.com/webdriverio/expect-webdriverio/pull/1496

I ran `npm init wdio@latest ./mocha-wdio-demo` and `npm init wdio@latest ./jasmine-wdio-demo` to generate projects with mocha and jasmine respectively.


Type checking behavior can be verified via:
```
(cd jasmine-wdio-demo && npm ci && ./node_modules/.bin/tsc --noEmit)
(cd mocha-wdio-demo && npm ci && ./node_modules/.bin/tsc --noEmit)
```
