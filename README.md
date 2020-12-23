# Instructions

```
git clone https://github.com/tomasdev/ts_project_json_test.git
cd ts_project_json_test
npm install
npm run build
```

### Current output

```
$ npm run build

> test@0.1.0 build /Users/tomas/WORK/ts_project_json_test
> bazel build //...

INFO: Invocation ID: 3e225666-5d0c-4e05-bf1c-e4f122ad5efe
INFO: Analyzed 2 targets (44 packages loaded, 839 targets configured).
INFO: Found 2 targets...
ERROR: /Users/tomas/WORK/ts_project_json_test/BUILD.bazel:3:11: output 'ar.json' was not created
ERROR: /Users/tomas/WORK/ts_project_json_test/BUILD.bazel:3:11: not all outputs were created or valid
INFO: Elapsed time: 14.100s, Critical Path: 3.77s
INFO: 17 processes: 15 internal, 2 darwin-sandbox.
FAILED: Build did NOT complete successfully
```

### Expected

No failures, as this use case seems to be covered by https://github.com/bazelbuild/rules_nodejs/tree/master/packages/typescript/test/ts_project/json ?
