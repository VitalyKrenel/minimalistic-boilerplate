### Minimalistic boilerplate for JS projects

**Small overview of devDependencies:**

- [`Mocha`](https://www.npmjs.com/package/mocha) and 
[`Chai`](https://www.npmjs.com/package/chai) are used for testing.

- [`Husky`](https://www.npmjs.com/package/husky) with support of [`npm-run-all`](https://www.npmjs.com/package/npm-run-all) is used for pre-commit git hook. `npm-run-all` helps simultaneously run npm scripts. Additional hooks may be added in package.json within husky.hooks property. 

- [`Eslint`](https://www.npmjs.com/package/eslint) is used for linting Javascript. Eslint config is [`eslint-config-airbnb-base`](https://www.npmjs.com/package/eslint-config-airbnb-base). Linting rules are based on [Airbnb style guide](https://github.com/airbnb/javascript) with minor personal changings. 

- [`Browser-sync`](https://browsersync.io/docs/command-line) takes
the server position. It's configured with -w flag to provide
autoreloading on resources update. It's suitable for the development
of interfaces, but not that useful for scalable JS development (no 
treeshaking, no code spliting, etc).
