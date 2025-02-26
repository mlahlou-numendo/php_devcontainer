# PHP development in a devcontainer with preinstalled code quality tools

Set of files for starting VSCode in *devcontainer* mode and writing PHP codebase. Several static code analysis tools such as php-cs-fixer, phpcbf, SonarLint and others are preinstalled.

Let's imagine one of the following situations:

1. You are working with several people on the same PHP project and you notice that one or other person does not comply with your quality criteria when it comes to the layout of the code. You like to use four spaces for indentation, you want the brace that marks the start of a function to be on the line, you don't want to see any more useless spaces at the end of the line, ... and damned! you notice that some people don't care about this.

2. You are working alone on a project and don't want to lose time to configure your VSCode experience. You wish to start very quickly with a lot of tools already installed in VSCode so you can put your focus to the code, not the editor.

The ultimate solution: using a `devcontainer` in VSCode.

By using a **devcontainer**, you (and your team colleague) will use a preinstalled environment and everyone will have exactly the same. You'll save yourself a lot of time by not having to configure your system, and you'll be able to start coding straight away, supported by a range of quality analysis tools.

Please read the [PHP development in a devcontainer with preinstalled code quality tools](https://www.avonture.be/blog/vscode-devcontainer) blog post to learn how to use this repository.

## Don't have time to read a full story

In this case, please read [Install a PHP Docker environment in a matter of seconds](https://www.avonture.be/blog/php-devcontainer).

## Quick start

You already have an existing project

Start a terminal and open the folder where your codebase is located.

```shell
cd my_project
```

In my project folder, now, I'll run:
```shell
curl -LOJ --silent https://github.com/mlahlou-numendo/php_devcontainer/archive/refs/heads/main.tar.gz
tar -xzvf php_devcontainer-main.tar.gz --strip-components 1 && rm -f php_devcontainer-main.tar.gz
```

Start VSCode on your machine:

```shell
code .
```

If you don't have this popup, just press CTRL+SHIFT+P to open the Command Palette and search for Dev Containers: Rebuild and Reopen in Dev Container and click on it.

VSCode will now take a while to build the Docker image then start a Docker container before you can work. It can take a few minutes depending on the speed of your machine.
VSCode will automatically suggest opening a Dev Container. Click on the Reopen in Container button.

## References

- [PHP development in a devcontainer with preinstalled code quality tools](https://www.avonture.be/blog/vscode-devcontainer/)
- [Install a PHP Docker environment in a matter of seconds](https://www.avonture.be/blog/php-devcontainer/)
