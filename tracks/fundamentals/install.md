# Install Substrate Templates

Once your [machine is configured](../install), you can use `git` to clone the Substrate Developer Hub Node
Templates, which serve as a good starting points for building on Substrate.

## Install the Node Template

1. Clone the Node Template (version `v3.0.0`).

    ```bash
    git clone -b v3.0.0 --depth 1 https://github.com/substrate-developer-hub/substrate-node-template
    ```
2. Compile the Node Template

    ```bash
    cd substrate-node-template
    # NOTE: you should always use the `--release` flag
    cargo build --release
    # ^^ this will take a while!
    ```

> **You should start building the node template _before_ moving on!**
>
> The time required for the compilation step depends on the hardware you're using.
>
> **Run into issues? Try the [troubleshooting tips](../../../knowledgebase/getting-started/index#troubleshooting-substrate-builds).**

## Install the Front-End Template

This tutorial uses a [ReactJS](https://reactjs.org/) front-end template to allow you to interact
with the Substrate-based blockchain node that you should have started compiling in the previous
step. You can use this same front-end template to create UIs for your own projects in the future.

To use the front-end template, you need [Yarn](https://yarnpkg.com), which itself requires
[Node.js](https://nodejs.org/). If you don't have these tools, you _must_ install them from these
instructions:

- [Install Node.js](https://nodejs.org/en/download/)
- [Install Yarn](https://yarnpkg.com/lang/en/docs/install/)

Now you can proceed to set up the front-end template with these commands.

```bash
# Clone the frontend template from github
git clone -b v3.0.0 --depth 1 https://github.com/substrate-developer-hub/substrate-front-end-template

# Install the dependencies
cd substrate-front-end-template
yarn install
```
