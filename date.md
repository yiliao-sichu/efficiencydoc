# Date函数
## format
  根据传入时间,返回你想要的时间格式字符串
### dateTime格式
  |参数名|备注|
  |:-:|:----:|
  |yyyy|年份|
  |yy|年份缩写|
  |MM|月|
  |dd|日|
  |hh|小时|
  |mm|分钟|
  |ss|秒钟|
  |qq|季节|
  |SS|毫秒|
### 参数
  |参数名|是否必填|类型|备注|
  |:-:|:-:|:-:|:----------:|
  |dataTime|是|string,date|根据传入的dateTime解析时间,可以为时间戳|
  |format|是|String|你要匹配时间格式字符串|
  |bool|否|boolean|默认为false不补0,比如月份小于10,则为9,补0则为09|
### 演示
  ``` js
  // 不传bool参数
    console.log(efficiency.format(new Date(), 'yyyy年yy月dd日'));
  // 打印 2022年7月7日


  // 传bool参数
    console.log(efficiency.format(new Date(), 'yyyy年yy月dd日', true));
  // 打印 2022年07月07日
  ```