# Array函数
## clearNull
  清空数组的空值
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |array|是|array|你要清空空值的数组|
  |bool|否|boolean|默认为false,是否需要清空0，默认只清空null和undefined|
  ### 演示
  ``` js
    // 不传bool
    console.log(efficiency.clearNull([123,dsd,0,null,'asdds']));
    // 打印 [123,0,dsd,null,'asdds']


    // 传bool为true
    console.log(efficiency.clearNull([123,dsd,0,null,'asdds'], true));
    // 打印 [123,dsd,null,'asdds']


    // 传bool为flase
    console.log(efficiency.clearNull([123,dsd,0,null,'asdds'], false));
    // 打印 [123,0,dsd,null,'asdds']
  ```


## sortArray
  对数组进行排序, 也能对json数组进行排序
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |array|是|array|你要进行排序的数组|
  |order|否|boolean|默认为true,true为正序,false为倒叙|
  |params|否|string|json数组排序需要传，该值为根据哪个参数进行排序|
  ### 演示
  ``` js
    // 不传order和params
    console.log(efficiency.sortArray([12, 12, 323, 15]));
    // 打印 [12, 12, 15, 323]


    // 不传params
    console.log(efficiency.sortArray([12, 12, 323, 15], false));
    // 打印 [323, 15, 12, 12]


    // json数组进行排序
    console.log(efficiency.sortArray([{a: 14},{a: 17},{a: 16}], false, 'a'));
    // 打印 [{a: 17},{a: 16},{a: 14}]
  ```


  ## findArray
  用于json数组寻找某一个对象，并进行返回该对象
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |array|是|array|你要进行寻找的数组|
  |key|是|String|你要匹配对象的字段名|
  |val|是|string,number,boolean|你要根据key变量名匹配的值|
  ### 演示
  ``` js
    // json数组寻找对象里a为14的
    console.log(efficiency.findArray([{a: 14},{a: 17},{a: 16}],'a',14));
    // 打印 {a: 14}
  ```


  ## flat2w
  把二维数组解析为一维数组
  ### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |array|是|array|你要进行解析的二维数组|
  ### 演示
  ``` js
    // json数组寻找对象里a为14的
    console.log(efficiency.flat2w([[1,2,3],4,5,[6,7]]));
    // 打印 [1,2,3,4,5,6,7]
  ```