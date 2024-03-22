# Custom Homestar TS Functions

This repo is place to store custom TypeScript functions to be used in [Homestar](https://github.com/ipvm-wg/homestar) workflows.

## Creating new functions

1. Create a new `<function_name>.ts` file in `src/functions`
2. Specify the argument and return types

## Adding a custom function to the [every-cli](https://github.com/everywhere-computer/every-cli)

1. Install the `every` CLI by running `npm i -g @everywhere-computer/every-cli`
2. Run the CLI and point it to your custom function using `every dev --fn <PATH_TO_YOUR_TS_FUNCTION_FILE>`.
