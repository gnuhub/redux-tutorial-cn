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
## 04 如何从 Redux 实例中读取 state
* 一个 reducer 只是一个函数，它能收到程序当前的 state 与 action
* reducer 类型 函数
* statue {}
* action 类型 对象 hash 关联数组 词典 
```
var reducer_1 = function (state, action) {
    console.log('reducer_1 was called with state', state, 'and action', action)
    if (typeof state === 'undefined') {
        return {}
    }

    return state;
}
```
* 一个成为reducer类型的函数，就是普通函数，输入是state 以及 action返回 state
* 目前为止都是初始的state，没有处理action也没有产生新的statue