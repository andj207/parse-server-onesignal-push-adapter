# parse-server-onesignal-push-adapter

[![Build Status](https://travis-ci.org/parse-server-modules/parse-server-onesignal-push-adapter.svg?branch=master)](https://travis-ci.org/parse-server-modules/parse-server-onesignal-push-adapter)
[![codecov.io](https://codecov.io/github/parse-server-modules/parse-server-onesignal-push-adapter/coverage.svg?branch=master)](https://codecov.io/github/parse-server-modules/parse-server-onesignal-push-adapter?branch=master)



OneSignal push adapter for parse-server.
This fork support multiple OneSignal apps in one application.


## Installation

```
npm install --save git+https://git@github.com/andj207/parse-server-onesignal-push-adapter.git
```

## Usage

```
var OneSignalPushAdapter = require('parse-server-onesignal-push-adapter');
let oneSignalPushAdapter = new OneSignalPushAdapter({
    'app identifier matches with the value in Installation table to classify': {
        oneSignalAppId: "",
        oneSignalApiKey: ""
    },
    ....
});

var api = new ParseServer({
  push: {
    adapter: oneSignalPushAdapter
  },
  ...otherOptions
});
```
