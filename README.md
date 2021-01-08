# Gatsby Playground

A gatsby site playground.

## Install

1. Copy the yellowcake repository:

    ```
    git clone --bare https://github.com/thriveweb/yellowcake
    cd yellowcake.git/
    git push --mirror https://github.com/ktmeaton/gatsby-playground
    ```

1. Open repository with gitpod.

1. Install node modules:

    ```
    npm install
    npm install -g gatsby-cli
    npm install gh-pages --save-dev
    ```

1. Test run the demo site:

    ```
    npm run start
    ```

## Deploy

### Github Pages

1. Add the deploy script to ```package.json```:

```
{
"scripts": {
    ...
    "deploy": "gatsby build --prefix-paths && gh-pages -d public",
    }
}
```

### Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/)

1. Build command: ```gatsby build --prefix-paths```
1. Publish directory: ```public```
1. Change site name to: https://ktmeaton-gatsby-playground.netlify.app
