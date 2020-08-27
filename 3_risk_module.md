


|验证器|范围|功能|实现|
|--|:--|--|--|
|Adaptor|All|检查柜台是否可用|已实现|
|Balance|NewOrder(Buy)|检查买单委托是否有足够余额|已实现|
|NewOrderQty|NewOrder|检查委托数量是否合法|已实现|
|NewOrderPriceDeviation|NewOrder|检查委托价格是否偏离买卖盘口价格指定比率|已实现|
|NewOrderPriceLimit|NewOrder|价格是否超过涨跌停限制|已实现|
|NewOrderFrequency|NewOrder|委托是否超过配置频率|已实现|
|NewOrderStStockLimit|NewOrder|检查委托是否符合对ST股票的限制|未实现|
|SelfTradeInSingleAccount|NewOrder|单账户自成交检查|已实现|
|SelfTradeInMultipleAccount|NewOrder|多账户自成交检查|未实现|
|CancelOrderFrequency|CancelOrder|撤单委托是否超过配置频率|已实现|
|CancelOrderInterval|CancelOrder|撤单与委托的间隔是否大于指定值|已实现|
