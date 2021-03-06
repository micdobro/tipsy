# Tipsy - A CakePHP 3 + Vue.js betting game SPA 

Tipsy is a betting game for football worldcups and shows how CakePHP 3 and Vue.js can be used to create SPAs that consist of a Vue.js powered frontend and an API implementation in CakePHP 3.

## Installation

1. Clone the project locally or on a server.
2. Install dependencies
    ```bash
    composer install
    ```
3. Configure your environment ([Environment Documentation](https://github.com/frankfoerster/cakephp-environment))
4. Migrate the DB
    ```bash
    chmod +x bin/cake
    bin/cake migrations migrate
    ```

## Development

1. Install npm packages
    ```bash
    npm install
    ```

2. Run any of the provided Grunt tasks to create a new frontend build.

    - **webpack-dev**
        ```bash
        grunt webpack-dev
        ```
        Creates an unminified development build that supports Vue.js Dev tools.
    
    - **webpack-prod**
        ```bash
        grunt webpack-prod
        ```
        Creates a production ready minified and uglified build without Vue.js Dev tools support.
    
    - **watch-vue**
        ```bash
        grunt watch-vue
        ```
        Watches for changes to any files (.vue, .js, .scss, .css) in the frontend app and automatically triggers a new webpack-dev build.

## Notes

Depending on the debug configuration of your environment the app will either load the dev build (debug = true) or the prod build (debug = false).

## About

This app is an experiment to see how easy it is to couple Vue.js with a stateless CakePHP API.

## Screenshots

**Login Screen:**

![login](docs/screen-login.png)

**Overview:**

![overview](docs/screen-overview.png)

**Voting on Games:**

![games](docs/screen-games.png)
