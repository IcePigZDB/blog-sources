---
layout:     post
title:      "生如夏花之绚烂 "
subtitle:   "Let life be beautiful like summer flowers."
date:       2020-04-19 23:59:59
author:     "IcePig"
header-img: "img/in-post/2020-04-19-blog-design-and-implement/summer-flower.jpg"
catalog: true
tags:
    - 博客实现
typora-root-url: ..
---

> 本文记录了2020年4月18日开始的个人博客的设计思路与实现方法。
> This document is not completed and will be updated anytime.

<!-- excerpt -->

## 博客需求分析与风格选型

* 博客个性签名的选择

  “**生如夏花之绚烂，死如秋叶之静美**”出自印度诗人泰戈尔所作《飞鸟集》第八十二首

  **"Let life be beautiful like summer flowers and death like autumn leaves."**的郑振铎译本。这首小诗有且仅有这一句，却优美而含蓄地表达出了作者的人生观和世界观，夏花是旺盛生命的象征，生如夏花，活着，就要灿烂、奔放，要像夏天盛开的花那样绚烂旺盛，要善待生命、珍惜生命，要活得有意义、有价值，而不要浑浑噩噩地过日子；秋叶，感伤，惆怅，凄美，安静，面临死亡，面对生命向着自然返归，要静穆、恬然地让生命逝去，不必轰轰烈烈，便只要像秋叶般悄然足已，更不要感到悲哀和畏惧。总而言之，就是一切都平静自然地进行。

  这句话前半句与我原想拿来当博客签名的**"Love life and enjoy work."** 都体现了要珍惜时光，不负韶华，好好奋斗，努力拼搏，热爱生活，享受工作的生活态度，至于后半句现在确实感悟不多，你好，我的邻居，谢谢你的分享。

