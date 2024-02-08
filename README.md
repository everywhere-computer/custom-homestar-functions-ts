# Custom Homestar TS Functions

This repo is place to store custom TypeScript functions to be used in [Homestar](https://github.com/ipvm-wg/homestar) workflows.

## Creating new functions
1. Create a new `<function_name>.ts` file in `src/functions`
2. Specify the argument and return types

## Adding a custom function to the [every-cli](https://github.com/everywhere-computer/every-cli)
1. Install the `every` CLI by running `npm i -g @everywhere-computer/every-cli`
2. Generate the [.wit](https://github.com/WebAssembly/component-model/blob/main/design/mvp/WIT.md) and [.wasm](https://webassembly.org/) files for your custom function by running:
  - `every gen-wasm <ABSOLUTE_PATH_TO_YOUR_TS_FUNCTION_FILE>` (This will soon support relative paths). 
  - If you would like to save your function to IPFS(https://ipfs.tech/) too, you can run `every gen-wasm --ipfs <ABSOLUTE_PATH_TO_YOUR_TS_FUNCTION_FILE>` instead(_This is the recommended command, as it will return a CID that can be used in your Homestar workflow_)