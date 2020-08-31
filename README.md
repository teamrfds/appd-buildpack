

### Building the Buildpack

To build this buildpack, run the following commands from the buildpack's directory:

1. Source the .envrc file in the buildpack directory.

   ```bash
   source .envrc
   ```
   To simplify the process in the future, install [direnv](https://direnv.net/) which will automatically source .envrc when you change directories.

1. Install tools

    ```bash
    ./scripts/install_tools.sh
    ```

1. Build the buildpack

    ```bash
    ./scripts/build.sh
    ```

1. Execute the below script, which builds, uploads the buildpack to cf 
    ```bash
    ./scripts/test.sh
    ```

