## 03
```
yarn run example 03_simple-reducer.js
yarn run v1.6.0
$ babel-node 03_simple-reducer.js
Reducer was called with args [ undefined, { type: '@@redux/INIT' } ]
✨  Done in 2.09s.
```
* [ undefined, { type: '@@redux/INIT' } ]
* 在被调用时，一个 reducer 会得到这些参数：(state, action)
* state undefined
* action { type: '@@redux/INIT' }