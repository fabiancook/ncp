# ncp - Asynchronous recursive file & directory copying

Think `cp -r`, but pure node, and asynchronous.  `ncp` can be used both as a CLI tool and programmatically.

## Command Line usage

Usage is simple: `ncp [source] [dest]`

If there are no errors, there will be no output.  Note that `ncp` will fail if its destination path exists.

## Programmatic usage

Programmatic usage of `ncp` is just as simple.  

```javascript
var ncp = require('ncp').ncp;

ncp(source, destination, function (err) {
 if (err) {
   return console.error(err);
 }
 console.log('done!');
});
```

Please open an issue if any bugs arise.  As always, I accept (working) pull requests, and refunds are available at `/dev/null`.