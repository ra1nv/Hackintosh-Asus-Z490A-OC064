# 14/04/2020
    本EFI理论适用于7，8，9代i7及以上带核显CPU
    使用前请确认自己平台解锁CFG和开启（或模拟）原生NVRAM
如若不会以上步骤，可以参考[独行秀才博客](https://shuiyunxc.gitee.io)<br>
附上OC引导配置说明[OpenCore配置文字说明.pdf](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/OpenCore%E9%85%8D%E7%BD%AE%E6%96%87%E5%AD%97%E8%AF%B4%E6%98%8E%E7%AC%AC%E5%9B%9B%E7%89%88.pdf)
# 配置/Feature
系统/OS：Catalina 10.15.5 beta
主板/motherboard：Asus-Z70A<br>
中央处理器/CPU：Intel Core i7-7700k 4.8Ghz-OC<br>
内存/memory：Corsair 3200Mhz(c15)-OC 8Gx2<br>
显卡/GPU：Sapphire 5500XT 8G / Intel HD Graphics 630<br>
固态/SSD：Intel 760P 512G<br>
无线网卡/Wireless：BCM943602CS<br>
雷电/Thunderbolt3 card：Asus ThunderboltEX 3
# 设置/Configuration
如有雷电卡，请尝试勾选ACPI->ADD->`Thunderbolt3-DTPG.aml` & `Thunderbolt3.aml`<br>以及Kernel->ADD->
`IOElectrify_10.15sdk.kext`<br>默认关闭HWP性能模式，如果你的CPU频率在4.8Ghz，勾选
Kernel->ADD->`CPUFriend.kext` & `CPUFriendDataProvider.kext`<br>如果显卡不是NAVI架构，请删除NVRAM->ADD->7C436110-AB2A-4BBB-A880-FE41995C9F82->boot-args中`agdpmod=pikera`

# 概况
开启核显加速硬解，正常使用隔空投送以及随航，开启原生HWP电源管理，驱动华硕雷电3

![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/DS.png)
![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/QQ20200414-012723@2x.png)
![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/QQ20200414-012750@2x.png)
![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/QQ20200414-012804@2x.png)
![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/QQ20200414-012835@2x.png)
![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/QQ20200414-013010@2x.png)
![image](https://github.com/ra1nv/Asus-Z270A-OC/blob/master/img/QQ20200414-013028@2x.png)

To be continue...
