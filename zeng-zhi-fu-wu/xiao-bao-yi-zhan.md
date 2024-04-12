# 小宝驿站

{% hint style="info" %}
* 开启小宝驿站，共享闲置带宽
* 可以赚取积分收益，积分可以兑换各类话费及影视会员卡
* 共享带宽为上行带宽，不影响观影、游戏及购物等体验
{% endhint %}

## **存储路径**

{% hint style="info" %}
* 由于设备系统的安全限制，小宝驿站不支持修改下载路径。
* 群晖修改路径：控制面板 ->共享文件夹 -> 选中OWSpeedup -> 点击编辑 -> 选择“所在位置”切换磁盘。
{% endhint %}

群晖：File Station/OWSpeedup；

海康：文件/下载/OWSpeedup；

联想：三方应用/OWSpeedup；

QNAP：Public/OWSpeedup。

***

## NAT类型

### **什么是NAT类型？**

* 具体NAT类型原理可查阅网络资料;
* 对于小宝积分而言，NAT类型的数值越低代表设备积分能力越强。

### **NAT类型检测**

* 下载NAT类型检测工具（NatTypeTester）
* 默认STUN server失效时，可使用stun.ionewu.com
* 根据NAT检测工具中NAT type测试的结果，对照下方信息确认自己的NAT类型：

<figure><img src="../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

* **`NAT1 → Full Cone NAT`**
* **`NAT2 → Address-Restricted Cone NAT`**
* **`NAT3 → Port-Restricted Cone NAT`**
* **`NAT4 → Symmetric NAT`**

### **NAT类型优化**

{% hint style="info" %}
📚路由相关配置可查阅[《路由优化指引》](https://yc.ionewu.com/jdb\_help/nat.html)
{% endhint %}

1. 尽可能少的路由层级；
2. 尽可能使用近端路由/光猫或电脑拨号上网；
3. 向运营商申请公网IP。

## 设备积分未到账

* 初次启动小宝积分，需要24-72小时的部署期
* 当日产生贡献的积分收益会在次日发放
