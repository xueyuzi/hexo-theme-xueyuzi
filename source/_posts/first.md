---
title: hexo主题:自定义路由
---

　　在制作主题的过程中 发现 官方的文档 就路由这部分的解释非常模糊，没有详细讲明其中已经定义的路由和怎样自定义路由。
hexo给我们提供的默认路由是/index.html,对应layout文件夹下的index.ejs,但是其他的路由却不能和对应的模板匹配。
　　所以只能曲线救国，首先通过创建一个模块page: <code class="code">hexo new page [路由名]</code> 这样创建的路由就都可以匹配到layout文件下的page.ejs，
然后吧page.ejs当做路由的入口文件，就解决了网站自定义路由的问题。