## BlackIP
扫描CobaltStrike的恶意IP合集

## 原理
CobaltStrike通过Stager上线默认会发送CheckSum8验证，某些<b>网络空间测绘扫描器</b>、<b>沙箱</b>会根据此规则主动探测标记CS服务器。

## 数据来源
分布在世界各地的多台服务器自动监控并自动汇总去重，更新频率为<b>5分钟</b>，如有新增恶意IP将自动同步到Github仓库。</br>
[![BlackIP](https://cdn.gksec.com/20211117/xuIk8ggK/BlackIP.png "BlackIP")](https://app.cloudcraft.co/view/bf5b7390-594b-4ad2-bb5d-7a898ce470e3?key=e23674d9-d4b0-491d-89b0-7b3ada28c1ae&interactive=true&embed=true)

## 服务器状态监控：
https://status.gksec.com </br>
https://status.wuyoukm.top </br>

## 数据准确性
目前只收集<b>主动</b>探测<b>包括但不限于CheckSum8默认规则</b>的黑IP，证书/端口特征被标记不在本项目考虑范围之内。
通过特定算法实现99.9%的准确性，精准标记恶意扫描的IP。

## 如何防止被扫描/标
- 修改CS的上线特征（包括但不限于CheckSum8）
- ban掉这些IP
- 套一层反向代理
