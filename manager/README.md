## 管理端

### 用户管理

#### 用户列表

##### 显示信息

* 注册渠道
* 注册方式
* 注册账号
* 注册时间

##### 新用户列表

每10s刷新一次

#### level管理

##### 说明

* 普通用户最高可达50分，从注册开始计算每天+0.5分
* 对用户进行分级，级别高的优先获得消息的提醒(监控消息和荐股消息)

##### 管理level
通过此管理端可直接修改用户的level

###### 每次修改需要如下信息，并保存更改日志

* 管理员ID
* 用户ID
* level
* 备注信息







### 监控提醒模板

由于我们适用邮箱进行提醒所以采用富文本的模板编辑

##### 添加和修改模板

* 监控类型
  * 跌涨幅监控
  * 价格监控
  * 资金流向监控
  * 消息面监控
* 平台名(名字还没取，可以取个高逼格的名字)
* 富文本内容

##### 提供预览功能

可直接预览

### 日志模块

#### 日志搜索

可通过如下参数进行日志的搜索

* 日志分类
* 时间间隔
* 用户邮箱

#### 日志分类

##### 监控消息发送日志

* 用户邮箱
* 监控类型
* 发送是否成功
* 发送时间

##### 持仓修改日志

* 用户邮箱
* 用户修改内容
* 修改时间

##### level管理日志

* 管理员ID
* 修改对象
* 修改内容
* 修改备注
* 修改时间

