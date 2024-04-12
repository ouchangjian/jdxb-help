# 远程开机

{% hint style="info" %}
<mark style="color:blue;">**判断设备是否支持远程开机**</mark>

1. 重启电脑设备进入BIOS的电源管理菜单
2. 查看菜单是否有Remote Wake Up或Wake on LAN等类似选项，否则不支持远程开机。
{% endhint %}

1. ## 进入BIOS

* 开机时反复按“DELTET”或“F2/F8/F12”等按键进入BIOS设置界面
* 具体按键可参考主板说明书或参考网络教程。

2. ## 开启唤醒功能

* 通常到“Power Managment（电源管理）”下寻找如下列选项或类似的配置项，并可以启用它。

```
"Boot on LAN";
"Wake on LAN";
"PME Event WakeUp",;
"Resume by MAC LAN";
"Wake-Up by PCI card";
"Wake Up On PCI PME";
"Power On by PCI Card";
"WakeUp by PME of PCI";
"Power On By PCI Devices";
"WakeUp by Onborad LAN";
"Resume By PCI or PCI-E Ddevice"
```

{% hint style="info" %}
**可视化图形的UEFI BIOS，可参考下列设置方式：**

&#x20; 高级 > 高级电源管理（APM）> 开启 Resume By PCI or PCI-E Ddevice（由 pci/pcie 设备唤醒）选项。
{% endhint %}

3. ## 系统设置

* 右键点击开始菜单-设备管理器，对网卡进行设置。

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

4. ## 添加被开机主机

* 通过发现服务，添加Windows3389远程桌面服务
* 当winPC离线后，在内网穿透列表可点击开机，远程唤醒该主机
