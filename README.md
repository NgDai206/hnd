# Shadowrocket: 2024-01-05 18:18:16
[General]
bypass-system = true
skip-proxy = 192.168.0.0/16,10.0.0.0/8,172.16.0.0/12,localhost,*.local,captive.apple.com,https://dns.nextdns.io/593a65
tun-excluded-routes = 10.0.0.0/8, 100.64.0.0/10, 127.0.0.0/8, 169.254.0.0/16, 172.16.0.0/12, 192.0.0.0/24, 192.0.2.0/24, 192.88.99.0/24, 192.168.0.0/16, 198.51.100.0/24, 203.0.113.0/24, 224.0.0.0/4, 255.255.255.255/32, 239.255.255.250/32
dns-server = system,https://dns.nextdns.io/593a65,1.5.2.9.17,4.2.5.9
fallback-dns-server = system
ipv6 = false
prefer-ipv6 = false
dns-fallback-system = false
dns-direct-system = false
icmp-auto-reply = true
always-reject-url-rewrite = false
private-ip-answer = false
# direct domain fail to resolve use proxy rule
dns-direct-fallback-proxy = true
# The fallback behavior when UDP traffic matches a policy that doesn't support the UDP relay. Possible values: DIRECT, REJECT.
udp-policy-not-supported-behaviour = REJECT

