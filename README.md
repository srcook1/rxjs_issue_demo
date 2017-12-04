"# rxjs_issue_demo" 

run 'npm start' to see issue

result I am seeing:
> node -r babel-register index.js

c:\path\rxjs_issue\index.js:10
var observable = new _Rx2.default.Subject();
                                  ^

TypeError: Cannot read property 'Subject' of undefined
    at Object.<anonymous> (c:/path/rxjs_issue/index.js:2:25)
    at Module._compile (module.js:635:30)
    at loader (c:\path\rxjs_issue\node_modules\babel-register\lib\node.js:144:5)
    at Object.require.extensions.(anonymous function) [as .js] (c:\path\rxjs_issue\node_modules\babel-register\lib\node.js:154:7)
    at Module.load (module.js:554:32)
    at tryModuleLoad (module.js:497:12)
    at Function.Module._load (module.js:489:3)
    at Function.Module.runMain (module.js:676:10)
    at startup (bootstrap_node.js:187:16)
    at bootstrap_node.js:608:3


change to rxjs v 5.5.2 and the code works