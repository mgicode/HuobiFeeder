# [Huobi Feeder](https://github.com/mmmaaaggg/HuobiFeeder)
连接火币交易所

通过 feed.md_feeder 接受事实行情及补充历史数据

通过 backend.handler 处理实时行情，保持到数据库，进行redis广播

该项目作为 ABAT 框架的 Feeder 组件可独立部署



## 安装

#### 系统环境要求：

> Python 3.6 
> MySQL 5.7 
> Redis 3.0.6 

#### 安装必要python包

Windows环境

> pip install -r requirements.txt

Linux环境

> pip3 install -r requirements.txt

#### 配置文件

config.py

#### 启动方法

直接运行 huobifeeder/run.py

启动过程中会自动建立相应数据库表结构



## 存储及服务

存储mysql数据库

> md_min1_tick_bc  tick数据
>
> my_min1_bc   一分钟数据
>
> md_min60_bc  一小时数据
>
> md_daily_bc  日数据

channel格式：

```
md.{market}.{period}.{symbol}
#    例如：
#    md.huobi.Min1.ethusdt
#    md.huobi.Tick.eosusdt
```



## 欢迎赞助

#### 微信

![微信支付](https://github.com/mmmaaaggg/ABAT_trader_4_blockchain/blob/master/mass/webchat_code200.png?raw=true)

#### 支付宝

![微信支付](https://github.com/mmmaaaggg/ABAT_trader_4_blockchain/blob/master/mass/alipay_code200.png?raw=true)

#### 微信打赏（￥10）

![微信打赏](https://github.com/mmmaaaggg/ABAT_trader_4_blockchain/blob/master/mass/dashang_code200.png?raw=true)

