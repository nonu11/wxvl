#  IBM 备份服务漏洞让攻击者能够提升权限  
邑安科技  邑安全   2025-06-16 08:34  
  
更多全球网络安全资讯尽在邑安全  
  
![](https://mmbiz.qpic.cn/mmbiz_png/1N39PtINn8vMlQicGDibZXZLarrZLBK1DLdMEzGjMk1dxsI1vu5uktAOugVMhNI0OaRKEdfUulb0ou29hYicyGCicA/640?wx_fmt=png&from=appmsg "")  
  
IBM Backup， Recovery， and Media Services for the i 平台中存在一个严重安全漏洞，可能允许攻击者获得提升的权限，并通过对主机作系统的组件级访问权限执行恶意代码。  
  
该漏洞被跟踪为 CVE-2025-33108，源于 BRMS 程序进行的不合格库调用，CVSS 基本分数为 8.5，表明严重性较高。  
  
该安全漏洞会影响 IBM i 版本 7.5 和 7.4，可能会使运行这些系统的组织面临权限提升攻击。  
  
根据 IBM 于 2025 年 6 月 13 日发布的安全公告，该漏洞可能使具有编译或程序恢复能力的用户能够通过用户控制的代码执行来利用系统。  
  
IBM 备份服务权限提升  
  
该漏洞分类为 CWE-250：以不必要的权限执行，并利用 BRMS 架构中的不合格库调用弱点。  
  
攻击媒介需要具有高攻击复杂性、低权限且无用户交互的网络访问，如 CVSS 向量 （CVSS：3.1/AV：N/AC：H/PR：L/UI：N/S：C/C：H/I：H/A：H） 所示。  
  
成功利用此漏洞的恶意行为者可能导致用户控制的代码以提升的系统权限执行，从而可能危及受影响系统的机密性、完整性和可用性。  
  
CVSS 向量中的范围更改指示器表明，该漏洞可能会影响易受攻击组件本身以外的资源。  
  
此缺陷的技术性质在于 BRMS 程序如何在没有适当资格的情况下进行库调用，从而为攻击者注入恶意代码创造了机会，这些代码以比预期更高的权限运行。  
  
这种类型的漏洞在备份和恢复系统通常具有大量系统访问权限的企业环境中尤其令人担忧。  
  
成功利用此漏洞可为攻击者提供对关键业务数据和系统功能的广泛访问权限。  
<table><tbody><tr style="box-sizing: border-box;background-color: rgb(240, 240, 240);"><td data-colwidth="156" style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><strong msttexthash="14330498" msthash="73" style="box-sizing: border-box;font-weight: bold;"><span leaf=""><span textstyle="" style="font-size: 15px;">风险因素</span></span></strong></td><td style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><strong msttexthash="3259074" msthash="74" style="box-sizing: border-box;font-weight: bold;"><span leaf=""><span textstyle="" style="font-size: 15px;">详</span></span></strong></td></tr><tr style="box-sizing: border-box;"><td data-colwidth="156" style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">受影响的产品</span></span></section></td><td style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">IBM 备份、恢复和媒体服务 i 版 （BRMS） 版本 7.5 和 7.4</span></span></section></td></tr><tr style="box-sizing: border-box;background-color: rgb(240, 240, 240);"><td data-colwidth="156" style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">冲击</span></span></section></td><td style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">权限提升</span></span></section></td></tr><tr style="box-sizing: border-box;"><td data-colwidth="156" style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">利用先决条件</span></span></section></td><td style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">– 编译或恢复程序的用户能力 - 网络访问 （AV：N） 和低权限 （PR：L）</span></span></section></td></tr><tr style="box-sizing: border-box;background-color: rgb(240, 240, 240);"><td data-colwidth="156" style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">CVSS 3.1 分数</span></span></section></td><td style="box-sizing: border-box;padding: 2px 8px;border: 1px solid rgba(0, 0, 0, 0);word-break: break-word;"><section style="margin-top: 8px;margin-bottom: 8px;"><span leaf=""><span textstyle="" style="font-size: 15px;">8.5 （高）</span></span></section></td></tr></tbody></table>  
缓解措施  
  
IBM 已发布 Program Temporary Fixes （PTF） 以解决受影响版本中的漏洞。  
  
运行 IBM i 发行版 7.5 的组织应应用 PTF SJ05907，而使用 Release 7.4 的组织需要安装 PTF SJ05906。这两个修复程序都可以通过 IBM 的支持门户网站和 Fix Central 获得。  
  
这些补丁专门针对 5770-BR1 产品代码，解决了导致权限提升的不合格库调用问题。  
  
系统管理员可以使用提供的链接从 IBM 的 MySupport 门户下载相应的 PTF，或通过集中式 Fix Central 存储库访问它。  
  
值得注意的是，IBM 已表示没有针对此漏洞的解决方法或缓解措施，因此应用安全补丁是唯一可行的解决方案。  
  
这强调了立即为受影响的系统部署补丁的极端重要性。  
  
组织应优先考虑立即部署可用的 PTF，尤其是在备份系统可通过网络访问或多个用户具有编译或恢复权限的环境中。  
  
原文来自: cybersecuritynews.com  
  
原文链接:   
https://cybersecuritynews.com/ibm-backup-services-vulnerability/  
  
欢迎收藏并分享朋友圈，让五邑人网络更安全  
  
![](https://mmbiz.qpic.cn/mmbiz_jpg/1N39PtINn8tD9ic928O6vIrMg4fuib48e1TsRj9K9Cz7RZBD2jjVZcKm1N4QrZ4bwBKZic5crOdItOcdDicPd3yBSg/640?wx_fmt=jpeg "")  
  
欢迎扫描关注我们，及时了解最新安全动态、学习最潮流的安全姿势！  
  
推荐文章  
  
1  
  
[新永恒之蓝？微软SMBv3高危漏洞（CVE-2020-0796）分析复现](http://mp.weixin.qq.com/s?__biz=MzUyMzczNzUyNQ==&mid=2247488913&idx=1&sn=acbf595a4a80dcaba647c7a32fe5e06b&chksm=fa39554bcd4edc5dc90019f33746404ab7593dd9d90109b1076a4a73f2be0cb6fa90e8743b50&scene=21#wechat_redirect)  
  
  
2  
  
[重大漏洞预警：ubuntu最新版本存在本地提权漏洞（已有EXP）　](http://mp.weixin.qq.com/s?__biz=MzUyMzczNzUyNQ==&mid=2247483652&idx=1&sn=b2f2ec90db499e23cfa252e9ee743265&chksm=fa3941decd4ec8c83a268c3480c354a621d515262bcbb5f35e1a2dde8c828bdc7b9011cb5072&scene=21#wechat_redirect)  
  
  
  
  
  
