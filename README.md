<p align="center">
  <img src ="https://github.com/msincenselee/vnpy/blob/master/huafu_on_premise.jpg"/>
</p>


# “当你想放弃时，想想你为什么开始。埃隆·马斯克”

###Fork版本主要改进如下
1. 事件引擎，增加运行效率调试功能
2. 增加rabbitMQ通信组件
3. 增加tdx 免费数据源
4. 增加App: tick_recorder, 直接异步写入csv文件
5. 增加App: index_tick_publisher, 订阅通达信指数行情=》rabbit_mq 推送
6. 增强ctp_gateway，包括:
    
    - 提供指数行情订阅
    - 使用RabbitMQ指数源，或tdx单一数据源
    - 提供自定义合约功能，实时提供其合成后的tick行情
7. 增加App: cta_strategy_pro，包括：
    
    - 提供cta_line_bar k线组件，支持国内文华/交易师/TB等分钟/小时的计算模式，支持任意秒/分钟/小时/天/周等周期，支持k线数据实时生成。
    - 提供cta_position 组件，支持多/空/净仓位记录，支持套利
    - 提供cta_policy 组件，持久化复杂的策略执行逻辑
    - 提供cta_period 组件，支持策略中‘周期’的逻辑
    - 提供cta_grid_trade组件，支持网格交易、复杂的策略持仓逻辑、持久化
    - 提供策略实例的单独日志记录文件
    - 去除统一的策略数据持久化功能，改为策略内部自行实现。
    - 去除加载k线/tick初始化服务，改为策略内部自行实现。
    - 提供单独重启某一策略实例功能，可在线更新策略源码后，重启某一策略实例，不影响其他运行实例。
大佳
QQ/Wechat：28888502


--------------------------------------------------------------------------------------------
#  原版 vn.py - 基于python的开源交易平台开发框架
https://github.com/vnpy/vnpy
--------------------------------------------------------------------------------------------
### License
MIT
