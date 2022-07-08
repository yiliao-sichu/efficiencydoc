# 工具类函数
## copy
  对数组和对象进行深拷贝
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |obj|是|object,array|你要进行深拷贝的对象|
  ### 演示
  ``` js
    console.log(efficiency.copy({i: '111'}))
    // 打印{i: '111'}
  ```


## throttle
  防止重复触发,立即触发函数,n秒内只有一次有效触发
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |methods|是|function|你要防止重复触发的函数|
  |time|否|number|默认为2000,单位为毫秒,time内只有一次有效点击|
  ### 演示
  ``` js
    efficiency.throttle(function() {
      console.log('11111');  
    }, 3000)
    // 打印 11111
  ```


## antiSjale
  防止重复触发, 触发n秒后执行函数，如重复点击则重置n秒后执行
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |methods|是|function|你要防止重复触发的函数|
  |time|否|number|默认为2000,单位为毫秒,time内只有一次有效点击|
  ### 演示
  ``` js
    efficiency.antiSjale(function() {
      console.log('11111');  
    }, 3000)
    // 3秒后打印 11111
  ```


  