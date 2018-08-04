> 图片效果

![](https://huanfan-1252958858.cos.ap-shanghai.myqcloud.com/2018/08/QQ%E5%9B%BE%E7%89%8720180804130958.jpg)

# 原版主题

> [https://www.haomwei.com/technology/maupassant.html](https://www.haomwei.com/technology/maupassant.html)

## 屠城hexo版
> github地址：
>
> [https://github.com/tufu9441/maupassant-hexo](https://github.com/tufu9441/maupassant-hexo)

> 相关配置介绍：
>
> [https://www.haomwei.com/technology/maupassant-hexo.html](https://www.haomwei.com/technology/maupassant-hexo.html)

> 效果地址：
>
> [https://www.haomwei.com/](https://www.haomwei.com/)

## 本优化版

> github地址：
>
> [https://github.com/iyohei/maupassant-hexo-hfanss](https://github.com/iyohei/maupassant-hexo-hfanss)

> 相关配置介绍：
>
> [https://www.hfanss.com/2018/Maupassant主题优化、屠城主题优化版.html](https://hfanss.com/2018/Maupassant%E4%B8%BB%E9%A2%98%E3%80%81%E5%B1%A0%E5%9F%8E%E4%B8%BB%E9%A2%98%E4%BC%98%E5%8C%96%E7%89%88.html)

> 效果地址：
>
> [https://www.hfanss.com/](https://www.hfanss.com/)

---
# 现版主题
## 主要优化点
- 增加强制https 开关
- 归档页集成分类、标签、全部文章
- 菜单栏置顶
- 侧边栏删除
- 增加底部栏
- 搜索移至顶部菜单栏
- 文章页添加统一版权声明
- 文章添加置顶、原创、转载标志
- 底部文件始终在浏览器最下方
- 底部文件集成 关于我、微信二维码、熊掌号、关于博主，关于本站，友情链接
- 底部文件集成备案号，百度云统计、github、码云、CSDN外链
- 分享使用bshare，集成更多分享
- config.yml一些常用属性都做了中文注释
- 集成百度主动推送插件
- 优化整体布局
- 优化移动端菜单单独配置

## 增加配置开关
```YAML


valine: ## https://valine.js.org        评论系统
  enable: false ## 是否开启valine评论系统
  appid:  ## LeanCloud App ID, pRBBL2JR4N7kLEGojrF0MsSs-gzGzoHsz
  appkey:  ##LeanCloud App Key, e.g. tjczHpDfhjYDSYddzymYK1JJ
  notify: false ## Mail notifier, see https://github.com/xCss/Valine/wiki/Valine-评论系统中的邮件提醒设置
  verify: true ## 启用评论校验功能
  placeholder: 　 ## 留言板预设内容
  visitor: true ## 1.2版本新增功能阅读统计，具体使用参考https://valine.js.org/visitor.html
  avatar: 'monsterid' ## 默认头像 参考 https://valine.js.org/avatar.html
  pageSize: 10 ## 每页显示评论条数
  guest_info: nick,mail,link ## 昵称，邮箱，网站
## 百度统计ID
baidu_analytics:  ## 百度统计ID id, e.g. 8006843039519956000
## 图片灯箱开关
fancybox: true ## 是否启用Fancybox图片灯箱效果,建议开启（效果为点击图片既放大）
##版权声明，加在每篇文章下方
banquan: 
  enable: true ##是否开启
  name: 幻凡ss
  note: 本文所有权归博主所有，转载请注明署名、出处！Thanks ##版权信息
## 强制https访问开关
https: true ## 是否开启强制https（不影响本地调试）,本开关说明：https网站能正常访问开启才有效，如www.baidu.com跳转到http://www.baidu.com，不自动跳到https开头的网址，而且https://www.baidu.com能正常访问才行
## 文章字数统计开关
wordcount: true ##文章字数统计
readtime: false ##文章阅读时长统计
## daovice在线聊天相关 官网：http://www.daovoice.io/
daovoice: false ## 页面右下角在线聊天
daovoice_app_id:  ## daovice  ID 如：22c081c3
##搜索相关,只能开启一项
self_search: true ## 页面jquery搜索，需安装插件,开启此搜索后，博客根目录的  url属性必须带有http://和https://
baidu_search: false ##百度搜索.开启百度搜索后，博客根目录的  url属性不能带有http://和https://,否则会导致搜索不到东西（原理：基于你的网站百度收录结果搜索，如果没有被百度收录，就不会有结果）
## 文章目录开关
toc_number: true ## 文章目录开关 使用方法：#一级目录  ##二级目录  。。。 以此类推
## 文章分享开关  使用bshare.js  官网：http://www.bshare.cn/、注册站长并输入网址  需替换post.pug  55行script
shareto: true ## 文章分享开关
## 文章捐赠按钮。赞赏按钮
donate:
  enable: false ## If you want to show the donate button after each post, please set the value to true and fill the following items according to your need. You can also enable donate button in a page by adding a "donate: true" item to the front-matter.
  github: https://github.com/hfanss ## GitHub URL, e.g. https://github.com/Kaiyuan/donate-page
  alipay_qr: /img/AL.png ## Path of Alipay QRcode image, e.g. /img/AliPayQR.png
  wechat_qr: /img/QQ.png## Path of Wechat QRcode image, e.g. /img/WeChatQR.png
  btc_qr: ## Path of Bitcoin QRcode image, e.g. /img/BTCQR.png
  btc_key: ## Bitcoin key, e.g. 1KuK5eK2BLsqpsFVXXSBG5wbSAwZVadt6L
  paypal_url: ## Paypal URL, e.g. https://paypal.me/tufu9441


## 微信相关信息
weixin:
    enable: true
    name: hyaini ##微信号码
    url:  https://huanfan-1252958858.cos.ap-shanghai.myqcloud.com/pic/302701117226241178.jpg ##微信个人二维码url       
## 微博相关信息
weibo:
    enable: true
    name: 幻凡ss ##微博名字
    url: https://weibo.com/0377k  ##微博外链  如：https://weibo.com/0377k
## QQ相关信息
qq:
    enable: true
    name: 2158798 ##QQ号码
    url: https://wpa.qq.com/msgrd?v=3&uin=2158798&site=qq&menu=yes ##网页QQ聊天的外链  如  https://wpa.qq.com/msgrd?v=3&uin=2158798&site=qq&menu=yes 
## email相关信息
email:
    enable: true
    name: hfans@foxmail.com  ##邮箱地址
    url: http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=8JiWkZ6DsJafiJ2RmZzek5_d ##邮箱外链,邮我  如：http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=8JiWkZ6DsJafiJ2RmZzek5_d
## 联系地址相关信息
address:
    enable: true
    name: Pudong New Area, Shanghai, China ##地理位置的英文（请不要太过具体）
    url:  ##公司在百度地图上的位置的网址
## 百度熊掌号相关信息
xzHao:
    enable: true
    note: 专注Java • 分享生活 • 记录人生 ##熊掌号描述
    url: https://author.baidu.com/home/1603347506741536?from=dusite_artdetailh5 ##熊掌号url
## 备案相关信息
beian:
    enable: false
    note:  ##备案号
## 百度统计相关信息
baidu:
    enable: true
    url: https://tongji.baidu.com/web/25553450/overview/index?siteId=11976031 ##百度统计的网址，点开百度云图标后登陆可看到网站统计\
## github相关信息
github:
    enable: true
    url: https://github.com/hfanss/ ##github外链 如 ：https://github.com/hfanss/
## 码云相关信息
gitee:
    enable: true
    url: https://gitee.com/iyohei ##码云外链 如 ：https://gitee.com/iyohei
## CSDN相关信息
csdn:
    enable: true
    url: https://blog.csdn.net/q2158798 ##CSDN博客外链 如：https://blog.csdn.net/q2158798
## 底部显示设置
footersenable: true   ##是否开启底部菜单栏
footers: 
  - gywo    ##关于我
  - gzhao   ##公众号或微信二维码
  - xzhao   ##百度熊掌号相关信息
  - links   ##友情链接/关于本站/关于博主(简历)
## PC菜单显示选项  
menu:
  - page: home
    directory: .
    icon: fa-home2
  - page: archive ##显示名字，根据中英文兑换，也可直接写中文
    directory: archives/   ##链接地址（source下的文件夹）
    icon: fa-archive2   ##图标。在线图标，http://www.fontawesome.com.cn/faicons/，把名字贴这里即可
  - page: music
    directory: music/
    icon: fa-user2
  - page: tool
    directory: tool/
    icon: fa-user2 
  - page: guestbook
    directory: comment/
    icon: fa-rss2

## 移动端菜单显示选项  
mobileMenu:
  - page: home
    directory: .
    icon: fa-home2
  - page: archive ##显示名字，根据中英文兑换，也可直接写中文
    directory: archives/   ##链接地址（source下的文件夹）
    icon: fa-archive2   ##图标。在线图标，http://www.fontawesome.com.cn/faicons/，把名字贴这里即可
  - page: music
    directory: music/
    icon: fa-user2
  - page: tool
    directory: tool/
    icon: fa-user2 
  - page: guestbook
    directory: comment/
    icon: fa-rss2
  - page: about
    directory: about/
    icon: fa-rss2
  - page: site
    directory: site/
    icon: fa-rss2
  - page: href
    directory: href/
    icon: fa-rss2
## 网站地图   博主没用过，意义不大
timeline:
  - num: 1
    word: 2014/06/12-Start
  - num: 2
    word: 2014/11/29-XXX
  - num: 3
    word: 2015/02/18-DDD
  - num: 4
    word: More
# Static files。缓存目录
js: js
css: css

# 主题版本，方便刷新
version: 0.1.0


```
开关的一些说明在配置文件中都有中文解释
## 额外说明
- 评论只支持valine
- 搜索只支持self_search、baidu_search
- 网站统计只有百度统计
- 移动端默认不显示底部(关于我、熊掌号...)菜单

---
# 使用方法
## 下载主题	
> https://gitee.com/iyohei/hfanss.git

# 安装插件	
```YAML
npm install --save hexo-deployer-git hexo-generator-archive hexo-generator-category hexo-generator-index-pin-top hexo-generator-search hexo-generator-tag hexo-helper-qrcode hexo-renderer-ejs hexo-renderer-marked hexo-renderer-pug hexo-renderer-sass hexo-renderer-stylus hexo-server hexo-tag-aplayer hexo-wordcount
```
安装不成功可以通过 [淘宝镜像](https://npm.taobao.org) 下载

# 修改配置	
```YAML
博客根目录下
config.yml
URL分类下	
 url: http://www.baidu.com ## 分享页的头网址，域名地址或iyohei.githug.io	
 permalink: :year/:title.html ## 更改文章页的地址带有.html后缀	
博客根目录下 source文件夹下	
 新建about文件夹--含一个index.md文件--最下方  关于博主页（内容自行书写）	
 新建comment文件夹--含一个index.md文件--菜单栏  留言页（内容自行书写）	
 新建href文件夹--含一个index.md文件--最下方  友情链接页（内容自行书写）	
 新建music文件夹--含一个index.md文件--菜单栏  音乐页（内容自行书写）	
 新建tool文件夹--含一个index.md文件--菜单栏    工具页（内容自行书写）	
 粘贴一个favicon.ico的文件（网站图标）	
 新建CNAME文件，无后缀（需要绑定域名的请在里面书写你的域名）	、

```

以上新建文件博主都集成在主题中，大家下载下来有两个文件夹，一个为主题，一个为source，复制其中的内容覆盖自己的source即可

------

## 注意事项

> 文章页增添开关

```YAML
top: true  ##开启文章置顶
yuanchuang: true ##开启原创标签
toc: true ##开启目录
如果文章为转载，需要配置以下开关
    zhzai: true ##开启转载标签
    zhzaiName: 杨云召 ##原文作者
    zhzaiUrl: https://blog.znmlr.cn/4cabcca.html ##原文链接
```

 zhzai(转载) && yuanchuang(原创)只能开启一项

> 非菜单页选中样式问题

```
新建的页面如果没在菜单栏显示需要在index.md中  文章最下方加入以下代码：（目的是保证菜单栏的首页为选中样式）
<script>$(".header-02-3 a:first").addClass('current');</script>
效果：例如友情链接在菜单栏中没有，加入此行代码会默认选中首页这个样式
```

> 底部熊掌号使用

```YAML
qita.pug 20 行代码为自己的熊掌号script
head.pug 19行代码为自己熊掌号ID声明
```

> 百度主动推送请阅读 [说明文档](https://hui-wang.info/2016/10/23/Hexo%E6%8F%92%E4%BB%B6%E4%B9%8B%E7%99%BE%E5%BA%A6%E4%B8%BB%E5%8A%A8%E6%8F%90%E4%BA%A4%E9%93%BE%E6%8E%A5/)

## 自行优化
> 附上几个重要的文件作用，方便大家自行优化：

```YAML
base.pug		集成head部分模版+底部
archive.pug		归档页的模版
page.pug		自定义页面的模版
post.pug		文章页模版
footer.pug		尾部文件模版
footer02.pug  	底部菜单模版
head.pug		首页的模版（主要是通用JS的引用，如评论，计数器）
_footer文件夹	  底部菜单各模版
search.pug		搜索模版
推荐插件：
 详见另一篇博文  hexo博客常用插件及教程
valine评论个性头像：https://cn.gravatar.com/全球头像分享网站-注册-设置头像,在valine评论中，填上注册时的邮箱就会显示头像
```

> 详细diy

```YAML
底部菜单栏diy:
    _footer文件夹
    添加:
         在_footer文件夹中新建xxx.pug,写上内容
         在config文件中的footer下 添加进去 -xxx  即可显示
    修改:
        gywo.pug		##关于我
        gzhao.pug   	##公众号或微信二维码
        xzhao.pug  		##百度熊掌号相关信息
        links.pug  		##友情链接/关于本站/关于博主(简历)
友情链接:
	sources/href/index.md
关于本站:
	sources/site/index.md
关于博主:
	sources/about/index.md
留言:
	sources/comment/index.md
工具:
	sources/tool/index.md
音乐:
	sources/music/index.md
```

> 原版主题的配置只要没跟本主题冲突，没有特别说明，都可以支持

------

如有本主题的相关优化问题，可在下方评论区留言
github有时候会抽风，提供码云备用地址：[点我](https://gitee.com/iyohei/hfanss)
另：如大家使用本主题，还请在下载主题页  右上角   star  一下，感谢！
