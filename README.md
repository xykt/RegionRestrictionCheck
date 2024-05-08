<p align="center">
<img src="https://hits.seeyoufarm.com/api/count/keep/badge.svg?url=https%3A%2F%2Fmedia.ispvps.com&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=runs&edge_flat=false"/> 
<img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fxykt%2FRegionRestrictionCheck&count_bg=%233DC8C0&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=visits&edge_flat=false"/> 
<a href="/LICENSE"><img src="https://img.shields.io/badge/license-GPL-blue.svg" alt="license" /></a>  
</p>

## 流媒体解锁检测脚本 -  [Streaming Unlock Test Script (EN)](https://github.com/xykt/RegionRestrictionCheck/blob/main/README_EN.md)

**支持OS/Platform：CentOS 6+, Ubuntu 14.04+, Debian 8+, Alpine, MacOS, Android with Termux, [iOS](https://github.com/lmc999/RegionRestrictionCheck/wiki/iOS%E8%BF%90%E8%A1%8C%E8%84%9A%E6%9C%AC%E6%96%B9%E6%B3%95)**

![截图](https://raw.githubusercontent.com/xykt/RegionRestrictionCheck/main/reference/IMG/ScreenShot.png)

**使用脚本前请确认curl已安装**

````bash
bash <(curl -L -s media.ispvps.com)
````

##### 只检测IPv4结果：
````bash
bash <(curl -L -s media.ispvps.com) -M 4
````

##### 只检测IPv6结果：
````bash
bash <(curl -L -s media.ispvps.com) -M 6
````

##### 指定检测的网卡名称：
````bash
bash <(curl -L -s media.ispvps.com) -I eth0
````

##### 选择脚本语言为英文：
````bash
bash <(curl -L -s media.ispvps.com) -E
````

**或者直接运行以下Docker命令** (兼容ARM架构)
````docker
docker run --rm -ti --net=host xykt/regioncheck && docker rmi xykt/regioncheck > /dev/null 2>&1
````

## 脚本更新

2024/03/22 09:45 修复MyTVSuper，感谢[RikkaNaa](https://github.com/RikkaNaa)

2024/03/22 09:30 增加ChatGPT地区检测，更新英文原生/DNS解锁显示内容

2024/02/20 01:30 修正Docker运行报错的bug，补全全区域检测项目

2024/02/18 22:00 修复LineTV.tw

2024/02/17 16:00 修复Now E，感谢[RikkaNaa](https://github.com/RikkaNaa)

2024/02/12 00:45 增加Alpine系统支持

2024/02/09 23:59 Netflix页面改版导致原脚本判定出现错误，现已修正

2024/01/31 00:30 修复Youtube极小概率解锁类别判断错误问题

2024/01/08 13:01 增加TikTok解锁检测

2024/01/07 21:55 增加对动画疯、MyTVSuper、4GTV的DNS解锁检测

2024/01/04 18:55 增加独立的脚本运行计数器

2024/01/03 23:27 进一步增加DNS检测机制，增加代理服务器解锁检测，修正纯ipv6机器无法检测的bug

2024/01/02 23:00 增加双重DNS检测机制，修正原版日本流媒体检测报错，广告前置

2024/01/02 03:00 改进检测机制，杜绝了部分误判

2024/01/01 21:00 增加DNS/原生解锁检测机制

## 脚本贡献

**Acknowledgments:**

- 感谢[lmc999原作](https://github.com/lmc999/RegionRestrictionCheck)，本改版脚本由此进化而来

- 本脚本基于[CoiaPrant/MediaUnlock_Test](https://github.com/CoiaPrant/MediaUnlock_Test)代码进行修改

- [onoc1yn](https://github.com/onoc1yn) 提供多架构docker解决方案及Hulu Cookies加密方案

- 目前市面的流媒体解锁检测脚本都是从[Lemonbench](https://github.com/LemonBench/LemonBench)演化而来

**Contributors:**

<a href="https://github.com/RikkaNaa"><img src="https://avatars.githubusercontent.com/u/98643870?s=60&v=4" alt="@RikkaNaa" size="48" height="48" width="48" data-view-component="true"></img></a>

**Stars History:**
![Stargazers over time](https://starchart.cc/xykt/RegionRestrictionCheck.svg?background=%23FFFFFF&axis=%23333333&line=%2377dd77)



