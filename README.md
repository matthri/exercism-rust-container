# Exercism Rust container

## What this template is for
This template is intended to provide an easy way to create a development environment to solve the tasks of the Exercism Rust track without having to install the required tooling yourself.
Aside from that, the template can be used to track your progress and solutions to the tasks in your own repository.

## Prerequisites
- [Docker](https://www.docker.com/get-started)
- [VS Code](https://code.visualstudio.com)
- [Remote Contianers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## How to use this template

## Configure CLI
After the first start of a new container you need to configure your exercism CLI. For this execute the following command with your token in the terminal of the container.

You can find your API token on your [setings page](https://exercism.org/settings/api_cli).
```
exercism configure --token=<your-exercism-api-token>
```

## Troubleshooting
Sometimes autocomplete does not work properly after downloading a new exercise. To make the autocomplete work also in the new exercise it can help to restart the Language Server. To do so open the command palette with `CMD + SHIFT + P` and search for `Rust Analyzer: Restart server`.


### Container settings
`workspaceFolder` to set the folder path