[Rule]
RULE-SET,https://raw.githubusercontent.com/bigdargon/hostsVN/master/extensions/threat/surge-rule.conf,REJECT
DOMAIN-SET,ocsp2.apple.com,REJECT
# Block HTTP3/QUIC
# AND,((PROTOCOL,UDP),(DEST-PORT,443)),REJECT-NO-DROP
# Baidu/iqiyi
DOMAIN-SUFFIX,baidu.com,DIRECT
DOMAIN-SUFFIX,baidubcr.com,DIRECT
DOMAIN-SUFFIX,bdstatic.com,DIRECT
DOMAIN-SUFFIX,yunjiasu-cdn.net,DIRECT
# Alibaba
DOMAIN-SUFFIX,taobao.com,DIRECT
DOMAIN-SUFFIX,alicdn.com,DIRECT
# Accelerate most visited sites
DOMAIN,blzddist1-a.akamaihd.net,DIRECT
DOMAIN,cdn.angruo.com,DIRECT
DOMAIN,download.jetbrains.com,DIRECT
DOMAIN,file-igamecj.akamaized.net,DIRECT
DOMAIN,images-cn.ssl-images-amazon.com,DIRECT
DOMAIN,officecdn-microsoft-com.akamaized.net,DIRECT
DOMAIN,speedtest.macpaw.com,DIRECT
DOMAIN-SUFFIX,126.net,DIRECT
DOMAIN-SUFFIX,127.net,DIRECT
DOMAIN-SUFFIX,163.com,DIRECT
DOMAIN-SUFFIX,163yun.com,DIRECT
DOMAIN-SUFFIX,21cn.com,DIRECT
DOMAIN-SUFFIX,343480.com,DIRECT
DOMAIN-SUFFIX,360buyimg.com,DIRECT
DOMAIN-SUFFIX,360in.com,DIRECT
DOMAIN-SUFFIX,51ym.me,DIRECT
DOMAIN-SUFFIX,71.am.com,DIRECT
DOMAIN-SUFFIX,8686c.com,DIRECT
DOMAIN-SUFFIX,abchina.com,DIRECT
DOMAIN-SUFFIX,accuweather.com,DIRECT
DOMAIN-SUFFIX,acgvideo.com,DIRECT
DOMAIN-SUFFIX,acm.org,DIRECT
DOMAIN-SUFFIX,acs.org,DIRECT
DOMAIN-SUFFIX,aicoinstorge.com,DIRECT
DOMAIN-SUFFIX,aip.org,DIRECT
DOMAIN-SUFFIX,air-matters.com,DIRECT
DOMAIN-SUFFIX,air-matters.io,DIRECT
DOMAIN-SUFFIX,aixifan.com,DIRECT
DOMAIN-SUFFIX,akadns.net,DIRECT
DOMAIN-SUFFIX,alibaba.com,DIRECT
DOMAIN-SUFFIX,alikunlun.com,DIRECT
DOMAIN-SUFFIX,alipay.com,DIRECT
DOMAIN-SUFFIX,amap.com,DIRECT
DOMAIN-SUFFIX,amd.com,DIRECT
DOMAIN-SUFFIX,ams.org,DIRECT
DOMAIN-SUFFIX,animebytes.tv,DIRECT
DOMAIN-SUFFIX,annualreviews.org,DIRECT
DOMAIN-SUFFIX,aps.org,DIRECT
DOMAIN-SUFFIX,ascelibrary.org,DIRECT
DOMAIN-SUFFIX,asm.org,DIRECT
DOMAIN-SUFFIX,asme.org,DIRECT
DOMAIN-SUFFIX,astm.org,DIRECT
DOMAIN-SUFFIX,autonavi.com,DIRECT
DOMAIN-SUFFIX,awesome-hd.me,DIRECT
DOMAIN-SUFFIX,b612.net,DIRECT
DOMAIN-SUFFIX,baduziyuan.com,DIRECT
DOMAIN-SUFFIX,battle.net,DIRECT
DOMAIN-SUFFIX,bdatu.com,DIRECT
DOMAIN-SUFFIX,beitaichufang.com,DIRECT
DOMAIN-SUFFIX,biliapi.com,DIRECT
DOMAIN-SUFFIX,biliapi.net,DIRECT
DOMAIN-SUFFIX,bilibili.com,DIRECT
DOMAIN-SUFFIX,bilibili.tv,DIRECT
DOMAIN-SUFFIX,bjango.com,DIRECT
DOMAIN-SUFFIX,blizzard.com,DIRECT
DOMAIN-SUFFIX,bmj.com,DIRECT
DOMAIN-SUFFIX,booking.com,DIRECT
DOMAIN-SUFFIX,broadcasthe.net,DIRECT
DOMAIN-SUFFIX,bstatic.com,DIRECT
DOMAIN-SUFFIX,cailianpress.com,DIRECT
DOMAIN-SUFFIX,cambridge.org,DIRECT
DOMAIN-SUFFIX,camera360.com,DIRECT
DOMAIN-SUFFIX,cas.org,DIRECT
DOMAIN-SUFFIX,ccgslb.com,DIRECT
DOMAIN-SUFFIX,ccgslb.net,DIRECT
DOMAIN-SUFFIX,cctv.com,DIRECT
DOMAIN-SUFFIX,cctvpic.com,DIRECT
DOMAIN-SUFFIX,chdbits.co,DIRECT
DOMAIN-SUFFIX,chinanetcenter.com,DIRECT
DOMAIN-SUFFIX,chinaso.com,DIRECT
DOMAIN-SUFFIX,chua.pro,DIRECT
DOMAIN-SUFFIX,chuimg.com,DIRECT
DOMAIN-SUFFIX,chunyu.mobi,DIRECT
DOMAIN-SUFFIX,chushou.tv,DIRECT
DOMAIN-SUFFIX,clarivate.com,DIRECT
DOMAIN-SUFFIX,classix-unlimited.co.uk,DIRECT
DOMAIN-SUFFIX,cmbchina.com,DIRECT
DOMAIN-SUFFIX,cmbimg.com,DIRECT
DOMAIN-SUFFIX,cn,DIRECT
DOMAIN-SUFFIX,com-hs-hkdy.com,DIRECT
DOMAIN-SUFFIX,ctrip.com,DIRECT
DOMAIN-SUFFIX,czybjz.com,DIRECT
DOMAIN-SUFFIX,dandanzan.com,DIRECT
DOMAIN-SUFFIX,dfcfw.com,DIRECT
DOMAIN-SUFFIX,didialift.com,DIRECT
DOMAIN-SUFFIX,didiglobal.com,DIRECT
DOMAIN-SUFFIX,dingtalk.com,DIRECT
DOMAIN-SUFFIX,docschina.org,DIRECT
DOMAIN-SUFFIX,douban.com,DIRECT
DOMAIN-SUFFIX,doubanio.com,DIRECT
DOMAIN-SUFFIX,douyu.com,DIRECT
DOMAIN-SUFFIX,duokan.com,DIRECT
DOMAIN-SUFFIX,dxycdn.com,DIRECT
DOMAIN-SUFFIX,dytt8.net,DIRECT
DOMAIN-SUFFIX,eastmoney.com,DIRECT
DOMAIN-SUFFIX,ebscohost.com,DIRECT
DOMAIN-SUFFIX,emerald.com,DIRECT
DOMAIN-SUFFIX,empornium.me,DIRECT
DOMAIN-SUFFIX,engineeringvillage.com,DIRECT
DOMAIN-SUFFIX,eudic.net,DIRECT
DOMAIN-SUFFIX,feiliao.com,DIRECT
DOMAIN-SUFFIX,feng.com,DIRECT
DOMAIN-SUFFIX,fengkongcloud.com,DIRECT
DOMAIN-SUFFIX,fjhps.com,DIRECT
DOMAIN-SUFFIX,frdic.com,DIRECT
DOMAIN-SUFFIX,futu5.com,DIRECT
DOMAIN-SUFFIX,futunn.com,DIRECT
DOMAIN-SUFFIX,gandi.net,DIRECT
DOMAIN-SUFFIX,gazellegames.net,DIRECT
DOMAIN-SUFFIX,geilicdn.com,DIRECT
DOMAIN-SUFFIX,getpricetag.com,DIRECT
DOMAIN-SUFFIX,gifshow.com,DIRECT
DOMAIN-SUFFIX,godic.net,DIRECT
DOMAIN-SUFFIX,gtimg.com,DIRECT
DOMAIN-SUFFIX,hdbits.org,DIRECT
DOMAIN-SUFFIX,hdchina.org,DIRECT
DOMAIN-SUFFIX,hdhome.org,DIRECT
DOMAIN-SUFFIX,hdsky.me,DIRECT
DOMAIN-SUFFIX,hdslb.com,DIRECT
DOMAIN-SUFFIX,hicloud.com,DIRECT
DOMAIN-SUFFIX,hitv.com,DIRECT
DOMAIN-SUFFIX,hongxiu.com,DIRECT
DOMAIN-SUFFIX,hostbuf.com,DIRECT
DOMAIN-SUFFIX,huxiucdn.com,DIRECT
DOMAIN-SUFFIX,huya.com,DIRECT
DOMAIN-SUFFIX,icetorrent.org,DIRECT
DOMAIN-SUFFIX,icevirtuallibrary.com,DIRECT
DOMAIN-SUFFIX,iciba.com,DIRECT
DOMAIN-SUFFIX,idqqimg.com,DIRECT
DOMAIN-SUFFIX,ieee.org,DIRECT
DOMAIN-SUFFIX,iesdouyin.com,DIRECT
DOMAIN-SUFFIX,igamecj.com,DIRECT
DOMAIN-SUFFIX,imf.org,DIRECT
DOMAIN-SUFFIX,infinitynewtab.com,DIRECT
DOMAIN-SUFFIX,iop.org,DIRECT
DOMAIN-SUFFIX,ip-cdn.com,DIRECT
DOMAIN-SUFFIX,ip.la,DIRECT
DOMAIN-SUFFIX,ipip.net,DIRECT
DOMAIN-SUFFIX,ipv6-test.com,DIRECT
DOMAIN-SUFFIX,iqiyi.com,DIRECT
DOMAIN-SUFFIX,iqiyipic.com,DIRECT
DOMAIN-SUFFIX,ithome.com,DIRECT
DOMAIN-SUFFIX,jamanetwork.com,DIRECT
DOMAIN-SUFFIX,java.com,DIRECT
DOMAIN-SUFFIX,jd.com,DIRECT
DOMAIN-SUFFIX,jd.hk,DIRECT
DOMAIN-SUFFIX,jdpay.com,DIRECT
DOMAIN-SUFFIX,jhu.edu,DIRECT
DOMAIN-SUFFIX,jidian.im,DIRECT
DOMAIN-SUFFIX,jpopsuki.eu,DIRECT
DOMAIN-SUFFIX,jstor.org,DIRECT
DOMAIN-SUFFIX,jstucdn.com,DIRECT
DOMAIN-SUFFIX,kaiyanapp.com,DIRECT
DOMAIN-SUFFIX,karger.com,DIRECT
DOMAIN-SUFFIX,kaspersky-labs.com,DIRECT
DOMAIN-SUFFIX,keepcdn.com,DIRECT
DOMAIN-SUFFIX,keepfrds.com,DIRECT
DOMAIN-SUFFIX,kkmh.com,DIRECT
DOMAIN-SUFFIX,ksosoft.com,DIRECT
DOMAIN-SUFFIX,kuyunbo.club,DIRECT
DOMAIN-SUFFIX,libguides.com,DIRECT
DOMAIN-SUFFIX,livechina.com,DIRECT
DOMAIN-SUFFIX,lofter.com,DIRECT
DOMAIN-SUFFIX,loli.net,DIRECT
DOMAIN-SUFFIX,luojilab.com,DIRECT
DOMAIN-SUFFIX,m-team.cc,DIRECT
DOMAIN-SUFFIX,madsrevolution.net,DIRECT
DOMAIN-SUFFIX,maoyan.com,DIRECT
DOMAIN-SUFFIX,maoyun.tv,DIRECT
DOMAIN-SUFFIX,meipai.com,DIRECT
DOMAIN-SUFFIX,meitu.com,DIRECT
DOMAIN-SUFFIX,meituan.com,DIRECT
DOMAIN-SUFFIX,meituan.net,DIRECT
DOMAIN-SUFFIX,meitudata.com,DIRECT
DOMAIN-SUFFIX,meitustat.com,DIRECT
DOMAIN-SUFFIX,meixincdn.com,DIRECT
DOMAIN-SUFFIX,mgtv.com,DIRECT
DOMAIN-SUFFIX,mi-img.com,DIRECT
DOMAIN-SUFFIX,microsoft.com,DIRECT
DOMAIN-SUFFIX,miui.com,DIRECT
DOMAIN-SUFFIX,miwifi.com,DIRECT
DOMAIN-SUFFIX,mobike.com,DIRECT
DOMAIN-SUFFIX,moke.com,DIRECT
DOMAIN-SUFFIX,morethan.tv,DIRECT
DOMAIN-SUFFIX,mpg.de,DIRECT
DOMAIN-SUFFIX,msecnd.net,DIRECT
DOMAIN-SUFFIX,mubu.com,DIRECT
DOMAIN-SUFFIX,mxhichina.com,DIRECT
DOMAIN-SUFFIX,myanonamouse.net,DIRECT
DOMAIN-SUFFIX,myapp.com,DIRECT
DOMAIN-SUFFIX,myilibrary.com,DIRECT
DOMAIN-SUFFIX,myqcloud.com,DIRECT
DOMAIN-SUFFIX,myzaker.com,DIRECT
DOMAIN-SUFFIX,nanyangpt.com,DIRECT
DOMAIN-SUFFIX,nature.com,DIRECT
DOMAIN-SUFFIX,ncore.cc,DIRECT
DOMAIN-SUFFIX,netease.com,DIRECT
DOMAIN-SUFFIX,netspeedtestmaster.com,DIRECT
DOMAIN-SUFFIX,nim-lang-cn.org,DIRECT
DOMAIN-SUFFIX,nvidia.com,DIRECT
DOMAIN-SUFFIX,oecd-ilibrary.org,DIRECT
DOMAIN-SUFFIX,office365.com,DIRECT
DOMAIN-SUFFIX,open.cd,DIRECT
DOMAIN-SUFFIX,oracle.com,DIRECT
DOMAIN-SUFFIX,osapublishing.org,DIRECT
DOMAIN-SUFFIX,oup.com,DIRECT
DOMAIN-SUFFIX,ourbits.club,DIRECT
DOMAIN-SUFFIX,ourdvs.com,DIRECT
DOMAIN-SUFFIX,outlook.com,DIRECT
DOMAIN-SUFFIX,ovid.com,DIRECT
DOMAIN-SUFFIX,oxfordartonline.com,DIRECT
DOMAIN-SUFFIX,oxfordbibliographies.com,DIRECT
DOMAIN-SUFFIX,oxfordmusiconline.com,DIRECT
DOMAIN-SUFFIX,passthepopcorn.me,DIRECT
DOMAIN-SUFFIX,paypal.com,DIRECT
DOMAIN-SUFFIX,paypalobjects.com,DIRECT
DOMAIN-SUFFIX,pnas.org,DIRECT
DOMAIN-SUFFIX,privatehd.to,DIRECT
DOMAIN-SUFFIX,proquest.com,DIRECT
DOMAIN-SUFFIX,pstatp.com,DIRECT
DOMAIN-SUFFIX,pterclub.com,DIRECT
DOMAIN-SUFFIX,qdaily.com,DIRECT
DOMAIN-SUFFIX,qhimg.com,DIRECT
DOMAIN-SUFFIX,qhres.com,DIRECT
DOMAIN-SUFFIX,qidian.com,DIRECT
DOMAIN-SUFFIX,qq.com,DIRECT
DOMAIN-SUFFIX,wechat.com,DIRECT
DOMAIN-SUFFIX,dns.pub,DIRECT
DOMAIN-SUFFIX,doh.pub,DIRECT
DOMAIN-SUFFIX,qyer.com,DIRECT
DOMAIN-SUFFIX,qyerstatic.com,DIRECT
DOMAIN-SUFFIX,raychase.net,DIRECT
DOMAIN-SUFFIX,redacted.ch,DIRECT
DOMAIN-SUFFIX,ronghub.com,DIRECT
DOMAIN-SUFFIX,rsc.org,DIRECT
DOMAIN-SUFFIX,ruguoapp.com,DIRECT
DOMAIN-SUFFIX,s-microsoft.com,DIRECT
DOMAIN-SUFFIX,s-reader.com,DIRECT
DOMAIN-SUFFIX,sagepub.com,DIRECT
DOMAIN-SUFFIX,sankuai.com,DIRECT
DOMAIN-SUFFIX,sciencedirect.com,DIRECT
DOMAIN-SUFFIX,sciencemag.org,DIRECT
DOMAIN-SUFFIX,scomper.me,DIRECT
DOMAIN-SUFFIX,scopus.com,DIRECT
DOMAIN-SUFFIX,seafile.com,DIRECT
DOMAIN-SUFFIX,servicewechat.com,DIRECT
DOMAIN-SUFFIX,siam.org,DIRECT
DOMAIN-SUFFIX,sina.com,DIRECT
DOMAIN-SUFFIX,sm.ms,DIRECT
DOMAIN-SUFFIX,smzdm.com,DIRECT
DOMAIN-SUFFIX,snapdrop.net,DIRECT
DOMAIN-SUFFIX,snssdk.com,DIRECT
DOMAIN-SUFFIX,snwx.com,DIRECT
DOMAIN-SUFFIX,sogo.com,DIRECT
DOMAIN-SUFFIX,sogou.com,DIRECT
DOMAIN-SUFFIX,sogoucdn.com,DIRECT
DOMAIN-SUFFIX,sohu-inc.com,DIRECT
DOMAIN-SUFFIX,sohu.com,DIRECT
DOMAIN-SUFFIX,sohucs.com,DIRECT
DOMAIN-SUFFIX,soku.com,DIRECT
DOMAIN-SUFFIX,spiedigitallibrary.org,DIRECT
DOMAIN-SUFFIX,springer.com,DIRECT
DOMAIN-SUFFIX,springerlink.com,DIRECT
DOMAIN-SUFFIX,springsunday.net,DIRECT
DOMAIN-SUFFIX,sspai.com,DIRECT
DOMAIN-SUFFIX,staticdn.net,DIRECT
DOMAIN-SUFFIX,steam-chat.com,DIRECT
DOMAIN-SUFFIX,steamcdn-a.akamaihd.net,DIRECT
DOMAIN-SUFFIX,steamcontent.com,DIRECT
DOMAIN-SUFFIX,steamgames.com,DIRECT
DOMAIN-SUFFIX,steampowered.com,DIRECT
DOMAIN-SUFFIX,steamstat.us,DIRECT
DOMAIN-SUFFIX,steamstatic.com,DIRECT
DOMAIN-SUFFIX,steamusercontent.com,DIRECT
DOMAIN-SUFFIX,takungpao.com,DIRECT
DOMAIN-SUFFIX,tandfonline.com,DIRECT
DOMAIN-SUFFIX,teamviewer.com,DIRECT
DOMAIN-SUFFIX,tencent-cloud.net,DIRECT
DOMAIN-SUFFIX,tencent.com,DIRECT
DOMAIN-SUFFIX,tenpay.com,DIRECT
DOMAIN-SUFFIX,test-ipv6.com,DIRECT
DOMAIN-SUFFIX,tianyancha.com,DIRECT
DOMAIN-SUFFIX,tjupt.org,DIRECT
DOMAIN-SUFFIX,tmall.com,DIRECT
DOMAIN-SUFFIX,tmall.hk,DIRECT
DOMAIN-SUFFIX,totheglory.im,DIRECT
DOMAIN-SUFFIX,toutiao.com,DIRECT
DOMAIN-SUFFIX,udache.com,DIRECT
DOMAIN-SUFFIX,udacity.com,DIRECT
DOMAIN-SUFFIX,un.org,DIRECT
DOMAIN-SUFFIX,uni-bielefeld.de,DIRECT
DOMAIN-SUFFIX,uning.com,DIRECT
DOMAIN-SUFFIX,v-56.com,DIRECT
DOMAIN-SUFFIX,visualstudio.com,DIRECT
DOMAIN-SUFFIX,vmware.com,DIRECT
DOMAIN-SUFFIX,wangsu.com,DIRECT
DOMAIN-SUFFIX,weather.com,DIRECT
DOMAIN-SUFFIX,webofknowledge.com,DIRECT
DOMAIN-SUFFIX,wechat.com,DIRECT
DOMAIN-SUFFIX,weibo.com,DIRECT
DOMAIN-SUFFIX,weibocdn.com,DIRECT
DOMAIN-SUFFIX,weico.cc,DIRECT
DOMAIN-SUFFIX,weidian.com,DIRECT
DOMAIN-SUFFIX,westlaw.com,DIRECT
DOMAIN-SUFFIX,whatismyip.com,DIRECT
DOMAIN-SUFFIX,wiley.com,DIRECT
DOMAIN-SUFFIX,windows.com,DIRECT
DOMAIN-SUFFIX,windowsupdate.com,DIRECT
DOMAIN-SUFFIX,worldbank.org,DIRECT
DOMAIN-SUFFIX,worldscientific.com,DIRECT
DOMAIN-SUFFIX,xiachufang.com,DIRECT
DOMAIN-SUFFIX,xiami.com,DIRECT
DOMAIN-SUFFIX,xiami.net,DIRECT
DOMAIN-SUFFIX,xiaomi.com,DIRECT
DOMAIN-SUFFIX,xiaohongshu.com,DIRECT
DOMAIN-SUFFIX,xhscdn.com,DIRECT
DOMAIN-SUFFIX,ximalaya.com,DIRECT
DOMAIN-SUFFIX,xinhuanet.com,DIRECT
DOMAIN-SUFFIX,xmcdn.com,DIRECT
DOMAIN-SUFFIX,yangkeduo.com,DIRECT
DOMAIN-SUFFIX,ydstatic.com,DIRECT
DOMAIN-SUFFIX,youku.com,DIRECT
DOMAIN-SUFFIX,zhangzishi.cc,DIRECT
DOMAIN-SUFFIX,zhihu.com,DIRECT
DOMAIN-SUFFIX,zhimg.com,DIRECT
DOMAIN-SUFFIX,zhuihd.com,DIRECT
DOMAIN-SUFFIX,zimuzu.io,DIRECT
DOMAIN-SUFFIX,zimuzu.tv,DIRECT
DOMAIN-SUFFIX,zmz2019.com,DIRECT
DOMAIN-SUFFIX,zmzapi.com,DIRECT
DOMAIN-SUFFIX,zmzapi.net,DIRECT
DOMAIN-SUFFIX,zmzfile.com,DIRECT
DOMAIN-SUFFIX,manmanbuy.com,DIRECT
# Remove these lines below if you don't have trouble accessing Apple resources
DOMAIN,www-cdn.icloud.com.akadns.net,DIRECT
DOMAIN-SUFFIX,aaplimg.com,DIRECT
DOMAIN-SUFFIX,apple-cloudkit.com,DIRECT
DOMAIN-SUFFIX,apple.co,DIRECT
DOMAIN-SUFFIX,apple.com,DIRECT
DOMAIN-SUFFIX,apple.news,DIRECT
DOMAIN-SUFFIX,apple.com.cn,DIRECT
DOMAIN-SUFFIX,appstore.com,DIRECT
DOMAIN-SUFFIX,cdn-apple.com,DIRECT
DOMAIN-SUFFIX,crashlytics.com,DIRECT
DOMAIN-SUFFIX,icloud-content.com,DIRECT
DOMAIN-SUFFIX,icloud.com,DIRECT
DOMAIN-SUFFIX,icloud.com.cn,DIRECT
DOMAIN-SUFFIX,me.com,DIRECT
DOMAIN-SUFFIX,mzstatic.com,DIRECT
# LINE
DOMAIN-SUFFIX,scdn.co,PROXY
DOMAIN-SUFFIX,line.naver.jp,PROXY
DOMAIN-SUFFIX,line.me,PROXY
DOMAIN-SUFFIX,line-apps.com,PROXY
DOMAIN-SUFFIX,line-cdn.net,PROXY
DOMAIN-SUFFIX,line-scdn.net,PROXY
USER-AGENT,Line*,PROXY
# Google
DOMAIN-KEYWORD,blogspot,PROXY
DOMAIN-KEYWORD,google,PROXY
DOMAIN-SUFFIX,abc.xyz,PROXY
DOMAIN-SUFFIX,admin.recaptcha.net,PROXY
DOMAIN-SUFFIX,ampproject.org,PROXY
DOMAIN-SUFFIX,android.com,PROXY
DOMAIN-SUFFIX,androidify.com,PROXY
DOMAIN-SUFFIX,appspot.com,PROXY
DOMAIN-SUFFIX,autodraw.com,PROXY
DOMAIN-SUFFIX,blogger.com,PROXY
DOMAIN-SUFFIX,capitalg.com,PROXY
DOMAIN-SUFFIX,certificate-transparency.org,PROXY
DOMAIN-SUFFIX,chrome.com,PROXY
DOMAIN-SUFFIX,chromeexperiments.com,PROXY
DOMAIN-SUFFIX,chromestatus.com,PROXY
DOMAIN-SUFFIX,chromium.org,PROXY
DOMAIN-SUFFIX,creativelab5.com,PROXY
DOMAIN-SUFFIX,debug.com,PROXY
DOMAIN-SUFFIX,deepmind.com,PROXY
DOMAIN-SUFFIX,dialogflow.com,PROXY
DOMAIN-SUFFIX,firebaseio.com,PROXY
DOMAIN-SUFFIX,getmdl.io,PROXY
DOMAIN-SUFFIX,getoutline.org,PROXY
DOMAIN-SUFFIX,ggpht.com,PROXY
DOMAIN-SUFFIX,gmail.com,PROXY
DOMAIN-SUFFIX,gmodules.com,PROXY
DOMAIN-SUFFIX,godoc.org,PROXY
DOMAIN-SUFFIX,golang.org,PROXY
DOMAIN-SUFFIX,gstatic.com,PROXY
DOMAIN-SUFFIX,gv.com,PROXY
DOMAIN-SUFFIX,gvt0.com,PROXY
DOMAIN-SUFFIX,gvt1.com,PROXY
DOMAIN-SUFFIX,gvt3.com,PROXY
DOMAIN-SUFFIX,gwtproject.org,PROXY
DOMAIN-SUFFIX,itasoftware.com,PROXY
DOMAIN-SUFFIX,madewithcode.com,PROXY
DOMAIN-SUFFIX,material.io,PROXY
DOMAIN-SUFFIX,polymer-project.org,PROXY
DOMAIN-SUFFIX,recaptcha.net,PROXY
DOMAIN-SUFFIX,shattered.io,PROXY
DOMAIN-SUFFIX,synergyse.com,PROXY
DOMAIN-SUFFIX,telephony.goog,PROXY
DOMAIN-SUFFIX,tensorflow.org,PROXY
DOMAIN-SUFFIX,tfhub.dev,PROXY
DOMAIN-SUFFIX,tiltbrush.com,PROXY
DOMAIN-SUFFIX,waveprotocol.org,PROXY
DOMAIN-SUFFIX,waymo.com,PROXY
DOMAIN-SUFFIX,webmproject.org,PROXY
DOMAIN-SUFFIX,webrtc.org,PROXY
DOMAIN-SUFFIX,whatbrowser.org,PROXY
DOMAIN-SUFFIX,widevine.com,PROXY
DOMAIN-SUFFIX,x.company,PROXY
DOMAIN-SUFFIX,xn--ngstr-lra8j.com,PROXY
DOMAIN-SUFFIX,youtu.be,PROXY
DOMAIN-SUFFIX,yt.be,PROXY
DOMAIN-SUFFIX,ytimg.com,PROXY
# Clubhouse
DOMAIN-SUFFIX,clubhouseapi.com,PROXY
DOMAIN-SUFFIX,clubhouse.pubnub.com,PROXY
DOMAIN-SUFFIX,joinclubhouse.com,PROXY
DOMAIN-SUFFIX,ap3.agora.io,PROXY
# Top blocked sites
DOMAIN-KEYWORD,aka,PROXY
DOMAIN-KEYWORD,facebook,PROXY
DOMAIN-KEYWORD,youtube,PROXY
DOMAIN-KEYWORD,twitter,PROXY
DOMAIN-KEYWORD,instagram,PROXY
DOMAIN-KEYWORD,gmail,PROXY
DOMAIN-KEYWORD,pixiv,PROXY
DOMAIN-SUFFIX,fb.com,PROXY
DOMAIN-SUFFIX,meta.com,PROXY
DOMAIN-SUFFIX,twimg.com,PROXY
DOMAIN-SUFFIX,t.co,PROXY
DOMAIN-SUFFIX,kenengba.com,PROXY
DOMAIN-SUFFIX,akamai.net,PROXY
DOMAIN-SUFFIX,whatsapp.net,PROXY
DOMAIN-SUFFIX,whatsapp.com,PROXY
DOMAIN-SUFFIX,snapchat.com,PROXY
DOMAIN-SUFFIX,amazonaws.com,PROXY
DOMAIN-SUFFIX,angularjs.org,PROXY
DOMAIN-SUFFIX,akamaihd.net,PROXY
DOMAIN-SUFFIX,amazon.com,PROXY
DOMAIN-SUFFIX,bit.ly,PROXY
DOMAIN-SUFFIX,bitbucket.org,PROXY
DOMAIN-SUFFIX,blog.com,PROXY
DOMAIN-SUFFIX,blogcdn.com,PROXY
DOMAIN-SUFFIX,blogsmithmedia.com,PROXY
DOMAIN-SUFFIX,box.net,PROXY
DOMAIN-SUFFIX,bloomberg.com,PROXY
DOMAIN-SUFFIX,cl.ly,PROXY
DOMAIN-SUFFIX,cloudfront.net,PROXY
DOMAIN-SUFFIX,cloudflare.com,PROXY
DOMAIN-SUFFIX,cocoapods.org,PROXY
DOMAIN-SUFFIX,dribbble.com,PROXY
DOMAIN-SUFFIX,dropbox.com,PROXY
DOMAIN-SUFFIX,dropboxstatic.com,PROXY
DOMAIN-SUFFIX,dropboxusercontent.com,PROXY
DOMAIN-SUFFIX,docker.com,PROXY
DOMAIN-SUFFIX,duckduckgo.com,PROXY
DOMAIN-SUFFIX,digicert.com,PROXY
DOMAIN-SUFFIX,dnsimple.com,PROXY
DOMAIN-SUFFIX,edgecastcdn.net,PROXY
DOMAIN-SUFFIX,engadget.com,PROXY
DOMAIN-SUFFIX,eurekavpt.com,PROXY
DOMAIN-SUFFIX,fb.me,PROXY
DOMAIN-SUFFIX,fbcdn.net,PROXY
DOMAIN-SUFFIX,fc2.com,PROXY
DOMAIN-SUFFIX,feedburner.com,PROXY
DOMAIN-SUFFIX,fabric.io,PROXY
DOMAIN-SUFFIX,flickr.com,PROXY
DOMAIN-SUFFIX,fastly.net,PROXY
DOMAIN-SUFFIX,github.com,PROXY
DOMAIN-SUFFIX,github.io,PROXY
DOMAIN-SUFFIX,githubusercontent.com,PROXY
DOMAIN-SUFFIX,goo.gl,PROXY
DOMAIN-SUFFIX,godaddy.com,PROXY
DOMAIN-SUFFIX,gravatar.com,PROXY
DOMAIN-SUFFIX,imageshack.us,PROXY
DOMAIN-SUFFIX,imgur.com,PROXY
DOMAIN-SUFFIX,jshint.com,PROXY
DOMAIN-SUFFIX,ift.tt,PROXY
DOMAIN-SUFFIX,j.mp,PROXY
DOMAIN-SUFFIX,kat.cr,PROXY
DOMAIN-SUFFIX,linode.com,PROXY
DOMAIN-SUFFIX,lithium.com,PROXY
DOMAIN-SUFFIX,megaupload.com,PROXY
DOMAIN-SUFFIX,mobile01.com,PROXY
DOMAIN-SUFFIX,modmyi.com,PROXY
DOMAIN-SUFFIX,nytimes.com,PROXY
DOMAIN-SUFFIX,name.com,PROXY
DOMAIN-SUFFIX,openvpn.net,PROXY
DOMAIN-SUFFIX,openwrt.org,PROXY
DOMAIN-SUFFIX,ow.ly,PROXY
DOMAIN-SUFFIX,pinboard.in,PROXY
DOMAIN-SUFFIX,ssl-images-amazon.com,PROXY
DOMAIN-SUFFIX,sstatic.net,PROXY
DOMAIN-SUFFIX,stackoverflow.com,PROXY
DOMAIN-SUFFIX,staticflickr.com,PROXY
DOMAIN-SUFFIX,squarespace.com,PROXY
DOMAIN-SUFFIX,symcd.com,PROXY
DOMAIN-SUFFIX,symcb.com,PROXY
DOMAIN-SUFFIX,symauth.com,PROXY
DOMAIN-SUFFIX,ubnt.com,PROXY
DOMAIN-SUFFIX,thepiratebay.org,PROXY
DOMAIN-SUFFIX,tumblr.com,PROXY
DOMAIN-SUFFIX,twitch.tv,PROXY
DOMAIN-SUFFIX,twitter.com,PROXY
DOMAIN-SUFFIX,wikipedia.com,PROXY
DOMAIN-SUFFIX,wikipedia.org,PROXY
DOMAIN-SUFFIX,wikimedia.org,PROXY
DOMAIN-SUFFIX,wordpress.com,PROXY
DOMAIN-SUFFIX,wsj.com,PROXY
DOMAIN-SUFFIX,wsj.net,PROXY
DOMAIN-SUFFIX,wp.com,PROXY
DOMAIN-SUFFIX,vimeo.com,PROXY
DOMAIN-SUFFIX,tapbots.com,PROXY
DOMAIN-SUFFIX,ykimg.com,DIRECT
DOMAIN-SUFFIX,medium.com,PROXY
DOMAIN-SUFFIX,fast.com,PROXY
DOMAIN-SUFFIX,nflxvideo.net,PROXY
DOMAIN-SUFFIX,linkedin.com,PROXY
DOMAIN-SUFFIX,licdn.com,PROXY
DOMAIN-SUFFIX,bing.com,PROXY
# SoundCloud
DOMAIN-SUFFIX,soundcloud.com,PROXY
DOMAIN-SUFFIX,sndcdn.com,PROXY
# Telegram
DOMAIN-SUFFIX,t.me,PROXY
DOMAIN-SUFFIX,tdesktop.com,PROXY
DOMAIN-SUFFIX,telegra.ph,PROXY
DOMAIN-SUFFIX,telegram.me,PROXY
DOMAIN-SUFFIX,telegram.org,PROXY
DOMAIN-SUFFIX,telesco.pe,PROXY
IP-CIDR,91.108.4.0/22,PROXY,no-resolve
IP-CIDR,91.108.8.0/22,PROXY,no-resolve
IP-CIDR,91.108.12.0/22,PROXY,no-resolve
IP-CIDR,91.108.16.0/22,PROXY,no-resolve
IP-CIDR,91.108.56.0/22,PROXY,no-resolve
IP-CIDR,109.239.140.0/24,PROXY,no-resolve
IP-CIDR,149.154.160.0/20,PROXY,no-resolve
IP-CIDR,2001:B28:F23D::/48,PROXY,no-resolve
IP-CIDR,2001:B28:F23F::/48,PROXY,no-resolve
IP-CIDR,2001:67C:4E8::/48,PROXY,no-resolve
# DNS Leak
DOMAIN-SUFFIX,dnsleaktest.com,PROXY
DOMAIN-SUFFIX,dnsleak.com,PROXY
DOMAIN-SUFFIX,expressvpn.com,PROXY
DOMAIN-SUFFIX,nordvpn.com,PROXY
DOMAIN-SUFFIX,surfshark.com,PROXY
DOMAIN-SUFFIX,ipleak.net,PROXY
DOMAIN-SUFFIX,perfect-privacy.com,PROXY
DOMAIN-SUFFIX,browserleaks.com,PROXY
DOMAIN-SUFFIX,browserleaks.org,PROXY
DOMAIN-SUFFIX,vpnunlimited.com,PROXY
DOMAIN-SUFFIX,whoer.net,PROXY
DOMAIN-SUFFIX,whrq.net,PROXY
# LAN
IP-CIDR,192.168.0.0/16,DIRECT
IP-CIDR,10.0.0.0/8,DIRECT
IP-CIDR,172.16.0.0/12,DIRECT
IP-CIDR,127.0.0.0/8,DIRECT
# China
GEOIP,CN,DIRECT
# Final
FINAL,PROXY

[Host]
localhost = 127.0.0.1

[URL Rewrite]
^https?://(www.)?g.cn https://www.google.com 302
^https?://(www.)?google.cn https://www.google.com 302

[Script]
spti = type=http-response,script-path=https://raw.githubusercontent.com/app2smile/rules/master/js/spotify-proto.js,pattern=^https:\/\/spclient\.wg\.spotify\.com\/(bootstrap\/v1\/bootstrap|user-customization-service\/v1\/customize)$,max-size=0,requires-body=true,binary-mode=true,timeout=10,script-update-interval=0,enable=true

[MITM]
ca-passphrase = Shadowrocket
ca-p12 = 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
enable = false
hostname = https://dns.nextdns.io/593a65
