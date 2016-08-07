# MonkingStand.github.io #
blog of MS

##【关于此项目】 ##
本项目主要基于github的代码托管和他提供的“页面自动生成器”（***Launch automatic page generator***应该没翻译错吧）。

本项目开始的契机：自己想搭一个博客，但是又不想用别人给的平台（博客园、CSDN这种），因为版式、布局都是定好的，没什么自己想发挥的空间。

但是又不会折腾后台，又不想折腾数据库，同时也不想用别人给的解决方案，所以后来想了个办法，用纯静态页面的方式（因为github提供了“页面自动生成器”这一东西），结合本地json模拟ajax的情形，就完成了一个个人博客的搭建。

ver 1.0 版本完成后，总结了一下，有点类似于SPA。


##【关于博客内容】 ##
结合项目的结构目录，用于存储博文内容的json文件放在***res/papers/***文件夹中。

该目录下的***category.json***文件主要存储了全部文章的一些索引信息、标签对应哪些文章、时间轴中某个年月对应哪些文章。

该目录下的***content***文件夹主要存储了全部的文章内容，***content001.json***（可能是***content002.json***等等）就是一篇博文内容。

该目录下的***img***文件夹主要存储了全部的图片（博文中需要配图显示的，图片全部存储在该目录下）。


##【关于博客内容的格式】 ##
其实主要是对于***res/papers/***下的内容的格式说明。在此之前对markdown有过一点了解，后来把两者对比了一下，好像我这个就是山寨、简化版的markdown。

详细的说明在该目录下的***readme.txt***中，在此不再赘述。至于为何没有用md文件，因为md适合在线看，但是在线看，就需要把里面的html内容转换格式，此时再切换到本地查看的话，看起来又不是特别方便，最后才决定使用最原始的文本好了。


##【关于博客内容编辑、上传】  ##
当需要新增一篇博文时，现在***category.json***中新增索引内容，具体需要哪些内容可以参考我在上面写的一些内容，至于格式，参考***readme.txt***中的说明。

在本地进行编辑（主要针对***category.json***目录索引文件，或者***contentxxx.json***博文内容文件）、新增（主要是修改***category.json***目录索引文件，以及***contentxxx.json***博文内容文件），编辑、新增结束后，使用***github desktop***或者***git bash***等工具（当然也可以直接上github进行在线的代码上传操作），进行commit、push操作，然后，再访问对应的页面，可以看到内容更新了。

PS：感觉还是***github desktop***这个工具比较方便。
