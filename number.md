# Number函数
## randomNum
  获取随机范围内数字,可设置初始大小数字
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |scope|是|number|从0-scope随机获取数字|
  |start|否|number|默认为0, 控制最小数字范围，不能大于scope|
  ### 演示
  ``` js
    // 不传scope
    console.log(efficiency.randomNum(1000))
    // 打印441 可能出现的随机数为0 - 1000


    // scope 和 start 都传
    console.log(efficiency.randomNum(1000, 900));
    // 打印 910 可能出现的随机数为900 - 1000

  ```

## decimalPoint
  去除数字的小数点
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |floot|是|number|你要去除小数点的数字|
  |figure|否|number|默认为0, 去除所有小数点,如果为正数,则保留几位小数点,如为负数的话则去除最后几位小数点|
  ### 演示
  ``` js
    // 不传figure
    console.log(efficiency.decimalPoint(1000.11142))
    // 打印1000


    // figure为正数
    console.log(efficiency.decimalPoint(1000.11142, 2));
    // 打印1000.11

    // figure为负数
    console.log(efficiency.decimalPoint(1000.11142, -2));
    // 打印1000.111
  ```

  