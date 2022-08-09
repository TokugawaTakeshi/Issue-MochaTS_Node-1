# Experiment flow

## 1 Install dependencies

```shell
npm i
```

## 2 Run tests

```shell
mocha
```

You should the message like below:

```
TypeError [ERR_UNKNOWN_FILE_EXTENSION]: Unknown file extension ".ts" for D:\IntelliJ IDEA\Issues\Issue-MochaTSNode\node_modules\tsconfig-paths\src\__tests__\config-loader.test.ts
```

If tests completed normally, it means that current issue is environment-dependent.
If you get the error please proceed to next step.


## 3 Uninstall the "@yamato-daiwa/style_guides", the ESLint preset

```shell
npm uninstall @yamato-daiwa/style_guides
```


## 4 Rerun tests

```
mocha
```

This time test should complete properly.

Optionally, you can revert changes, reinstall the dependencies and run `mocha` again - error will return. 
