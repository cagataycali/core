[![Build Status](https://travis-ci.org/oslab-fr/lesspass-npm.svg?branch=master)](https://travis-ci.org/oslab-fr/lesspass-npm)

# LessPass Core

LessPass npm module use to generate unique password 

## Install

    npm install lesspass

## Usage

    var lesspass = require('lesspass');
    var entry = {
        site: 'lesspass',
        password: {
            length: 14,
            settings: ['lowercase', 'uppercase', 'numbers', 'symbols'],
            counter: 1
        }
    };
    var masterPassword = '90cff82b8847525370a8f29a59ecf45db62c719a535788ad0df58d32304e925d';
    var password = lesspass.createPassword(masterPassword, entry);
    console.log(password); // ubUB4[yqAD3?od

