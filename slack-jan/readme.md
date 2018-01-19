# Azure Functions

This repository contains Azure Functions I use for all kinds of automation tasks.

## Prerequisites for debugging
* Software dependencies:
  * [.NET Core 2.0](https://www.microsoft.com/net/download/core)
  * Install the [Azure Core Function Tools 2.0](https://docs.microsoft.com/en-us/azure/azure-functions/functions-run-local) with the following command
  ```bash
  npm install -g azure-functions-core-tools@core
  ```
  > Note: when installing on Ubuntu, you may need to use `sudo`. On MacOS and Linux, you may need to include the `unsafe-perm` flag, as follows:
  ```bash
  sudo npm install -g azure-functions-core-tools@core --unsafe-perm true
  ```

* vscode extensions:
  * [VS Code Debugger for C#](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)
  * [Azure Funtions](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurefunctions)

## How to debug
Start the local environment by pressing `CTRL-Shift-B` (run task) followed by F5 once started. Make any http request to `http://localhost:7071/api/<function name>`. Add breakpoints where wanted, profit.