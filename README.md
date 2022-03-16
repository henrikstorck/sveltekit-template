# SvelteKit Template

This repository contains a basic template for developing web applications with Svelte Kit.

## Setup

Create a repository based on this template using [this link](https://github.com/henrikstorck/sveltekit-template/generate).

Change the project name in the [package.json](package.json#L2) file.

## Configuration

This template project was set up using [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte). (As of Feb 3rd 2022)

```bash

npm init svelte@next sveltekit-template

```

The setup was configured using the following decisions:

* Which Svelte app template? **Skeleton project**
* Use TypeScript? **Yes**
* Add ESLint for code linting? **Yes**
* Add Prettier for code formatting? **Yes**
* Add Playwright for browser testing? **Yes**

## Additional features

### Visual Studio Code Devcontainer

This repository includes configuration files for local dev containers using Visual Studio Code.

The development container already includes everything required to get started:
* Node v16.x
* Playwright installation + browser dependencies
* Git
* Visual Studio Code extensions
  * [Svelte for VS Code](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode)
  * [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  * [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  * [Playwright Test for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-playwright.playwright)

**Prerequisites:**
* Docker
* Visual Studio Code
* "Remote - Container" Extension for Visual Studio Code 
* WSL & "Remote - WSL" Extension for Visual Studio Code  (Recommended - Windows only)

**Steps:**

* *Recommended - Windows only: Make sure the repository is placed in your WSL filesystem*
* Navigate to the repository folder and open it in Visual Studio Code using the shell command `code .`
* Once Visual Studio Code prompts you *Folder contains a Dev Container configuration file*, click *Reopen in container*

For detailed informations on how to use dev containers, visit the official [Visual Studio Code Documentation](https://code.visualstudio.com/docs/remote/containers).

___

### VS Code Debug Configuration

This repository contains a basic Svelte debug configuration in the [launch.json file](/.vscode/launch.json), which starts the svelte development server, opens and attaches to your chrome browser and terminates the development server when the browser is closed or the debug session is stopped.
