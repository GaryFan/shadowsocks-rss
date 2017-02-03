# ShadowsocksR C# 版本4.1.0 #

获取高速ShadowsocksR账号：http://www.nap6.vip

ZeroNet:[shadowsocksr.bit](http://127.0.0.1:43110/shadowsocksr.bit)  
BitTorrent Sync：BHS55LP54SO7A434QBB5Z2O6B7A45B2BX  
发布链接：[https://github.com/breakwa11/shadowsocks-rss](https://github.com/breakwa11/shadowsocks-rss)  
服务端配置教程：[Wiki](https://github.com/breakwa11/shadowsocks-rss/wiki/Server-Setup) （含单用户和多用户）  
ShadowsocksR主要分支：[SSR C#](https://github.com/shadowsocksr/shadowsocksr-csharp), [SSR python manyuser](https://github.com/shadowsocksr/shadowsocksr/tree/manyuser), [SSR-libev](https://github.com/shadowsocksr/shadowsocksr-libev)  
Android APP: [SSR-android](https://github.com/shadowsocksr/shadowsocksr-android/releases)  
iOS APP： [Shadowrocket](https://itunes.apple.com/us/app/shadowrocket/id932747118)  
MAC APP：[ShadowsocksX-NG](https://github.com/qinyuhang/ShadowsocksX-NG/releases), [ShadowsocksX-R](https://github.com/yichengchen/ShadowsocksX-R/releases)  
其它不完全支持：[NEKit](https://github.com/zhuhaow/NEKit), [Wingy](https://itunes.apple.com/cn/app/id1178584911), [Potatso](https://itunes.apple.com/us/app/potatso-qiang-da-wang-luo/id1070901416)

推荐使用ZeroNet地址，或BitTorrent Sync免翻自动更新，最及时自动获取最新版本  
注意发布压缩包内有一个以sig后缀的签名文件（如果没有签名文件，即文件已经被修改过），**您应该使用GPG进行校验**  
公钥地址 [https://github.com/breakwa11/pubkey](https://github.com/breakwa11/pubkey)  
Key ID: A36AAA42  
Fingerping: 23AD 0055 4751 B956 174C  724A 87DF 7FAC A36A AA42  
Key ID: DA0F4B18  
Fingerping: CDFB 1D2E A63B 9149 3EAE  C35E D7CE 0EDE DA0F 4B18  
尽量在此处下载，以避免使用被篡改的版本。如果为了图方便在其它公开网络或下载站下载的，记得要做签名校验，签名是唯一凭证。

### 版本特点 ###
1. 全能代理，同一端口支持socks4/socks4a/socks5/http
2. 节点统计，包括延迟、连接数、当前下载速度、最高速度、出错率等等
3. 连接管理，随时断开指定节点的连接，或修改节点后自动断开
4. 协议转换，把UDP包封装于TCP里发送，或把TCP包封装于UDP里发送
5. 多重代理，通过设置前置socks5/http代理，可达到任意重代理
6. 协议插件，支持自定义协议和协议混淆，详见[ShadowsocksR插件文档 <<== 要了解插件的点这里看](https://github.com/breakwa11/shadowsocks-rss/blob/master/ssr.md)

你要是有兴趣和我联系的话，特别是编程技术上的支持，那就到  
Twitter: [@breakwa11](https://twitter.com/breakwa11)  
聊天室: [https://gitter.im/breakwa11/shadowsocksr](https://gitter.im/breakwa11/shadowsocksr)  
Riot: `#ssr:matrix.org`  
社区: [ShadowsocksR](https://plus.google.com/communities/117390969460066916686)  
Blogger: [https://breakwa11.blogspot.com](https://breakwa11.blogspot.com)  
Google Group: [ShadowsocksR](https://groups.google.com/forum/#!forum/shadowsocksr)  
TOX: D211FF64C848E03161700E74714A2100D363757AED4982F35486CC0713577C2F356B7DD84CAB  

### 更新记录： ###
版本4.1.0 *2017-01-24*  
1.修正自启动显示  
2.修正socks5认证处理  
3.DNS设置支持使用冒号分隔端口号，IPv6地址需要使用中括号，如[::1]:53  

版本4.0.9 *2017-01-21*  
1.修正自启动设置(需要管理员权限)  
2.优化下载时CPU占用  
3.端口设置窗口中文界面

版本4.0.8 *2017-01-19*  
1.修正DNS查询  

版本4.0.7 *2017-01-18*  
1.修正负载均衡策略  
2.修正代理规则  

版本4.0.6 *2017-01-17*  
1.负载均衡在组内切换单独选项，可应用到任何其它策略  
2.端口设置内可指定使用节点或指定组，或留空不指定（选择所有）  
3.界面调整，使用数字控件  
4.系统代理模式区分“直连”及“不修改”，“不修改”时可避免与其它代理软件冲突  
5.隐藏弱加密（但可输入使用）  
6.DNS缓存优化，查询不到时可使用旧的结果

版本4.0.5 *2017-01-08*  
1.添加协议参数  
2.代码整理（嗯，从外观是看不出来的）

版本4.0.4 *2017-01-03*  
1.修正Bug  
2.添加log显示窗口  
3.修正64位系统下的内存占用

版本4.0.3 *2016-12-25*  
1.修正Bug  

版本4.0.2 *2016-12-24*  
1.修正64位配置  
2.修正无法更新PAC  
3.调整消息提示和更新提示  
4.连接Bug修正及剪贴板导入修正  
5.设置系统代理修正  
6.加密性能优化  
7.调socks5及http connect握手响应时机

版本4.0.1 *2016-12-12*  
1.修正自效验在部分环境下的效验错误  
2.从剪贴板导入多个节点时按次序导入  
3.修正端口设置在无设置项时会挂的BUG  
4.在x64上运行为64位应用程序  
5.修正在部分系统下不能正常使用`auth_aes128_md5`的问题  
6.找了个台湾妹子和帅哥校对正体部分

版本4.0 *2016-12-03*  
1.自动修正重复节点ID  
2.端口配置面板，可配置为端口映射或指定节点代理  
3.增加加密方式none（不加密），aes-128-cfb8等  
4.privoxy模板清空使得仅返回错误码，由浏览器决定显示内容  
5.优化DNS查询  
6.支持清空历史流量（在服务器统计窗口菜单内）  
7.通过本地及网络做简单的exe自效验  
8.修正上传时的超时处理及程序错误，及上传速度统计修正  
9.支持超长备注和组名  
10.支持自定义任务栏图标及服务器统计窗口图标（在exe同目录下放icon.png文件）  
11.支持配置文件加密（含transfer_log）  
12.国内IP列表更新  

注意事项：

- 端口配置面板可以菜单的服务器那找到，或alt+鼠标左键
- aes-128-cfb8需要libeay32.dll的支持，但如无特殊需要并不建议使用
- 右键菜单的顶部将会实时显示自效验结果，仅启动时做效验，**若效验失败程序将自行退出，所以exe和签名文件务必放在一起**。效验通过的会同时在那里显示短小的公告之类的，更新提示也同时将这样进行，也即其它修改版（甚至即使只是重新编译，不同环境编译的二进制文件不一样）都不会收到更新提示及公告。如果那个菜单变得可点击，记得点击看看。
- 如果设置了配置密码，那么转移或复制配置时需要同时把gui_config.json和transfer_log.json一起复制，否则如果后者不复制，则会因为解密失败导致历史流量清空
- 如果设置了配置密码，建议退出后手动把整个temp目录删除，否则log里面会泄露节点地址

版本3.9.6 *2016-10-17*  
1.本地API认证码（含PAC部分），抵抗部分XSS（此攻击可探测是否在运行SS-C#）  
2.增加代理规则，可绕过局域网及大陆IP（或非大陆IP），在选项里设置无污染DNS可获得最佳效果  
3.再弄DPI问题  
4.UDP细节问题修正  
5.修正`tls1.2_ticket_auth`上传数据错误

- 注意，在使用二级代理时，使用绕过局域网及大陆IP的代理规则，效果是局域网直连，大陆IP通过二级代理连接目标网站，其它的通过二级代理连接SSR服务端再连接到目标网站。启用代理规则为绕过局域网及大陆IP时，所有通过此客户端代理的都有绕过的效果，不需要设置PAC，系统代理可直接设置为全局  
- 关于XSS攻击，此问题从C#支持PAC第一天起，已经有这个漏洞，任何网站均可通过恶意的代码探测出你是否在运行C#版客户端（特别是数字或百毒的站），类似方式百毒曾经用于获取用户手机信息（在手机上监听特定端口，然后网页上通过JS访问127.0.0.1:xxxx以获得用户手机号、IMEI、通讯录、地理位置等等信息），所以我想这可能是win10早期默认阻止连接127.0.0.1地址的原因，特别建议你不要使用默认的1080端口做代理  
- 压缩包内有一个delegated-apnic.txt文件，是APNIC上记录分配到CN的IP地址段，可自行在APNIC上下载更新。当然如果你把这个文件删除了，或者没带上，那么使用绕过局域网及大陆IP的代理规则时除了局域网外任何IP都将不会绕过


版本3.9.5 *2016-10-12*  
1.重新支持rc4  
2.协议列表移除auth\_aes128，添加auth\_aes128\_md5和auth\_aes128\_sha1  
3.协议内填充字节全部随机化  
服务端需要更新到2.9.5才能使用新增协议


版本3.9.4 *2016-10-09*  
1.自定义生成二维码  
2.细节Bug修正，编辑服务器界面调整  
3.服务器统计列表右键菜单改为窗口菜单且添加断开所有连接  
4.选项设置窗口添加默认值设置  
5.修正关闭软件时没有还原系统代理设置  
6.修正重连逻辑（部分情况下导致发送了错误的数据）  
7.按新版服务端逻辑优化（服务端须为2016年10月3日以后更新的版本）  
8.增加代理规则，设置为socks5下亦可设置绕过局域网（不需要PAC支持）  
简单来说，代理规则是所有连接到SSR客户端都会走的规则（不局限于浏览器），将部分替代PAC的功能


版本3.9.3 *2016-10-04*  
1.协议列表移除auth\_sha1和auth\_sha1\_v3  
2.优化负载均衡策略  
3.优化及修正超时断开逻辑  
4.除鼠标中键添加ctrl+左键打开服务器统计窗口  
注：服务端需配合更新以使优化效果更明显，配合auth协议食用风味更佳。


版本3.9.2 *2016-09-28*  
1.添加auth\_aes128  
2.优化负载均衡策略，自动识别不可用节点  
3.优化本地代理连接握手效率


版本3.9.1 *2016-09-27*  
1.修正verify\_sha1的UDP接收错误  
2.修正DNS错误  
3.添加服务器加在当前位置的后面  
4.细调连接方式保持握手包和数据包一起发送


版本3.9.0 *2016-09-20*  
1.增加auth\_sha1\_v4协议  
2.增加gfw_list备用地址  
3.配置窗口不隐藏协议混淆  
4.连接性能优化  


版本3.8.9 *2016-09-18*  
1.服务器菜单分组显示，右键菜单整理（非常苗条了喵）  
2.从配置文件导入服务器  
3.DPI模式调整  
4.修正特殊情况下的连接异常，导致非正常中断  


版本3.8.8 *2016-09-13*  
1.修正UDP连接及通过二级代理的UDP连接  
2.SS节点自动隐藏SSR配置项，为SS用户有原版相似的配置体验  
3.界面各种字体和大小的调整  


版本3.8.7 *2016-09-10*  
1.添加连接超时选项  
2.图标颜色细调（避免黄色时与白色太相近）  
3.连接参数修正  
4.真·DPI修正  
5.服务器统计窗口优化，不再闪烁  


版本3.8.6 *2016-09-04*  
1.支持扫任意二维码，非SS/SSR的码显示扫描结果  
2.添加auth\_sha1\_v3协议  
3.修正UDP over TCP  
4.高DPI下界面的全面修正  
5.系统代理模式菜单项调整  
6.服务器编辑界面细调，显示过二维码后下次可隐藏图片  
7.服务器统计界面打开时焦点自动切换到选择的节点上  
8.Pofile网络模块，效率优化  
9.修正google doc编辑时掉线问题


版本3.8.5.2 *2016-08-26*  
1.扫码增强，提升扫码识别能力  
2.网络连接逻辑调整  
3.服务器统计界面右键可导出当前或所有开启节点的链接  
4.编辑界面手动添加时复制当前节点配置  
5.服务器统计界面DPI适配  
6.扫码的DPI适配（C#下不同DPI远程桌面会位置错误，C#的BUG）  


版本3.8.5.0 Release *2016-08-23*  
1.支持正体中文  
2.增强auth\_sha1的混淆力度


版本3.8.5.0 *2016-08-19*  
1.网络部分重构  
2.注册表读写调整（针对win10）  
3.测速再调整，更实时准确


版本3.8.4.4 *2016-08-17*  
1.连接keepalive方式调整  
2.privoxy开启连接共享


版本3.8.4.3 *2016-08-15*  
1.删除auth\_simple，tls\_simple  
2.服务器统计列表浮点精度调整  
3.仅点击链接时显示二维码  
4.速度统计调整  


版本3.8.4.2 *2016-08-08*  
1.连接占用BUG修正  
2.调整图标  
3.打开日志使用系统默认程序  
4.连接错误统计BUG修正


版本3.8.4 *2016-08-05*  
1.支持二级代理的http connect自定义useragent  
2.自定义DNS  
3.base64生成去掉填充符  
4.上传速度  
5.调整图标


版本3.8.3 *2016-07-08*  
1.tunnel模式下转发SSH连接修正  
2.优化服务器统计的更新  
3.在auth\_sha1\_v2下支持心跳包（需更新服务端，且开启超时时间）  
4.新ssr链接格式，简化解析，且防特殊字符  
5.新增控制台版本（仅支持socks5代理，需要自己编译）  
6.新增动态加载libeay32.dll及其部分加密  
7.修正杀掉Privoxy进程的名字


版本3.8.2 *2016-06-14*  
1.连接管理优化，解决偶尔的资源泄露及偶尔的死锁  
2.支持tunnel模式，即端口映射（但未实现图形界面配置的部分）  
3.优化pac参数设置，可免ip地址设置项，默认127.0.0.1  
4.API支持修改除token外的所有配置（可用于实现自动更新节点功能）  
5.彻底移除TCP over UDP功能（如有此需求请使用kcptun）  
6.支持简易伪装privoxy进程名（例如把主程序改为qq.exe），以躲避国产流氓软件获取进程列表被关键字检测  

版本3.8.1.2 *2016-05-28*  
1.优化并修正UDP加解密  
2.缺少注册表代理设置项时加上

版本3.8.1.1 *2016-05-24*  
1.解密遇到错误UDP包时忽略  
2.扫码细节调整，兼容带冒号的密码  
3.增加同一目标地址保持同一节点的时间（3分钟），可通过配置文件修改  
4.新增http_post混淆

版本3.8.1 *2016-05-19*  
1.二级代理socks5修正  
2.优化历史流量记录（与以前版本不兼容）  
3.解密首包长度小于IV时出错的BUG修正  
4.统计窗口拉伸优化，自动填充  
5.实验性功能：支持基本的API，可获取当前所有节点的配置信息和统计信息  
此API目前可直接使用浏览器访问 http://127.0.0.1:1080/api?token=&action=config 获得结果  
端口号1080修改为你的本地端口，如需统计信息，那么使用action=statistics  
以下隐藏一大堆TODO列表

版本3.8.0.7 *2016-05-17*  
1.PAC支持返回二级代理地址  
这功能用于在特殊局域网（如某些公司）内必须通过指定代理才能上外网的情况，  
在判断不需要经过SS节点时，也使用指定的二级代理地址连接，  
避免只能全局通过SS节点。此功能必须与二级代理功能一起开启。

版本3.8.0.6 *2016-05-13*  
1.服务器编辑列表分组名显示的各种Bug修正  
2.DPI配置修正  
3.添加自动调整服务器统计表格宽度的菜单项  
4.服务器统计窗口各种自适应

版本3.8.0.5 *2016-05-10*  
1.服务器编辑列表显示分组名  
2.负载均衡策略添加在所选组中切换  
3.不同DPI下的显示调整  
4.实验性功能：支持长期记录节点已通过的流量（按服务器名，不管端口）  
数据保存于transfer_log.json，如要清空数据，关掉软件删除此文件即可。此功能需要大家反馈改进意见。

版本3.8.0.4 *2016-05-06*  
1.优先相同节点连接同一地址菜单项初始化修正  
2.移除在线PAC残留功能  
3.代码瘦身  
4.添加指定UDP端口功能  
5.隐藏高级选项  
其它说明：指定UDP端口功能主要用于希望TCP端口走80或443之类，而UDP可以走原端口，以完整支持服务端单端口多用户支持。  
或者用于去除特征之用（TCP与UDP总走同一个端口这就是个特征）

版本3.8.0.3 *2016-05-04*  
1.privoxy只监听本地地址  
2.添加仅通过大陆常见域名列表（翻回国内用）  
3.优化历史统计  
4.移除在线PAC功能  

版本3.8.0.2 *2016-04-26*  
1.重命名ssr_privoxy，避免被原版SS强制杀掉进程，和谐共处╮(￣▽￣)╭  
2.添加ZeroNet域名  
3.支持服务器记录窗口置顶，在窗口的右键菜单中切换  

版本3.8.0.1 *2016-04-19*  
1.服务器统计窗口拖放优化，弹出优化  
2.支持相同地址优先选择相同节点连接，可解决开启负载均衡时google搜索验证码及各种登陆验证(1分钟内有效)  

版本3.8.0 *2016-04-17*  
1.移除tls_simple  
2.增加tls1.2\_ticket\_auth  

版本3.7.6.2 *2016-04-15*  
1.privoxy模板萌化尝试  
2.添加ZeroNet  

版本3.7.6.1 *2016-04-12*  
1.修正部分情况下程序随机异常退出  
2.支持pac参数实现本地动态代理地址，可指定目标"ip","port","type"  
3.设置privoxy的超时参数  
PAC配置示例：`http://127.0.0.1:1080/pac?ip=127.0.0.1&port=9050&type=socks5&t=123`  
type参数指定为s5或socks5使用socks5代理，s4同理，不指定时使用http代理  
其中参数t的值随意，目的是防浏览器对其缓存（出现缓存的情况就修改一下t的值使得URL变化了即可）

版本3.7.6 alpha *2016-04-01*  
1.服务器分组，支持按组开启/关闭/排序  
2.增加http代理域名白名单，允许自定义（在bypass.action）  
3.http代理自动跳过本地局域网  
4.采用实际发包响应时间计算延迟值（二级代理下亦能得到正确延迟）  
5.彩色图标显示当前代理配置模式(绿色表示开了系统代理且使用PAC模式，如果不开PAC就是青色（绿+蓝），如果不开系统代理就是蓝色，如果开了负载均衡就在前面的颜色里混合进红色)  
6.添加privoxy模板文件(压缩包里的templates目录和主程序要放在一起)  
7.修正超时处理，多连接优化  
8.缓冲区长度Bug修正  
9.privoxy被杀后的重启修正  
10.privoxy更新到最新版本  
11.修正较大UDP包接收不完整的错误  
注意：指定使用socks5协议时则为强制代理，不管目标地址，通常用于作为其它软件的二级代理（如tor）  
http代理域名白名单功能，默认会在gfw_whitelist项目里下载一个常见国内域名列表。  
但对于一些直接使用IP地址连接的国内视频网站建议配合**绕过大陆常见域名PAC**或**绕过大陆IP的PAC**，此PAC会对IP地址判断是否为国内  
此测试版本暂不支持TCP over UDP，有此需求的话请暂时使用旧版本  
privoxy的模板文件萌化期待  

版本3.7.4.1 *2016-02-01*  
1.修正超时统计  
2.优化统计流程  
3.发现协议非标准不断开连接  

版本3.7.4 *2016-01-22*  
1.增加插件auth\_sha1\_v2  
2.服务器统计增加“实际下载”列  
3.log文件按月份分离保存

版本3.7.3.1 *2016-01-11*  
1.修正部分http(s)连接错误  
---- (3.7.2 beta *2016-01-09*)  
2.重写http代理实现  
3.支持自定义abp.txt以替代gfwlist  
---- (3.7.1 alpha *2016-01-05*)  
4.支持设置验证密码，设置验证密码后允许任何IP连接，带验证时不支持socks4  
5.本地代理免验证  
6.空连统计清零规则调整

版本3.7.0 *2015-12-29*  
1.支持chacha20-ietf加密  
2.兼容FIPS设置  
3.支持UDP协议定制  
4.完整支持verify\_sha1

版本3.6.9 *2015-12-21*  
1.http\_simple插件支持自定义完整header  
2.错误统计方式调整，只记录最近100次连接的情况  
3.常见协议的正确性测试，可检测出密码错误或协议错误等  
4.仅当解密错误或协议错误或网络错误时，才自动禁用节点  
5.tls1.0插件协议修正（需要同时更新服务端）

版本3.6.8 *2015-12-18*  
1.连接超时处理优化，避免长时间连接等待（重连次数大于0时启用，建议设置5）  
2.重连机制增强，客户端未发送有效数据前均能重连  
3.无数据超时仅断开远端，满足上一条的情况下能重连  
4.更新PAC时防止缓冲  
5.tls1.0插件协议修正（需要同时更新服务端）

版本3.6.7.1 *2015-12-15*  
1.修正随机数发生方式  
2.配置界面次序调整  

版本3.6.7 *2015-12-14*  
1.调整流量计算方式，以客户端到ss服务端的TCP/UDP数据包大小为准（py服务端也已调整）  
2.verify\_deflate的BUG修正  
3.增加混淆插件tls1.0\_session\_auth  
4.负载均衡的“选中优先”bug修正  
5.服务端`auth_simple`和`auth_sha1`支持配置客户端上限

版本3.6.6 *2015-12-03*  
1.增加插件auth\_sha1  
2.过滤非局域网连接请求

版本3.6.5 *2015-11-24*  
1.移除内置http代理功能  
2.支持切换前置代理类型(Socks5/http tunnel)  
其它说明：http tunnel是指支持代理https连接的http代理，可以通过UDP over TCP方式使用UDP，不能使用原生UDP。特别注意某些代理软件某些功能上有BUG，会导致代理失败（如CCProxy开启二级代理时，不开启二级代理是正常的）  
前置代理类型中的“TCP端口转发”的混淆插件还没写

版本3.6.4.1 *2015-11-19*  
1.关闭内置http代理时privoxy的转发BUG修正  
2.不重复保存配置

版本3.6.4 *2015-11-18*  
1.支持verify\_sha1（即libev的OTA）  
2.UDP over TCP 实现调整，避免与verify\_sha1冲突  
3.UDP over TCP 细节bug修正  
4.显示超时次数列  
5.内置http代理部分bug修正  
6.特殊情况下缓冲区溢出修正

版本3.6.3.4 *2015-11-16*  
1.移除部分影响速度的调试代码  
2.修正扫码时混淆参数未解码  
3.增加插件字段

版本3.6.3 *2015-11-10*  
1.实现CONNECT方法的http代理，减少访问https站的连接数  
2.实现基本的http代理支持，更少资源占用（但存在BUG，试用阶段）  
3.内置http代理启用开关（开启后privoxy不会运行）  
4.修改生成链接格式，与SSR android兼容  
5.在服务器配置的“备注”前打钩则把备注加在链接（二维码）内  
6.支持前置socks5代理地址填写域名  
7.增加一个常见域名列表（即白名单），foxyproxy可使用此列表替代，  
&nbsp;&nbsp;&nbsp;&nbsp;因foxyproxy使用绕过大陆IP列表访问facebook等站会很卡  
其它说明：对于https站点，不管启不启用内置http代理，均无影响，  
启用内置http代理会影响http站点，目前发现的问题是页面元素较多时有部分请求不正常，用chrome打开时有一定概率变成空白页。

版本3.6.2 *2015-11-02*  
1.插件分类，独立出TCP协议字段（旧配置部分节点需要修改配置）  
2.稳定性增强  
3.更详细的log输出

版本3.6.1 *2015-10-27*  
1.多开时允许分别开机自动启动（更换前要把以前的自启动去掉）  
2.检测协议错误  
3.调整自动禁用节点的计算方式  
4.修正自动重连时没有更换混淆插件  
5.编辑节点后保持当前选择的节点  
6.添加auth\_simple混淆插件  
7.DNS缓存修正  
8.FIPS设置检查  
**附python部分**：  
版本2.6.12  
1.稳定性修正（目前最为稳定版本）  
2.添加auth\_simple混淆插件  
3.TCP分包处理修正  
4.IPv6优先  
5.混淆插件客户端部分完成支持

版本3.5.9 *2015-10-16*  
1.增强XP下的兼容性  
2.gfwlist模板不本地保存，精简exe大小  
3.gfwlist以及默认pac跳过局域网地址

版本3.5.8 *2015-10-15*  
1.增加插件参数字段  
2.PAC兼容性调整  
3.privoxy服务运行前先停止  
4.缓冲区优化

版本3.5.7 *2015-10-12*  
1.修正退出时有一定机率没退出完全的问题  
2.解决两个verify插件在部分情况下会越界错误  
3.添加绕过局域网的PAC，以替代全局模式  
4.修正系统代理在部分环境下手动取消失败的问题  
5.保证在使用PAC模式下即使强行结束客户端IE也能正常使用

版本3.5.6 *2015-10-09*  
1.增加混淆协议插件`verify_deflate`  
2.修正`tls_simple`, `random_head`的BUG

版本3.5.5 *2015-10-08*  
1.配置中remarks字段改回原文

版本3.5.4 *2015-10-08*  
1.调整插件接口，减少计算量和Bug修正  
2.网络缓冲的bug修正  
3.备注采用urlsafe-base64编码  
4.链接字段增加obfs-plugin  
5.其它编码错误修正

版本3.5.3 *2015-10-07*  
1.简化操作，**单击** 或 **shift+单击** 任务栏图标弹出配置窗口  
2.增加插件接口  
3.增加混淆协议插件`verify_simple`  
4.调整“连错”归零逻辑，避免插件的混淆返回干扰  
5.细调负载均衡，避免某个节点同时连接数大多  
6.修正端口重新监听时的异常

版本3.5.2 *2015-09-30*  
1.软件更新提示方式调整，点击气泡不弹窗  
2.注册表键值更名，避免与原版冲突  
3.Privoxy监听端口随机，不再默认为8123，避免与原版冲突  
4.移除“空连”错误统计  
5.修改图标  
6.移除table和rc4加密  
7.整理和简化右键菜单，配置移入选项设置

版本3.5.1 *2015-09-27*  
1.增加混淆协议插件`tls_simple`, `random_head`  
2.`http_simple`混淆增加随机路径和随机useragent  
3.更新配置不断开现有连接  
4.不开启系统代理时，系统代理菜单不置灰（PAC有效）

版本3.5.0 *2015-09-22*  
1.混淆协议插件`http_simple`  

版本3.4.4 *2015-09-19*  
1.设置界面拆分，区分编辑服务器和全局设置  
2.TCP连接协议改用下拉列表选择，字段名调整，相应节点要重新配置  
3.切换节点开关状态后立即保存设置  
4.调整随机数发生器，避免产生相同IV

版本3.4.3 *2015-09-16*  
1.服务器统计列的下载或上传刷新状态修正  
2.保存节点禁用状态  
3.增加按时间段切换服务器规则（每10分钟切换，或遇到连续出错时切换）

版本3.4.2 *2015-09-09*  
1.节点修改或删除后无引用的连接自动断开  
2.隐藏混淆UDP协议选项  
3.更新记录加入具体日期  
4.首包发送方式调整

版本3.4.1 *2015-08-28*  
1.增加新TCP连接协议

版本3.4.0 *2015-08-24*  
1.使用新的GFWList地址  
2.增加一个实验性功能TCP over UDP（目前有BUG，轻度使用还可，需要使用相应的服务端）

版本3.3.6 *2015-08-19*  
1.修正“自动禁用出错服务器”选项保存的问题  
2.所有临时文件全部放到./temp/下  
3.连接方式不同也视为不同服务器分别统计  
4.删除升级提示检查  
5.删除实验性功能代码并开源https://github.com/breakwa11/shadowsocks-csharp

版本3.3.5 *2015-08-17*  
1.合并部分主干代码，改用privoxy替代polipo（主程序增大140Kb）  
2.增加“低错误优先”的随机方式  
3.细调“低延迟优先”的算法  
4.增加“自动禁用出错服务器”选项  
5.连接超过超时秒数后断开算作“超时”

版本3.3.4 *2015-08-13*  
1.修正打开统计列表后，程序退出不正常的错误  
2.修正UDP over UDP的连接错误  
3.修正二重代理时UDP连接错误

版本3.3.2 *2015-08-12*  
1.合并部分主干代码  
2.断开当前所有连接功能  
3.优化统计窗口资源占用

版本3.3.1 *2015-08-06*  
1.修正连接数统计和管理错误  
2.修正多重代理时UDP代理错误  
3.重新实现UDP over TCP（与之前版本不兼容，以前的实现不正确，服务端需更新）

版本3.2.2 *2015-07-31*  
1.修正UDP下chacha20加密错误以及内存泄露  
2.提升UDP下加解密速度  
3.优化统计计算速度  
4.随机选择服务器改名负载均衡  
5.统计列表简化显示效果，减少卡顿  
6.自动更新方式调整

版本3.2.0 *2015-07-26*  
1.修正部分TCP连接失败的问题  
2.增加Socks5代理设置

版本3.1.4 *2015-07-23*  
1.调整TCP发包方式，把首协议包与第一个数据包连接发送  
2.移除混淆TCP选项  
3.服务端统计三列错误统计列改用“连错”列代替  
4.不要把版本号看成圆周率（明明差一个小数点）

版本3.1.3 *2015-07-16*  
1.本地连接的TTL支持，默认TTL=0（0表示不启用）  
2.重连次数的保存修正

版本3.1.2 *2015-07-14*  
1.连接统计窗口排序修正  
2.重连次数配置（默认值3）  
3.UDP over UDP选项更换为UDP over TCP，即高级选项全不打钩为通用设置，通用于所有服务端  
4.log文件和polipo放于temp子目录  
5.统计窗口数值格式化调整  
6.解决config问题，移除config文件  
7.允许密码显示

版本3.1.1 *2015-07-13*  
1.合并主干部分代码  
2.增加混淆UDP选项  
3.支持接收混淆UDP包  
4.连接数统计修正  
5.鼠标中键点击任务栏图标弹出服务器连接统计窗口  
6.修正配置界面部分环境下按钮不显示  
7.附加config文件避免部分系统运行异常  
8.改用7zip压缩，减少一半体积

版本3.0.1 *2015-07-09*  
1.配置保存bug修正  
2.右键菜单整理  
3.配置界面调整  
4.修正UDP握手协议实现与ProxyCap兼容  
5.加入源md格式说明文档

版本3.0 *2015-07-05*  
1.软件更名  
2.修正 UDP over UDP 的加解密错误

版本2.3.2 *2015-06-29*  
1.修正ipv4连接的问题  
其它：目前已知使用pc版微信发图发文件会导致polipo崩溃，建议改用Provixy，具体使用方法可以参考网上教程

版本2.3.1.9 *2015-06-28*  
1.修正http连接会出现连接失败的问题（同时修正了自动更新和pac更新）  
2.增加连接管理，双击连接数即可断开该节点现有连接  
3.增强UDP连接兼容性  
4.更新地址可以配置窗口点击

版本2.3.1.8 *2015-06-26*  
1.支持TCP协议头混淆（需服务端更新支持）  
2.UDP包混淆（需服务端更新支持）  
3.支持UDP包通过 UDP Relay 转发（需服务端更新支持）  
4.支持Socks4/Socks4a协议  
5.局域网共享时支持同时监听IPv4/IPv6  
6.配置添加UDP包通过方式  
7.配置添加TCP协议头混淆

版本2.3.1.7 *2015-06-19*  
1.IPv6连接修正  
2.随机时“按次序”方式的bug修正  
3.IPv6地址显示方式调整  
4.空连统计包含连接重置等错误  
5.服务器连接统计列排序功能  
6.取消自动关闭无效服务器，防误判  
7.手工检查更新

版本2.3.1.6 *2015-06-11*  
1.增加随机选择服务器的方式  
2.连接数统计修正  
3.支持代理UDP（以TCP转发），需要服务端更新

版本2.3.1.5 *2015-06-04*  
1.调整配置窗口的设置体验  
2.软件自动更新支持

版本2.3.1.4R2 *2015-06-03*  
1.修正polipo某些情况下运行异常  
2.修正连接统计窗口一些错误  
3.修正部分dns错误未处理的问题  
4.三次错误后自动关闭无效服务器  
5.增加ChnIPList的pac，国内不代理，国外全走代理  
6.调整连接统计窗口列顺序  
7.节点自动重连尝试（开启随机选择服务器时，第一次重连相同节点，第二次、第三次选择其它节点）  
8.从剪贴板复制多行文本地址功能修正  
9.服务器配置显示二维码，增加列表高度

版本2.3.1.4 *2015-06-01*  
1.polipo配置修正  
2.使用当前目录运行polipo，完美支持多开（端口同时支持socks5和http协议）  
3.增加当前下载速度统计，以及最大下载速度记录  
4.连接统计窗口优化显示效率  
5.服务器配置显示ss链接，以便快速复制  
6.连接统计窗口支持手工调整列宽

版本2.3.1.3 *2015-05-18*  
1.服务器的DNS缓冲（TTL=600），让直接填写域名与写IP一样稳定  
2.服务器连接状态记录，含上传下载流量，连接延迟统计，连接错误统计  
3.服务器独立开关，在连接状态的“开”一列，鼠标点击之，红色为关闭  
4.连接记录清除，在连接状态的错误记录三列，双击则重置错误数，双击百分比列则重置本服务器的所有信息  
5.统计列表标题显示监听方式及端口（方便多开的时候对应上）  
6.从剪贴板复制地址，方便从ss://xxxx这种格式快速输入

版本2.3.1.2 *2015-05-11*  
1.允许程序多开  
2.延迟统计，自动在低延迟服务器之中选择（高延迟的也会有低概率选取到）  
3.二维码菜单位置变动  
4.偶然会程序崩溃的问题不确定解决了没有，如还有发生请联系作者

版本2.3.1.1 *2015-05-03*  
1.随机选择服务器

### License ###
GPLv3

### Contact ###
[GPG pubkey](https://github.com/breakwa11/pubkey)
