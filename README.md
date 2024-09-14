# Zephyr Visual Studio Code Development Workspace Configuration
Zephyr Development VisualStudio Code Workspace configuration.

This workspace configuration file was initially based on https://github.com/Nukersson/zephyr_vscode_workspace.git but was reduced to the basics. It also a work in progress so many things still need to be fixed or improved.

# I. Usage description

Here you can find the description of this repository and it's usage. 

**Note:** Currently only `Ubuntu Desktop 24.04.1 LTS` with `zephyr-sdk-0.16.8` were tested!

You're also welcome to make changes on this repository.
Just fork it and provide PR with meaningful changes you need.
I should be able to review it in a couple of days.

## 1. Getting started
Follow this simple steps to simplify your Zephyr development in VSCode:

1. Follow Zephyr's latest [Getting Started Guide](https://docs.zephyrproject.org/latest/getting_started/index.html)
2. Switch to your `zephyrproject` path from terminal:
> cd ~/zephyrproject
3. Clone this repository in your `zephyrproject`:
> git clone https://github.com/sebastianschlupp/ZephyrWorkspace.git
4. Open [Zephyr.code-workspace](https://github.com/sebastianschlupp/ZephyrWorkspace.git) as a workspace in VSCode (be careful: last opened active workspace must be closed):
> File -> Open Workspace...

**Note:** This repository must be placed in your `zephyrproject` folder!

## 2. Workspace Configuration
The [Zephyr.code-workspace](https://github.com/sebastianschlupp/ZephyrWorkspace.git) contains some usefull workspace configuration that helps the user add the relevant useful Extensions as well as organizing the workspace in a helpful folder structure.

For some extensions a reconfiguration is necessary. Please proceed as follows:

1. Configure the `kconfig.zephyr.board` setting inside `Zephyr.code-workspace` for the board that you want to develop for
2. 

## 3. Zephyr Tasks
Use the terminal built into VS Code to execute the main west commands.
**Note:** Remember to activate your .venv before inserting any commands into the command line:
> source ~/zephyrproject/.venv/bin/activate

# II. Folder Structure Description

The Workspace is organized into the following folders:
* Workspace
* AppUnderDev
* BoardUnderDev
* zephyrproject

**Note:** It is assumed that this repository was cloned directly under the `zephyrproject` folder, the app that is being worked on is supposed to be located under `zephyrproject/app` and the custom board that is being developed is located under `zephyrproject/app/boards`. Ideally each of these would point to their own git repository.