* 博客功能需求

  * Name:~~其实我名字和数据库还挺有缘分的，简写下来是ZDB后面就是DataBase的简写，就叫做Db's Blog了，刚好研究生方向是数据库，不好好整也说不过去了，以后开发一个ZDB?~~
    * IcePigZDB's Blog ✔ 
    * Db's Blog
    * DB's Blog
    * Z Db's Blog
    * DbZ's Blog
    * Bing's Blog 名字的冰其实我很喜欢。
  * About: ~~大家好我是ZDB，刚好又研究数据库，所以博客名是Db’s Blog之类罗。~~
  * Home:按最近的时间线来整。
  * Archive: Tags and Time Line
  * [Books](https://izualzhy.cn/books.html):分享书籍，这个可以吧，其实也可以通过标签来实现。
  * [Pearls](https://izualzhy.cn/pearls.html)
  * Leetcode?头秃，生活好无趣，可以通过标签来实现。
  * 论文分享，毕竟是学硕，还是要好好整的，也可以通过标签来实现。
  * 自己这几天冒出来一个想法，想做一个Application或者博客里面的一个页面，可以用来记录每一天干的事情，然后一周之后会有一个周总结，周总结会把上一周每一天的覆盖了，每个月会有一个月总结，月总结会把周总结覆盖了，如果想要看细节的话就可以展开看，这样可以大概回顾自己这些日子把时间花在哪了？自己到底学过了什么东西？是一种能够促进自己回顾与展望的机制，能够加强记忆和时间管理。
  * 阅读次数统计
  * 搜索功能

* 博客模板

  * [黄玄Hux作者博客](https://huangxuan.me/)  [一个Hux的用户博客](http://kaiyuan.me/)
  * [毕设期间看的比较多的LevelDB大佬的博客风格](https://izualzhy.cn/archive.html)

* 框架选定

  * 博客要注重于内容，所以还是抄别人的模板吧，[黄玄Hux作者博客](https://huangxuan.me/) 好看，其实对我个人而言可能有点不是很简约了，不过先整整试试，不喜欢再换。
  
* [博客部署方式19分32秒](https://www.youtube.com/watch?v=7lFxEsF5Rw0)

  * github等机构的pages
  * 自备服务器/虚拟主机
  * surge.sh，类似于pages，会免费提供一个域名。

## 换名行动-> IcePigZDB

* [x] zdb424395031-> **IcePigZDB** 

  * IcePig是老姐之前给我想的，必须用，自己用的也很自然舒服。
  * Z是姓名没有用英文的习惯把姓放在最后出于两个原因
    * DbZ DBZ和 Orz有点像。
    * ZDB DataBase 不管以后能不能开发Z's DataBase，ZDB伏笔了。

* [ ] 谷歌邮箱原来的地址 zdb424395031@gmail.com太傻逼了，我想换一个。

  * ✘ @gmail.com这个是不能改的，但是可以通过添加辅助邮箱来解决，辅助邮箱只是多一个邮箱登录， IcePigZDB@gmail.com。

  * ✘ 那我就想把原来的删除了。 

    * 删除一个东西你要考虑后果！比如Google Drive上面的文件，又比如谷歌浏览器上的书签等，各种账号绑定等，比如说Github绑定的就是zdb424395031@gmail.com

  * ✔ 想到了一个比较好的办法，把自己旧的谷歌账号绑定到我姐姐的手机号上，然后就可以用自己的手机注册一个新号了,这样会有一个过渡期，反正老姐也用不到谷歌账号。 

    * 但是问题来了，我自己的手机号并没有被释放出来，于是搜那个错误，找到了知乎上的一个回答，用https://accounts.google.com/SignUpMobile先注册，注册好的账号会因为手机号绑定多个账号被停用，然后申请恢复，已经申请，两天内回复，申请内容如下。

      ```
         I used to have a google account zdb424395031@gmail.com wiht the phone number 155-----315. I want to change my googel email address to IcePigZDB@gmai.com,i google a lot ,but there seems no way.
         So i change the old account's phone number to my sister's and the old account now belongs to her.I think my phone number should be freed now, so i register this new account IcePigZDB@gmail.com whit my phone number,but the rules and codes behind users module in your company seems do not allow or just respond slowly.I think my request is reasonable. 
         Last but not least ,i am very appreciate Google Company and many helpful products.Look forward to your reply, thank you and holp you healthy.
      ```

* [x] github 名字有2种，一种是昵称，一种是username，换昵称随便换，username换了之后仓库地址会Redirect（按以前的用户名访问仓库的话会映射成访问新的用户名地址的仓库），但是Profile page和Github pages不会，比如你的领英或者博客上的链接就要自己手动更新为新的的username.github.io如果直接用域名的话就要更新你的DNS解析记录。

  * **name** :IcePIgZDB  **username**:IcePigZDB

  * ```
    We will not set up redirects for your old profile page.
    We will not set up redirects for Pages sites.
    We will create redirects for your repositories (web and git access).
    Renaming may take a few minutes to complete.
    ```

    

## Blog 1.0

* [Hux中文文档](https://github.com/Huxpro/huxpro.github.io/blob/master/README.zh.md)

  * 先git stable 版本Hux模板 git clone git@github.com:Huxpro/huxblog-boilerplate.git

  * 安装[jkyll on Windows](https://jekyllrb.com/docs/installation/windows/),win10不是官方支持版本，不得不说MAC香,Linux对于我个人来说是懒得折腾的，没有啥意义吧，jkyll是基于Ruby的，先要配置Ruby环境。

    * 不过是直接exe安装，最后的ridk install 看不太懂全部enter了。

    * 装了Ruby之后通过Ruby的包管理器>gem install jekyll bundler 安装jkyll。

    * ```
      >jekyll -v // 测试命令，输出以下信息表示安装安装成功
      jekyll 4.0.0
      ```

  * Github Pages

    * 作为github pages的仓库只能公开，私有的话要交钱。Upgrade to GitHub Pro or make this repository public to enable Pages.4美元一个月。
    * [ ] 如果不想别人内容被怎么样的话，要注意协议的选取。首先你用的是别人的模板，那模板代码方面的开源协议拿过来那一下协议就定下来了，查看License文件得知是Apache License2.0。但是自己的内容肯定要保护一下，知识产权？

  * 根据文档进一步个人化，在_config.yml、index.html里面设置博客名字、博客首页签名、博客图标等。

* [x] [博客评论系统的选择](https://weiweitop.fun/2019/08/10/%E9%9D%99%E6%80%81%E5%8D%9A%E5%AE%A2%E8%AF%84%E8%AE%BA%E7%B3%BB%E7%BB%9F%E7%9A%84%E6%AF%94%E8%BE%83%E5%8F%8A%E9%80%89%E6%8B%A9/) ->**暂且不提供评论功能，有事邮件。**

  * 默认提供的多说倒闭了，网易云跟帖也倒了。
  * Disqus要钱，独立系统要有Disqu账号。
  * 用Gitalk 利用了github issue 利用两个Label来匹配Gitalk和文章唯一ID,看到有人说gitalk向github要的权限太大了，不安全，不过是因为github权限粒度细分不够，要给所有rep的写权限。

* [ ] 如何增加网站的Seo（Search Engine Optimization）

  * 购买了域名icepigzdb.xyz以及**icepigzdb.com**，更喜欢用后面那个，如果不开多个仓库不能使用多个域名，那就用后面那个了。

  * [ ] [Google站长分析工具](https://accounts.google.com/ServiceLogin/webreauth?service=sitemaps&passive=1209600&continue=https%3A%2F%2Fwww.google.com%2Fwebmasters%2Ftools%2F&followup=https%3A%2F%2Fwww.google.com%2Fwebmasters%2Ftools%2F&authuser=0&flowName=GlifWebSignIn&flowEntry=ServiceLogin)

  * [ ] [百度站长分析工具](https://ziyuan.baidu.com/?castk=LTE%3D) 

    方法一不能用了，我更换最新版本的博客代码之后，rubygems版本需要2.7以上，而coding服务器的之后2.6.x,所以先只部署在github上等以后文章多了再部署回国内吧，无所谓了。

    * [ ] ✘法一： [github pages 拒绝百度spider的访问导致了百度不收录如何解决](https://blog.csdn.net/damontive/article/details/89856143)，提出了coding（腾讯）+github双部署的[解决方案](https://10101.io/2018/09/18/Blog_3)，码云也有pages服务，不过Coding现在被腾讯爹爹收购了，以后稳步看好，且coding的pages仓库可以设置为私有的。
      * 注册Coding团队账号之后，新建一个项目推荐新建**DevOps**项目，这个项目是默认开启了静态博客功能的，而我选择了**代码托管项目**，这个默认是没有开启静态博客的，因为对coding的新节目的不熟悉，加上刚刚被腾讯收购大改版，他家的文档不全，网上教程也没有，所以我整了半个小时都没整明白，然后就打了他家的客服电话，告诉了我项目页面里面的左下角有个项目设置，里面开启**持续集成** **持续部署**，就可以了。

      * 另一个需要注意的是Coding注册都是以团队为单位的，2020年4月19日我用微信注册之后username就是我的手机号，不同于github pages的是，新版的Coding pages不需要创建一个以 username.github.io这样的仓库才能用生成pages，随便一个blog代码仓库只要开启静态博客功能就能生成一个pages域名网址如：[https://8auj0r.coding-pages.com](https://8auj0r.coding-pages.com/)，开启之后就按上面提到过的[教程](https://blog.csdn.net/damontive/article/details/89856143)进行DNS复用解析，这边我直接将coding提供的国内地址作为了默认解析，境外的走github pages，这样百度spider就可以抓取了，具体效果如何还要观察。[参考1](https://cloud.tencent.com/document/product/302/5518) [参考2](https://help.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site)

      ![DNS复用解析](/img/in-post/2020-04-19-blog-design-and-implement/DNS-setting.png)

    * [ ] ✔ 除了coding + github pages还有一种解决方案 [zeit.co](https://zhuanlan.zhihu.com/p/111773896)

  * [x] 强制HTTPS设置以及SSL证书的获取。

    * [http与https的区别？为何要强制https？](https://juejin.im/entry/58d7635e5c497d0057fae036)更安全。http明文传输，https 在加了一层SSL，公钥私钥加密传输，但是增加了开销，SEO方面如果用HTTPS的话排名会更高
    
  * http返回的状态码[一览表](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81)，特别提出来几个。200OK、404 NOT FOUND、301被请求的资源已永久移动到新位置，并且将来任何对此资源的引用都应该使用本响应返回的若干个URI之一,[就被用来实现HTTP转移到HTTPS](https://www.seoshipin.cn/seojiqiao/2298.html)。
    * 浏览器提示链接不安全的可能原因：

      * 没有用HTTPS协议，用的是HTTP协议。
    * SSL证书过期，网站持有者应该抓紧更新。
      * 网页中调用了非HTTPS的外部资源（图片或者JS）。

* [x] 如何完成一次Post

  本篇的内容就是一个jekyll的post样板，主要有2个点：一个是post头，另一个是post中的图片处理。

  * post头就像本post最开头那样写好啦，要注意标签要省着用,多了看起来烦。

  * 如何实现typora、github mark down预览模式、博客中图片都能够完整的显示。

    * 首先jekyll要求 _post 和 img (资源文件夹，名字自取) 要放在同一级, jekyll 根据post找图片的时候始终会从根目录username.github.io/img/找下来。

    * typora 偏好设置->图像插入时 复制到制定位置并将地址设为 `../img/in-post/${filename}`（这个中间文件夹in-post可有可无），在每一篇post的开头配置行中加入`typora-root-url:..`，这样插入图片的时候，就会自动在_post平级的img文件下面生成一个与post同名的文件夹并放入名称类似`../img/in-post/post_name/picture_name.png`的图片,通过`/img/post_name/picture_name.png`引用图片的时候typora会去找`../img/post_name/picture_name.png` 能够预览图片，在github pages时`typora-root-url:..` 无效，找的还是`/img/post_name/picture_name.png` 能够正确显示图片。

    * 引出了一个要求，以后所有的新的typora文章都采用平级的img来存储图片。为了能够更加快速的迁移发布或者在不同电脑/系统上迁移，这样在win下设置目录格式吧：

      ```
      +-- calasification分类
          +-- _drafts 当前分类的草稿
          |   +-- 2020-04-19-example1.md
          |   +-- 2020-04-19-example2.md
          +-- img 当前分类的图片
          |   +-- 2020-04-19-example1
          |   +-- 2020-04-19-example2
      ```
  
* [x] [如何自定义文章摘要](https://jekyllcn.com/docs/posts/)。

* [ ] 网站如何被百度以及谷歌收录

  要给百度以及谷歌主动提交sitemap，加快收录速度。

  * [x] 百度有三种方式：主动推送，通过token和API给百度服务器发送url文件;自动推送，在网站的html代码里加入java script脚本，当网站被访问的时候会自动提交给百度服务器；sitemap推送，jekyll可以装jekyll-sitemap插件，自动生成sitemap文件，通过链接https://icepigzdb.com/sitemap.xml在百度平台上提交sitemap。 参考：[平台工具使用帮助2/24](https://ziyuan.baidu.com/college/courseinfo?id=267&page=2#h2_article_title4) ，[对于大企业的网站是三个都用，相互补充](https://ziyuan.baidu.com/college/articleinfo?id=874)
  * [ ] 谷歌

* [ ] 以后添加自己想要的模块

  - [ ] 添加自己的模块首先要看懂原来的代码格式。[官方文档](https://jekyllcn.com/docs/home/)，[简约版文档](https://gist.github.com/biezhi/f88be58ef4ae0f3741bb36ab8daa53c5)。
  - [ ] 阅读次数
  - [ ] 搜索功能







