@stylexjs/webpack-plugin currently has webpack as a dependency. If an app's webpack version, and stylex's webpack version don't match, the compilation fails.

Running `yarn start` results in

```
[webpack-cli] TypeError: The 'compilation' argument must be an instance of Compilation
    at NormalModule.getCompilationHooks (/stylex-webpack-bug/node_modules/@stylexjs/webpack-plugin/node_modules/webpack/lib/NormalModule.js:241:10)
```
