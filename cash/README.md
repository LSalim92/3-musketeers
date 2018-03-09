<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Cash](#cash)
- [Installation](#installation)
- [Use](#use)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Cash
This application allows to apply conversion of different currencies.

## Installation

First of all, you have to install the following package in the directory /cash

```js
npm install
```

## Use

You have different possibility to use the application. The list of the different currencies is available at http://akep.us/currencies

1. The following command will the convert the given amount of the given currency by default to Euro and Pound Sterling
```js
node bin/index.js <amount_to_convert> <currency>
```
Exemple:
```js
node bin/index.js 1 usd
```

2. The following command will the convert the given amount of the given currency by default to the currencies listed just after
```js
node bin/index.js <amount_to_convert> <currency_from> <currency_to>
```
Exemple:
```js
node bin/index.js 1 usd eur pln aud
```

3. You can also use different commands
```js
node bin/index.js <command>
```
The different command available are:
 * --save,  -s       Save currencies as default currencies
 * --help,  -h       Display help message
 * --version,  -v     Display version number

    Exemple:
    ```js
    node bin/index.js --save usd eur pln aud
    ```
    ```js
    node bin/index.js --help
    ```
