# crawler
## 跑起来
1. npm install
2. npm run exe
3. 程序能够运行

## 要求
- 实现一个简易爬虫
- 从东方财富API爬取基金净值信息
- npm run exe 123456 将会获取基金ID为123456的基本信息与基金净值
- 基本信息包括： 基金名称，基金类型
- 基金净值为2D数组，[时间, 净值][]，时间保存为unix时间戳
- 最终数据保存为json文件存在硬盘
- 爬虫要考虑效率，使用并发，不能挨个发请求

## 爬虫端点
- 基金基本信息: http://fund.eastmoney.com/js/fundcode_search.js
- 基金净值: http://fund.eastmoney.com/f10/F10DataApi.aspx?type=lsjz&code=160220&page=1
- 基金净值中，code是基金ID，page是页数。
