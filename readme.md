# Module Resolution Test

A repo to reproduce and debug an issue with node_module resolution in Windows.

## The Issue

In some cases attempting to run this application will throw an exception:

```
Uncaught TypeError: Failed to resolve module specifier "moment". Relative references must start with either "/", "./", or "../".
```

"moment" can be substituted for any other `npm` package as the issue is not related to the `moment` package itself.

### Reproduction Steps

1. Clone this repo
2. Open the repo in a terminal
3. `npm i`
4. `npm run test`
5. `npm run start`

### Expected Results

- The year is {current year}
- Uncaught TypeError

#### Submit your results

Please contact Oliver on Discord if you are a Windows user with a failing result.