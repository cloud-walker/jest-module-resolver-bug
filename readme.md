# Jest + babel-plugin-module-resolver aliases bug 🐛

If you use `babel-plugin-module-resolver` to handle deps aliases, jest watch won't
see aliases changes.

## To reproduce

* `yarn`
* `npm t`
* modify the coefficient in the `source/constants.js` file, both `add` and `subtract` functions use it, and only subtract test error will be notified on jest --watch 😫
