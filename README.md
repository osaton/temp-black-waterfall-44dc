# @cloudflarevitest-pool-workers bug

## Reproduction

Install dependencies and run `npm test` to reproduce the bug.


## Issue

Pages project with `pages_build_output_dir` in `wrangler.toml` fails to run with the following error:

```
Error: Pages doesn't currently support JSON formatted config `/black-waterfall-44dc/wrangler.toml`. Please use wrangler.toml instead.
```

If you comment out the `pages_build_output_dir` in `wrangler.toml`, the tests runs successfully.
