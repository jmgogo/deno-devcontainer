# Deno Devcontainer! 🦕

<p align="center">
  <a href="https://github.com/jgome284/hello-deno">
    <img src="imgs/hello-deno-banner.png" alt="Logo">
  </a>
</p>
<h3 align="center">Foreword</h3>
<p align="center">
  A Deno dev container setup to try deno on a jupyter notebook.
  <br>
  <a href="https://github.com/jgome284/hello-deno/issues">Report Bug</a>
  ·
  <a href="https://github.com/jgome284/hello-deno/issues">Request Feature</a>
</p>
<br>

## Prerequisites

### Docker

To start, you need to have Docker Engine and Docker Compose on your machine. You can either:

- Install Docker Desktop which includes both Docker Engine and Docker Compose
- Install Docker Engine and Docker Compose as standalone binaries

### VSCode

This devcontainer is setup for development on Visual Studio Code. You should have it installed along with the [remote development pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) to enable the IDE's devcontainers functionality.

There is an official extension for Visual Studio Code called `vscode_deno`. When installed, it will connect to the language server built into the Deno CLI.

Because most people work in mixed environments, the extension does not enable a workspace as Deno enabled by default, and it requires that the *"deno.enable"* flag to be set. (This is already handled in the [settings.json](/.vscode/settings.json) file). If you have your own settings, you can add the setting yourself, or run `Deno: Enable` from the command palette to enable your project.

## Getting Started

Open Docker Desktop to run the Docker daemon, a background process that manages and coordinates Docker containers on your system. On VS Code, start the development container by running `Dev Containers: Rebuild and Reopen In Container` in the command palette. It can be accessed with the keyboard shortcut `ctrl + shift + P` on your keyboard.

Visual Studio will establish a remote connection to the development container. Several extensions are installed in the IDE as development utilities.