### 兼容性

在chrome58.0.xx的版本下报错： .then(...).catch(...).finally is not a function

[资料](https://blog.csdn.net/simon9124/article/details/80940338)

    yarn add promise.prototype.finally    // 安装 promise.prototype.finally 包
    require('promise.prototype.finally').shim();   // 最后记得在 main.js 里引入该依赖包
