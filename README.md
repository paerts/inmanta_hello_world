# Hello world


This is a simple example project to test if your orchestrator is installed correctly.

For instruction on installing the inmanta orchestrator go [here](https://docs.inmanta.com/community/latest/install.html).


# Using this repo

This model installs a file on the orchestrator machine itself in `/tmp/inmanta_hello_world` as the `inmanta` user.

To install this project from the CLI, on the orchestrator
```bash
inmanta-cli project create --name test
inmanta-cli environment create --name hello_world --project test --repo-url git@github.com:inmanta/hello_world.git

```
Then go to the web console and click 'Update and Recompile'





