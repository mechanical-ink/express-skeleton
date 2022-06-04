# express-skeleton

👋 Welcome to express-skeleton, part of the [Project Calavera](https://github.com/project-calavera). Express-skeleton is a starter template(skeleton) for [Expressjs](https://expressjs.com/) based apps and websites.

## What is this repository?

This repository allows you to quickly scaffold a basic Expressjs project using the [Pug templating](https://pugjs.org/api/getting-started.html) language. It provides the following:

Once [cloned](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository), either directly, or a repository that uses this one as a [template repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template), it allows you to simply run `npm i` or `yarn` to install the dependencies you will need.

```json
"devDependencies": {
  "nodemon": "^2.0.16",
  "parcel-bundler": "^1.12.5"
},
"dependencies": {
  "express": "^4.18.1",
  "pug": "^3.0.2"
}
```

The `pckage.json` that comes with the project also has the following NPM script targets:

```json
"build": "parcel views/index.pug",
"start": "nodemon app.js",
```

> NOTE: Remember to update the `package.json` with information about your project.

It also contains a basic `.gitignore` file as well as a default configuration(`.prettierrc`) for [Prettier](https://prettier.io/).
It contains a [single `route`](https://github.com/project-calavera/express-skeleton/blob/main/routes/router.js) that will serve your [index](https://github.com/project-calavera/express-skeleton/tree/main/views) file.

The project also contains an empty [`main.js`](https://github.com/project-calavera/express-skeleton/blob/main/static/js/main.js) file, which is already being included for you inside the [footer partial](https://github.com/project-calavera/express-skeleton/blob/main/views/includes/footer.pug). There is also a [head.pug](https://github.com/project-calavera/express-skeleton/blob/main/views/includes/head.pug) file that contains basic elements that goes into the `head` of your HTML document. This then also loads the [CSS file](https://github.com/project-calavera/express-skeleton/blob/main/static/style/main.css) from the static folder.

The project also includes a [`.github` folder](https://github.com/project-calavera/express-skeleton/tree/main/.github) with the following:

- dependabot.yml - Setup to automatically keep the [project dependencies up to date](https://github.com/dependabot).
- workflows/auto-merge.yml - This will automatically merge Dependabot pull request that are not a major version bump and, should all your CI tests and workflows pass. To use this, you will also need to configure a repository [environmental secret](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository) with a [personal access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) that has repo scope.

## Why is it useful?

If you often start new projects that uses Expressjs, Pug and the [Parcel bundler](https://parceljs.org/) this will definitely save you at least an hour of your day. That is nothing to sneeze at right? 😁

## How do I get started?

- Once you have your repository ready, clone it locally
- Change into the root directory for the cloned repository
- Run `yarn` or `npm i`
- Run `yarn start` or `npm start`
- Open your browser to `http://localhost:3000`

https://user-images.githubusercontent.com/10350960/172025206-225b2123-20f5-4484-b5c0-c877d6afeb0f.mp4

## Where can I get more help, if I need it?

If anything is not working as expected, please join our [Discord server](https://discord.gg/6MrjtEmDgr) or [open an issue](https://github.com/project-calavera/express-skeleton/issues/new) here on GitHub.

## Licensing and code of conduct

The is project is licensed under an MIT license. If you wish to participate with this project, please read our code of conduct to ensure we foster a healthy and welcoming community.
