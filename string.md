# String函数
## randomStr
  获取随机字符串
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |dight|是|number|获取随机字符串的长度|
  |str|否|string|获取字符串内容的集合,默认从英文数字里面获取随机字符|
  ### 演示
  ``` js
    // 不传str,会随机获取dight个英文和数字
    console.log(efficiency.randomStr(10))
    // 打印adfdwe15Fs


    // dight 和 str 都传
    console.log(efficiency.randomStr(5, '哇哈123'));
    // 打印 2哇哈哈1

  ```