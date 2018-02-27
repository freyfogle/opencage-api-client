# opencage-api-client

This node package is an [OpenCage Data API](https://geocoder.opencagedata.com/api) client.

[![CircleCI](https://circleci.com/gh/tsamaya/opencage-api-client/tree/master.svg?style=svg)](https://circleci.com/gh/tsamaya/opencage-api-client/tree/master)
[![codecov](https://codecov.io/gh/tsamaya/opencage-api-client/branch/master/graph/badge.svg)](https://codecov.io/gh/tsamaya/opencage-api-client)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

:warning: working progress

## Getting started

Signup for a [free API Key](https://geocoder.opencagedata.com/users/sign_up).

The library uses [dotenv](https://www.npmjs.com/package/dotenv) on node runtime to configure OpenCage Data API key.

First install the library with `npm` or `yarn`:

```
$ npm i opencage-api-client
```
or
```
$ yarn add opencage-api-client
````

Create a `.env` file with:
```
OCD_API_KEY=YOUR-OPENCAGE_DATA_API_KEY
```

Here is an example:

```javascript
const opencage = require('opencage-api-client');

opencage.geocode({q: 'lyon'}).then(data => {
  console.log(JSON.stringify(data));
}).catch(error => {
  console.log('error', error.message);
});
```

## API

> TODO

## Build and test

1. Fork or clone this repository
1. `$ cd` into the `repository` folder
1. `$ npm install` to install all the required dependencies from [npm](https://www.npmjs.com/)
1. lint and test using `$ npm test`
1. coverage `$ npm run coverage`
1. Build : `$ npm run build`

## Contributing

Anyone and everyone is welcome to contribute.

## Issues

Find a bug or want to request a new feature? Please let me know by submitting an issue.

## Licensing

Licensed under the MIT License

A copy of the license is available in the repository's [LICENSE](LICENSE.md) file.
