# libphonenumber [![Build Status](https://travis-ci.org/mattbornski/libphonenumber.png)](http://travis-ci.org/mattbornski/libphonenumber) [![Build status](https://ci-beta.appveyor.com/api/projects/status/rmhkeri71ystuk7w)](https://ci-beta.appveyor.com/project/mattbornski/libphonenumber)

NodeJS port of Google's libphonenumber (thanks to SocialCam), packaged for npm

## Installation

### Installing npm (node package manager)
```
curl http://npmjs.org/install.sh | sh
```

### Installing libphonenumber
```
npm install libphonenumber
```

## Example Usage

```javascript
var libphonenumber = require('libphonenumber')
var PhoneUtil = libphonenumber.phoneUtil;

var number = PhoneUtil.parseAndKeepRawInput("05 92 29 20 29", 'fr');
var formated = PhoneUtil.format(number, 0); //TODO Export original PhoneNumberFormat for format values
console.log(formated); //Prints: +33592292029

```
