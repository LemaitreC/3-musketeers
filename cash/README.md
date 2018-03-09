<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Cash](#cash)
  - [Introduction](#introduction)
  - [Instalation](#instalation)
  - [How to use it](#how-to-use-it)
    - [Get amout in defaults currencies](#get-amout-in-defaults-currencies)
    - [Get other currencies](#get-other-currencies)
    - [Change default currencies](#change-default-currencies)
    - [If you need help](#if-you-need-help)
  - [Example of commands and returns](#example-of-commands-and-returns)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Cash

## Introduction

This nodeJS app is very useful to convert a currency in others. For example if you want to know the equivalent of 1 euros in US dollars or GBP.

## Instalation

To install the project you first need to clone it. After you have to run this command :
```
npm install
```

It will install all dependencies and modules the app needs to work properly.

## How to use it

Once in the directory of the app there is two ways of using the app :

### Get amout in defaults currencies

To get the amount in the default currencies (**USD**, **EUR**, **GBP** for example) you need to use this command :
```
node bin/index.js <amount> <currency>
```
You at least need to put in argument an **amount** and one **currency** corresponding to this amout.</br>
If the input currency is already one of (**USD**, **EUR**, **GBP** ) it just display the conversion in the two other currency.

### Get other currencies
To get the amount in other currencies you need to use the command :
```
node bin/index.js <amount> <currency> <otherCurrency>
```
You at least need to put in argument an **amount** and one **currency** corresponding to this amout.</br>
Add the name of all currencies you want to get the amount in.

### Change default currencies

To change the defaults currencies use this command:

```
$ node bin/index.js --save usd eur pln aud
```

### If you need help

If you need help use this command:

```
$ node bin/index.js --help
```

## Example of commands and returns
```
$ node bin/index.js 1 aud

√ 0.78 (USD) US Dollar
√ 0.63 (EUR) Euro
√ 0.56 (GBP) Pound Sterling

```

```
$ node bin/index.js 1 usd eur pln aud

√ 0.81 (EUR) Euro
√ 3.42 (PLN) Polish Zloty
√ 1.28 (AUD) Australian Dollar

```
