## BlackIP
扫描CobaltStrike的恶意IP合集

## 原理
CobaltStrike上线默认会发送CheckSum8验证，某些扫描器会根据此规则爆破CS服务器。

## 数据来源
分布在世界各地的多台服务器自动监控并定期汇总。
服务器状态监控：https://status.gksec.com/

## 数据准确性
目前只收集主动探测CheckSum8的黑IP，证书/端口特征被标记不在本项目考虑范围之内。
通过特定算法实现99.9%的准确性，精准标记恶意扫描的IP。

## 如何防止被扫描
- 修改CS的上线特征（包括但不限于CheckSum8）
- ban掉这些IP
- 套一层反向代理
