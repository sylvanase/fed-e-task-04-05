# fed-e-task-04-05

1. 通过该项目，请简要说明 typescript 比 javascript 的优势在哪？
对于函数中的入参出参等可以定义类型，已经进行类型判断及校验。对于不符合定义的参数等可以提前暴露错误，降低代码错误率。
对于大型多人维护项目，使用ts可以提高代码可维护性、易读性。

2. 请简述一下支付流程
首先用户提交订单，订单生成成功后返回支付地址，客户端跳转该支付地址，若用户支付完成，支付宝会重定向到设定的地址，提示用户该笔订单的支付状态为成功/失败。
同时支付宝会通知服务器该笔订单的支付状态，服务器对订单进行状态变更。


3.react-redux 的主要作用是什么，常用的 api 有哪些，什么作用？
主要作用是在react工程中进行状态管理。
- createStore: 创建状态容器
- dispatch：触发action
- subscribe：订阅状态
- getState：获取状态
- useDispatch：在react hooks中使用等同于dispatch
- useSelector：在react hooks中使用，获取状态

4. redux 中的异步如何处理
使用 redux-thunk 或者 redux-saga 中间件处理异步
