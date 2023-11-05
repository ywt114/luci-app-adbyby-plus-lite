## 简介

项目名：luci-app-adbyby-plus-lite

别看项目名多了一个lite，包名还是原来的名称，这代表着是基于原来版本的一个分支。

简单点说就是让它安心走HTTP流量，DNS的被移除了。

其实还是做了不少的调整，不仅优化了plus模式，还让它更能协调，也降低了非全局下对路由器的负担和对其他插件的可能性冲突。更新规则也不会引发整体上不能网的情况。自定义规则修改也不需要再重启路由等等。

移除了对adbyby的安装依赖，但加入了主动下载主程序的功能。替换了主过滤规则。

## 三个模式说明

- 全局

- Plus+

- 手动代理

第一个，全局，相当于全绑了。

第二个，Plus+，列表内才走adbyby流量，这就意味着需要`ipset`支持。

第三个，手动代理。意思是牢房ADBYBY已经备好了，但别想我主动工作。你想让谁进去蹲就手动-j，改走端口`8118`也可以。`8118`是adbyby默认的监听端口。手动模式我已经优化好了，但这属于别人的进阶模式。

客户端模式，不受上面三个影响。优先级最高。也就是绑定局域网IP的那块。

## 注意

没有安装adbyby本体且首次使用，请在启用之前，先选择架构，应用并保存后，再启用本应用。

## 更新地址
- md5地址更新为:https://cdn.jsdelivr.net/gh/kongfl888/ad-rules/md5.json
- lazy地址更新为:https://cdn.jsdelivr.net/gh/kongfl888/ad-rules/lazy.txt
- video地址更新为:https://cdn.jsdelivr.net/gh/kongfl888/ad-rules/video.txt
## 添加了第三方规则列表地址
- https://cdn.jsdelivr.net/gh/cjx82630/cjxlist/cjx-annoyance.txt
- https://easylist-downloads.adblockplus.org/easylistchina.txt
- https://easylist-downloads.adblockplus.org/easyprivacy.txt
- https://easylist-downloads.adblockplus.org/easylist.txt
- https://raw.githubusercontent.com/Spam404/lists/master/adblock-list.txt
- https://raw.githubusercontent.com/bongochong/CombinedPrivacyBlockLists/master/cpbl-abp-list.txt
- https://anti-ad.net/easylist.txt
- https://anti-ad.net/anti-ad-for-dnsmasq.conf
- https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt
- https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt

## 以上源均来自于以下地址
- https://adblockplus.org/zh_CN/subscriptions
- https://github.com/privacy-protection-tools/anti-AD
- https://anti-ad.net
- https://github.com/cjx82630/cjxlist

## 致谢

感谢

- kongfl888项目

- adbyby项目

- lean/luci/luci-app-adbyby-plus 分享者及贡献者

- 第三方规则的分享者（附带了cjx）等
