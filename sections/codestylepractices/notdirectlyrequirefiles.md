**TL;DR:** When developing a module/library in a folder, place an index.js file that exposes the module's
internals so every consumer will pass through it. This serves as an 'interface' to your module and eases
future changes without breaking the contract

**Otherwise:** Changing the internal structure of files or the signature may break the interface with
clients

### Code example

```javascript
// Do
module.exports.SMSProvider = require('./SMSProvider');
module.exports.SMSNumberResolver = require('./SMSNumberResolver');

// Avoid
module.exports.SMSProvider = require('./SMSProvider/SMSProvider.js');
module.exports.SMSNumberResolver = require('./SMSNumberResolver/SMSNumberResolver.js');
```
