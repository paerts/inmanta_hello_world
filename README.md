# Hello world

This is a simple example project to test if your orchestrator is installed correctly.

For instruction on installing the inmanta orchestrator go [here](https://docs.inmanta.com/community/latest/install.html).

## Using this repo

This model installs a file on the orchestrator machine itself in `/tmp/inmanta_hello_world` as the `inmanta` user.

The project can be installed using two ways; CLI and Web Console.

* To install from the `CLI`, on the orchestrator:

    ```bash
    inmanta-cli project create --name test
    inmanta-cli environment create --name hello_world --project test --repo-url git@github.com:inmanta/hello_world.git
    ```

    Then go to the `Web Console` and click 'Update and Recompile'

* To install from the `Web Console`, on the orchestrator:

    Head to the Web Console and click on `Create new environment`:

    ![mainpage](images/1.png)

    Fill in the information as follows and click `submit`:

    ```txt
      Project Name: test
      Name: hello_world
      Repository: https://github.com/inmanta/hello_world.git
      Branch: master
    ```

    ![createEnv](images/22.png)

    Go to settings:

    ![settings](images/3.png)

    Click on `Configuration` and go to the bottom of the page:

    ![configuration](images/4.png)

    Enable `server_compile` and click on `save`:

    ![serverCompile](images/5.png)

    Click on the `Recompile` arrow then select `Update project and recompile`:

    ![updateAndRecompile](images/6.png)

    Click on details

    ![compileDetails](images/7.png)

    The status should be successful:

    ![compileStatus](images/8.png)

    `inmanta_hello_world` file is created on Inmanta server:

    ![inmantaFile](images/9.png)