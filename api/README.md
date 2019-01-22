## 股票监控系统接口文档
```
接口BaseUrl: https://stock.vduan.top/api/
```

#### 实时获取股票平价格 (已完成)

##### 用途
* 实时的收益计算
* 价格监控

##### 请求路径

```
/price/:code
```
##### 请求方式

* GET
  
##### 试例

###### 请求
```
GET: https://stock.vduan.top/api/price/600516
```
###### 返回结果

| 参数 | 类型 | 描述 |
| ------ | ------ | ------ |
| code | string | 股票代码 |
| name | string | 股票名称 |
| todayOpening | string | 今日开盘价(元) |
| yesClosing | string | 昨日收盘价(元) |
| now | string | 现价(元) |
```
{
    "code": 0,
    "data": {
        "code": "600516",
        "name": "方大炭素",
        "todayOpening": "17.10",
        "yesClosing": "16.94",
        "now": "18.55"
    },
    "msg": "请求成功"
}
```


#### 实时获取资金流向 (已完成)
##### 用途

* 市场监控需要的资金流向监控

##### 请求路径

```
/flow/:code
```
##### 请求方式

* GET
  
##### 试例

###### 请求
```
GET: https://stock.vduan.top/api/flow/600516
```
###### 返回结果

| 参数 | 类型 | 描述 |
| ------ | ------ | ------ |
| code | string | 股票代码 |
| name | string | 股票名称 |
| date | string | 日期 |
| mainInflow | string | 主力流入(万元) |
| mainOutflow | string | 主力流出(万元) |
| mainFlow | string | 主力净流入(万元) |
| mainFund | string | 主力资金净流入/流出 |
| retailInflow | string | 散户流入(万元) |
| retailOutflow | string | 散户流出(万元) |
| retailFlow | string | 散户净流入(万元) |
| retailFund | string | 散户资金净流入/流出 |
| totalFlow | string | 总成交额(元) |

```
{
    "code": 0,
    "data": {
        "code": "600516",
        "name": "方大炭素",
        "date": "20190121",
        "mainInflow": "64161.54",
        "mainOutflow": "41556.78",
        "mainFlow": "22604.76",
        "mainFund": "18.44",
        "retailInflow": "58450.51",
        "retailOutflow": "50705.80",
        "retailFlow": "7744.71",
        "retailFund": "8.39",
        "totalFlow": "2251581265.00"
    },
    "msg": "请求成功"
}
```