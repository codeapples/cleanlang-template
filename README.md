## cleanlang-template

#### Description
This is a basic template for development in **Clean** language using vscode.

This template uses a devcontainer which requires [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension, you should get a pop-up about it if you don't have it installed as soon as you open this repository in vscode. Docker is also required, instructions to install Docker are provided in extension's description.

Dependency management and building is done via `Nitrile` package manager. If you are unfamiliar with it you can find documentation [here](https://clean-and-itasks.gitlab.io/nitrile/).

#### Building project
Template comes with some preconfigured tasks, so you can use `Shift+Alt+B` to start a build task in vscode.

Manually, you can build using `nitrile build` command.

Building options can be configured in `nitrile.yml` config file.

#### Language server
Dev container comes with a preinstalled language server [Eastwood](https://gitlab.com/top-software/eastwood). [Clean](https://marketplace.visualstudio.com/items?itemName=TOPSoftware.clean-vs-code) extension should be installed inside dev container in order for language server to work.

Mind that `Eastwood` requires you to list all source directories in `eastwood.yml` config file, including external libraries. So if you add more dependencies to your project make sure to specify correct path to the dependency's source code.

