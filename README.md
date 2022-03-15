# Exercism Rust container

## What this template is for
This template is intended to provide an easy way to create a development environment to solve the tasks of the Exercism Rust track without having to install the required tooling yourself.
Aside from that, the template can be used to track your progress and solutions to the tasks in your own repository.

## Prerequisites
- [Docker](https://www.docker.com/get-started)
- [VS Code](https://code.visualstudio.com)
- [Remote Contianers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## How to use this template
### Create and download the repository
First create your own repository from this template and install the prerequisites mentioned above on your local machine. After that you can clone your created repository in a **named** container volume. 
> **Note**: For performance reasons it is recommended to clone the repository in a named container volume instead of cloning the repository on your local machine and open the folder in the container using a bind mount. 

> **Second note**: Be careful to select a **named** container volume instead of an anonymus volume since the anonymus volume is not preserved when the container is rebuild which could result in data loss. Nevertheless you should regulary push your work to your repository to backup your data outside the container volume.

### Configure CLI
After the first start of a new container you need to configure your exercism CLI. For this execute the following command with your token in the terminal of the container.

You can find your API token on your [setings page](https://exercism.org/settings/api_cli).
```
exercism configure --token=<your-exercism-api-token>
```

### Start with the exercises
The development environment is now set up inside the container and you can start solving some exercises. To do so you can download the exercises using the exercism CLI with the command which is provided for each exercise on the exercism website.
After that you can start editing the downloaded files and run the tests as described in the exercise readme and hints documents. If you have finished your exercise you can submit your solution using the exercism CLI, additionaly you can commit and push your changes to your repository to keep track of your changes.


## Troubleshooting
Sometimes autocomplete does not work properly after downloading a new exercise. To make the autocomplete work also in the new exercise it can help to restart the Language Server. To do so open the command palette with `CMD + SHIFT + P` and search for `Rust Analyzer: Restart server`.


### Container settings
`workspaceFolder` to set the folder path
