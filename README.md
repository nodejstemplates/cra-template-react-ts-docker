# cra-template-typescript

This is the TypeScript template for [Create React App](https://github.com/facebook/create-react-app) to develop in  a docker environment.

To use this template, add `--template react-ts-docker` when creating a new app.

For example:

```sh
npx create-react-app my-app --template react-ts-docker

# or

yarn create react-app my-app --template react-ts-docker

# or

docker run -it -v .\:/appdir -w /appdir node:20.11.1-bullseye npx create-react-app my-reactapp --template react-ts-docker

```

For more information, please refer to:

- [Getting Started](https://create-react-app.dev/docs/getting-started) – How to create a new app.
- [User Guide](https://create-react-app.dev) – How to develop apps bootstrapped with Create React App.
