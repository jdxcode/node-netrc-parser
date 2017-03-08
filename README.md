# netrc-parser

[![CircleCI](https://circleci.com/gh/dickeyxxx/node-netrc-parser.svg?style=svg)](https://circleci.com/gh/dickeyxxx/node-netrc-parser)
[![codecov](https://codecov.io/gh/dickeyxxx/node-netrc-parser/branch/master/graph/badge.svg)](https://codecov.io/gh/dickeyxxx/node-netrc-parser)

# API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## Netrc

[src/netrc.js:183-274](https://github.com/dickeyxxx/node-netrc-parser/blob/4ed44c62cd3939e1e5cd1ed3731f5ae46b2e40e7/src/netrc.js#L183-L274 "Source code on GitHub")

parses a netrc file

### constructor

[src/netrc.js:191-200](https://github.com/dickeyxxx/node-netrc-parser/blob/4ed44c62cd3939e1e5cd1ed3731f5ae46b2e40e7/src/netrc.js#L191-L200 "Source code on GitHub")

generates or parses a netrc file

**Parameters**

-   `file` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 

**Examples**

```javascript
const Netrc = require('netrc-parser')
const netrc = new Netrc()
netrc.machines['api.heroku.com'].password // get auth token from ~/.netrc
```

### save

[src/netrc.js:215-239](https://github.com/dickeyxxx/node-netrc-parser/blob/4ed44c62cd3939e1e5cd1ed3731f5ae46b2e40e7/src/netrc.js#L215-L239 "Source code on GitHub")

save the current home netrc with any changes

**Examples**

```javascript
const Netrc = require('netrc-parser')
const netrc = new Netrc()
netrc.machines['api.heroku.com'].password = 'newpassword'
netrc.save()
```
