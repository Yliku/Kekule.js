Kekule.js JS file compressor
===================================

This application is a simple JavaScript compressor for Kekule.js source files.
It is helpful to build custom JS min files. 
You may run the application in the following command line:

```
node run.js -m=module1,module2,... -d=destinationPath
```  

where the -d arg appoint the output path and the -m arg limits the modules needed to be outputted. 
If this arg is not set, all modules of Kekule.js will be compressed and outputted.

For example, the following command line will compress files related to ```io``` and ```widget``` module
and output them in ```../dist`` directory:

```
node run.js -m=io,widget -d=../dist
```

To generate all min js files in default path, just call:

```
node run.js
```

Note this application only creates min JS files. CSS files and sprite images are not handled by this tool.
