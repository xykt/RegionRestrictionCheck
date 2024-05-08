<p align="center">
<img src="https://hits.seeyoufarm.com/api/count/keep/badge.svg?url=https%3A%2F%2Fmedia.ispvps.com&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=runs&edge_flat=false"/> 
<img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fxykt%2FRegionRestrictionCheck&count_bg=%233DC8C0&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=visits&edge_flat=false"/> 
<a href="/LICENSE"><img src="https://img.shields.io/badge/license-GPL-blue.svg" alt="license" /></a>  
</p>

## Streaming Unlock Test Script 

**Support OS/Platform：CentOS 6+, Ubuntu 14.04+, Debian 8+, Alpine, MacOS, Android with Termux, [iOS](https://github.com/lmc999/RegionRestrictionCheck/wiki/iOS%E8%BF%90%E8%A1%8C%E8%84%9A%E6%9C%AC%E6%96%B9%E6%B3%95)**

![ScreenShot](https://raw.githubusercontent.com/xykt/RegionRestrictionCheck/main/reference/IMG/ScreenShot.png)

**Please make sure curl is installed before using the script**

````bash
bash <(curl -L -s media.ispvps.com)
````

##### IPv4 Only:
````bash
bash <(curl -L -s media.ispvps.com) -M 4
````

##### IPv6 Only:
````bash
bash <(curl -L -s media.ispvps.com) -M 6
````

##### Specify network adapter:
````bash
bash <(curl -L -s media.ispvps.com) -I eth0
````

##### English output:
````bash
bash <(curl -L -s media.ispvps.com) -E
````

**Docker Command** (Compatible with ARM)
````docker
docker run --rm -ti --net=host xykt/regioncheck && docker rmi xykt/regioncheck > /dev/null 2>&1
````

## Updates

2024/03/22 09:45 Fix MyTVSuper, thanks to [RikkaNaa](https://github.com/RikkaNaa)

2024/03/22 09:30 Added ChatGPT region detection, updated English native/DNS unlocking display content

2024/02/20 01:30 Fixed the bug of Docker running error and completed the full-region detection project

2024/02/18 22:00 Repair LineTV.tw

2024/02/17 16:00 Fix Now E, thanks to [RikkaNaa](https://github.com/RikkaNaa)

2024/02/12 00:45 Add Alpine system support

2024/02/09 23:59 The revision of the Netflix page resulted in an error in the original script judgment, which has been corrected.

2024/01/31 00:30 Fixed the problem of incorrect judgment of Youtube’s very unlikely unlock category

2024/01/08 13:01 Add TikTok unlock detection

2024/01/07 21:55 Added DNS unlock detection for Anime Crazy, MyTVSuper, and 4GTV

2024/01/04 18:55 Increase independent script running counter

2024/01/03 23:27 Upgrade DNS detection mechanism, add proxy server unlock detection, correct the bug that IPv6 hosts cannot detect

2024/01/02 23:00 Add a dual DNS detection mechanism, correct the original Japanese streaming media detection error, and pre-advertise

2024/01/02 03:00 Improved detection mechanism to eliminate some misjudgments

2024/01/01 21:00 Add DNS/Native unlock detection mechanism

## Contribution

**Acknowledgments:**

- Thanks to [lmc999 original work](https://github.com/lmc999/RegionRestrictionCheck), this revised script evolved from it

- This script is modified based on the code of [CoiaPrant/MediaUnlock_Test](https://github.com/CoiaPrant/MediaUnlock_Test)

- [onoc1yn](https://github.com/onoc1yn) provides multi-architecture docker solutions and Hulu Cookies encryption solutions

- The streaming media unlocking detection scripts currently on the market are all evolved from [Lemonbench](https://github.com/LemonBench/LemonBench)

**Contributors:**

<a href="https://github.com/RikkaNaa"><img src="https://avatars.githubusercontent.com/u/98643870?s=60&v=4" alt="@RikkaNaa" size="48" height="48" width="48" data-view-component="true"></img></a>

**Stars History:**
![Stargazers over time](https://starchart.cc/xykt/RegionRestrictionCheck.svg?background=%23FFFFFF&axis=%23333333&line=%2377dd77)

