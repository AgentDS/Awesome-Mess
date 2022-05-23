# Awesome-Mess

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

An *awesome* & curated list of anything that I find might be useful for computer science students. Kinda messy but try to organize it well.

Some blogs are in Chinese, and some in English. Hope this repo will be helpful for more people. 

__ENJOY IT!!__



日常碰到的收集的觉得可能对计算机相关专业学生有用的资料。可能有点乱，会不定期整理。

有些链接文章是中文的，有些是英文的。希望尽可能对更多人有用。

[toc]

## Open-source Related 开源开发相关

- 之前的[__tensorD__](https://github.com/Large-Scale-Tensor-Decomposition/tensorD)项目可作为参考，包括API说明以及文档格式

- [Python Open-Source Project Developer Guide](http://www.wbh-doc.com.s3.amazonaws.com/Python-OpenSource-Project-Developer-Guide/Chapter0%20-%20Prelude.html)

- [How to Take Your Open Source Project from Good to Great](https://open.nytimes.com/how-to-take-your-open-source-project-from-good-to-great-49c392175e5c)

- [如何在GitHub上做一个优秀的贡献者？ - phodal的回答](https://www.zhihu.com/question/310488111/answer/585336948)

- [Open Source: Automating Release Notes in Github](https://open.nytimes.com/open-source-automating-release-notes-in-github-dd08f964465c)

- __Git相关__

  - [Git小书](https://github.com/865077695/book)
  - [什么是 .gitkeep ？](https://www.codenong.com/cs106131919/)
  - [GitHub无法访问、443 Operation timed out的解决办法](https://juejin.cn/post/6844904193170341896) 
  - [Gitignore not working?](https://stackoverflow.com/questions/25436312/gitignore-not-working)
  - Git的GUI客户端：
    - [SourceTree](https://www.sourcetreeapp.com/): macOS, windows
    - [GitKraken](https://www.gitkraken.com/): macOS, windows
  - [Git 使用规范流程](https://www.ruanyifeng.com/blog/2015/08/git-use-process.html)
  - [团队协作中的 Github flow 工作流程](https://zhuanlan.zhihu.com/p/39148914)
  - [Git分支管理策略](https://www.ruanyifeng.com/blog/2012/07/git.html)
  - [Git 分支命名规范](https://cheenwe.cn/2016-08-02/git-branch-and-usage/)

- __Python package的打包与发布__

  - [花了两天，终于把 Python 的 setup.py 给整明白了](https://zhuanlan.zhihu.com/p/276461821)
  - [Python打包的两三件事](https://www.escapelife.site/posts/fc616494.html)
  - [编写 python package 中的 setup.py 文件](https://www.jianshu.com/p/9a5e7c935273)
  - [Python 库打包分发(setup.py 编写)简易指南](https://blog.konghy.cn/2018/04/29/setup-dot-py/)

- __Python模块与包__

  - [第十章：模块与包](https://python3-cookbook.readthedocs.io/zh_CN/latest/chapters/p10_modules_and_packages.html)
  - [open-source项目文件结构一个示范](https://github.com/jrzaurin/pytorch-widedeep)

- __README相关__

  - [Standard Readme如何写标准README](https://github.com/RichardLitt/standard-readme)
  - [Best-README-Template: An awesome README template to jumpstart your projects!](https://github.com/othneildrew/Best-README-Template)
  - [Awesome README: A curated list of awesome READMEs](https://github.com/matiassingers/awesome-readme)
  - [项目徽章badges](https://lpd-ios.github.io/2017/05/03/GitHub-Badge-Introduction/)
    - 持续集成状态：[Travis CI](https://travis-ci.org/)对开源项目免费
    - 覆盖率：单元测试，[coveralls](https://coveralls.io/)与`coverage`
  - 协议License
    - [如何选择License](https://zhuanlan.zhihu.com/p/51331026)
    - 阮一峰[如何选择开源许可证？](http://www.ruanyifeng.com/blog/2011/05/how_to_choose_free_software_licenses.html)
    - [如何将 Apache License 2.0 应用到你的项目](https://adoyle.me/blog/how-to-apply-the-apache-2-0-license-to-your-project.html)

- __持续集成状态__

  - Travis CI不支持organization的private repo，__放弃吧__
    - [持续集成服务 Travis CI 教程](http://www.ruanyifeng.com/blog/2017/12/travis_ci_tutorial.html)
    - [使用Travis进行持续集成](https://www.liaoxuefeng.com/article/1083103562955136)
    - [The Travis CI Cookbook - Python](https://blog.travis-ci.com/python-cookbook)
    - [Extensive Python Testing on Travis CI](https://blog.travis-ci.com/2019-08-07-extensive-python-testing-on-travis-ci)
    - [带你入门travis-ci](https://151250010.github.io/2017/08/08/%E5%B8%A6%E4%BD%A0%E5%85%A5%E9%97%A8travis-ci/)

  - 改用Github Actions
    - [Introduction to GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/introduction-to-github-actions?learn=getting_started)
    - [Building and testing Python](https://docs.github.com/en/actions/guides/building-and-testing-python)
    - [Codecov GitHub Action](https://github.com/marketplace/actions/codecov)
    - 其他跟codecov和coverage的结合用法直接上GitHub搜人家代码：直接用[Codecov GitHub Action](https://github.com/codecov/codecov-action)

  - unit test代码覆盖率

    - coverage + codecov 支持organization的private rep
      - codecov的配置文件`codecov.yml`写法直接看[官方文档](https://docs.codecov.io/docs/quick-start)

    - coverage + coveralls
      - coveralls不支持organization的private repo
      - [Travis CI+Coveralls大致流程](https://yumminhuang.github.io/post/travisci/)

- __Unit test__

  - [`slumber`利用unittest编写tests示范](https://github.com/samgiles/slumber)
    - 在[`tests.__init__.py`文件](https://github.com/samgiles/slumber/blob/master/tests/__init__.py)中加载所有test suite
    - 项目[`setup.py`](https://github.com/samgiles/slumber/blob/master/setup.py)脚本中指定`tests_require`和`test_suite`
  - [`unittest` — Unit testing framework](https://docs.python.org/3/library/unittest.html#module-unittest) ->官方文档
  - [廖雪峰：单元测试](https://www.liaoxuefeng.com/wiki/1016959663602400/1017604210683936)
  - [提高你的Python能力：理解单元测试](https://segmentfault.com/a/1190000000400091)
  - 各位都是怎么进行单元测试的？ - 大宽宽的回答 - 知乎 https://www.zhihu.com/question/27313846/answer/853193909
  - 各位都是怎么进行单元测试的？ - gashero的回答 - 知乎 https://www.zhihu.com/question/27313846/answer/120164282
  - [unittest使用详解](https://blog.csdn.net/qq_43422918/article/details/98477312?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522161603835716780274152423%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=161603835716780274152423&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_click~default-1-98477312.first_rank_v2_pc_rank_v29&utm_term=unittest) 
  - [Python必会的单元测试框架 —— unittest](https://blog.csdn.net/huilan_same/article/details/52944782?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522161604832616780264095649%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=161604832616780264095649&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_v2~hot_rank-1-52944782.first_rank_v2_pc_rank_v29&utm_term=unittest)
  - torch相关代码如何做unit test？
    - [如何才能信任你的深度学习代码？](https://zhuanlan.zhihu.com/p/193102308)（[完整源码](https://github.com/tilman151/unittest_dl)）
    - 

- <span id = "docs">__文档开发与托管__</span>

  - [Sphinx](https://www.sphinx-doc.org/en/master/)+[Read the Docs](https://readthedocs.org/) (__Read the Docs对private repo收费，开发时候放弃吧!__)

    - [Get Start](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html)

    - 使用[Sphinx](https://www.sphinx-doc.org/en/master/)开发文档

      - Sphinx使用标记语言[reStructuredText](https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)编写文档

      - [用sphinx生成python文档](http://bondlee.github.io/2016/04/24/%E7%94%A8sphinx%E7%94%9F%E6%88%90python%E6%96%87%E6%A1%A3/)

      - [如何使用Sphinx生成Python文档](https://zhuanlan.zhihu.com/p/65947968)

      - Sphinx主题

        - 最主流的`sphinx_rtd_theme`：[Read the Docs Sphinx Theme](https://github.com/readthedocs/sphinx_rtd_theme) (__画风就真的很丑哈，实在没办法才换回来__)

          > 可以去GitHub看人家rst文件写法

        - [Sphinx Themes Previews](https://sphinx-themes.org/)

        - ~~目前用了[`sphinx-typo3-theme`](https://pypi.org/project/sphinx-typo3-theme/)主题([example](https://sphinx-themes.org/sample-sites/sphinx-typo3-theme/))~~

        - 目前用了[Furo](https://pradyunsg.me/furo/quickstart/)主题

          - 如何自定义修改相关元素: [Customisation](https://pradyunsg.me/furo/customisation/)
          - [urllib3的文档](https://urllib3.readthedocs.io/en/latest/)主题也是Furo，供参考

      - Sphinx文档自动抽取

        - `*.py`代码中的API docstrings可用Sphinx原生的扩展`sphinx-apidoc`抽取（语法直接看`sphinx-apidoc`的文档），但是build出来的效果不是很好而且不够auto。。。
        - <span id = "pycharmdocs">docstrings风格在PyCharm中的设置：[sphinx+python项目文档自动生成](https://www.cnblogs.com/combfish/p/10297987.html)</span>
        - [Google Python代码风格指南](https://google.github.io/styleguide/pyguide.html)
        - [Example Google Style Python Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html#example-google)
        - 增加第三方[sphinx-autoapi](https://sphinx-autoapi.readthedocs.io/en/latest/tutorials.html#setting-up-automatic-api-documentation-generation)插件！！！！

        > #### 注意事项
        >
        > __简易流程：__
        >
        > 1. 编写rst
        > 2. 当前目录到`docs`下，执行build相关指令生成html文件
        >
        > 
        >
        > __尽量不要直接用原生的apidoc，难用。。。__
        >
        > 建议安装`sphinx-autoapi`来构成自动docs抽取！！！！！！比原生的`sphinx.ext.autodoc`的效果好很多。。。。手动改rst之后进行build（`sphinx-autoapi`是否能自动生成rst？看文档），build要用的命令行：
        >
        > ```bash
        > # 目录切到docs下
        > # 移除build中原有文件
        > $ rm -r build
        > # 正式build
        > $ sphinx-build -b html ./source build
        > ```

    - Read the Docs: 

      - [Importing Your Documentation](https://docs.readthedocs.io/en/stable/intro/import-guide.html)
      - [创建并部署你的文档](http://www.wbh-doc.com.s3.amazonaws.com/Python-OpenSource-Project-Developer-Guide/Chapter3%20-%20Doc.html)
      - __务必要在GitHub项目中添加ReadTheDocs的hook！__

    - [【Open-Source】Sphinx+Read the Docs的多语言版本文档实现](https://zhuanlan.zhihu.com/p/427843476)

  - __Sphinx + GitHub Page__

    - [Yes You Can Use GitHub Pages with Python Sphinx](https://www.docslikecode.com/articles/github-pages-python-sphinx/)
    - [Publishing sphinx-generated docs on github](https://daler.github.io/sphinxdoc-test/includeme.html)
    - [How to use github pages from master /docs folder elegantly with sphinx](https://github.com/sphinx-doc/sphinx/issues/3382)
    - [可能有用：Github Action插件Sphinx Pages](https://github.com/marketplace/actions/sphinx-pages)

- __需要发布PyPI上吗__

  - [如何将自己的程序发布到 PyPI](https://zhuanlan.zhihu.com/p/26159930)

- 用Teambition进行合作: https://www.teambition.com/apps/

- Python Register module:

  - [Python中的注册器模块](https://applenob.github.io/python/register/)
  - [Python register在DELTA项目中的应用](https://github.com/Delta-ML/delta/blob/master/delta/utils/register.py)

- 





## Linux Server 服务器使用

### 服务器使用

- [如何用SSHFS？让服务器文件系统挂到自己本地系统里方便文件传输](https://blog.csdn.net/myhes/article/details/106712863)

  1. 下载`osxfuse` 

     ```bash
     brew install --cask osxfuse
     ```

  2. 下载`sshfs`  

     ```bash
     brew install sshfs
     ```

  3. 设置文件目录挂载

     ```bash
     # 创建本地目录,用于挂载
     $ mkdir -p xxxx/mount_remote
     
     # 挂在远程目录到本地，输入密码即可，若要免密，创建sshkey即可
     $ sshfs xxxx@x.x.x.x:/home/yyy /xxxx/mount_remote -p port_num
     
     # 在macOS的Finder里像用本地正常文件夹一样打开远程目录，进行操作
     
     # 使用结束，取消挂载(有时候会自动断掉链接，就不用手动取消挂载了)
     $ umount /xxxx/mount_remote
     ```

- [使用`expect`完成脚本一键登录服务器](https://github.com/AgentDS/CSCI-596-18fall)（README.md中的<u>Tips on Using SFTP & SSH</u>）

- [nvidia-smi查看GPU的使用信息并分析](https://blog.csdn.net/wumenglu1018/article/details/103057009#:~:text=%E5%8E%9F%E6%96%87%EF%BC%9Ahttps%3A%2F%2Fdeveloper.nvidia,%2Dmanagement%2Dinterf...&text=%E9%A6%96%E5%85%88%E6%89%93%E5%BC%80C%E7%9B%98%EF%BC%8C%E6%89%BE%E5%88%B0,%E5%9B%9E%E8%BD%A6%E5%90%8E%E6%98%BE%E7%A4%BAGPU)

- [通过SSH远程使用jupyter notebook](https://blog.csdn.net/u014022205/article/details/81025660?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-7.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-7.control)



### Docker







## Paper Writing 论文写作

- [論文引用格式：如何在學術論文中正確的引用文獻？](https://www.editing.tw/blog/writing/%E8%AB%96%E6%96%87%E5%BC%95%E7%94%A8%E6%A0%BC%E5%BC%8F-%E5%A6%82%E4%BD%95%E5%9C%A8%E5%AD%B8%E8%A1%93%E8%AB%96%E6%96%87%E4%B8%AD%E6%AD%A3%E7%A2%BA%E7%9A%84%E5%BC%95%E7%94%A8%E6%96%87%E7%8D%BB.html)
- [论文写作点滴：合理和有效的引用参考文献](https://www.xiahepublishing.com/2475-7543/MRP-2018-002)
- [Paper Writing Checklist Prepared by Prof. Zheng Zhang, UCSB](https://web.ece.ucsb.edu/~zhengzhang/paper%20writing%20checklist_v2.pdf)
- 文献管理工具：
  - [Zotero](https://www.zotero.org/)：
    - [我的 Zotero 实践汇总 - Hsin的文章](https://zhuanlan.zhihu.com/p/108366072)
    - 
  - 印象笔记EndNote
- Latex写作与常用machine learning符号写法
  - [machine learning符号写法](https://ctan.math.utah.edu/ctan/tex-archive/macros/latex/contrib/mlmath/)
  - [latex数学符号](http://mohu.org/info/symbols/symbols.htm)
  - [Paper Writing Tips](https://github.com/MLNLP-World/Paper-Writing-Tips)
- 数学公式Latex自动识别[Mathpix Snap](https://mathpix.com/)
- Python画图
  - [Python科研统计作图Plotnine+Seaborn+matplotlib替代R ggplot2系列！（一）](https://zhuanlan.zhihu.com/p/30933555)
- 实验log：wandb.ai
- 表格的latex代码自动生成https://www.tablesgenerator.com/
- 时间序列动图的可视化https://flourish.studio/
- 同义词查询https://www.thesaurus.com/
- 语言查询https://linggle.com/
- 用词搭配愈发查询https://www.writefull.com/
- overleaf上语法矫正Overleaf textarea插件
- 画图draw.io
- 文章取名https://acronymify.com/







## Personal Page 个人网页

- [GitHub Page](https://docs.github.com/en/pages)

  - [Quickstart for GitHub Pages](https://docs.github.com/en/pages/quickstart)
  - [Getting started with GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages)
  - [Setting up a GitHub Pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
  - [Configuring a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

- __关于Hexo vs Jekyll:__

  - [静态博客框架之Hexo & Jekyll](https://www.jianshu.com/p/ce1619874d34)
  - [hexo VS jekyll](https://www.daimajiaoliu.com/daima/47948b785900404)
  - [Git Pages + Jekyll/Hexo搭建自己的博客(最全总结你想知道的都在这里了)](https://blog.csdn.net/muzilanlan/article/details/81542917)
  - [静态博客框架jekyll、hexo和hugo三者之间的区别与差异](https://zhuanlan.zhihu.com/p/368407566)
  - [更换博客系统——从jekyll到hexo](https://segmentfault.com/a/1190000002398039)

- 用 GitHub Page + Jekyll 建立个人网站

  - [Jekyll快速开始教程](https://www.jiansoft.net/2020/04/26/Jekyll_quick_start.html)

  - [Jekyll - Static Site Generator|Tutorial](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB) <font color="Red">(强烈推荐highly recommended)</font>

  - [Jekyll搭建个人博客-拓展版](https://javef.github.io/2018/02/Jekyll-%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2-%E6%8B%93%E5%B1%95%E7%89%88/)

    > 可能会在本地执行`exec jekyll serve`时候报错：``require': cannot load such file -- webrick (LoadError)`，可以通过执行以下来解决：
    >
    > If there is feedback ``require': cannot load such file -- webrick (LoadError)` when executing `exec jekyll serve`, try to use follow command to resolve this:
    >
    > ```bash
    > bundle add webrick
    > ```
    >
    > 参考reference：[Load error: cannot load such file – webrick](https://talk.jekyllrb.com/t/load-error-cannot-load-such-file-webrick/5417)

  - github上利用jekyll搭建自己的blog的操作顺序？ - 王彦宁的回答 - 知乎 https://www.zhihu.com/question/30018945/answer/50507749

  - [Jekyll theme TeXt: Quick Start](https://tianqi.name/jekyll-TeXt-theme/docs/en/quick-start)

  - [如何搭建一个独立博客——简明 GitHub Pages与 jekyll 教程](https://www.cnfeat.com/blog/2014/05/11/how-to-build-a-blog/)

  - [Jekyll使用教程笔记 一](https://juejin.cn/post/6844903623567081486)

  - [Jekyll使用教程笔记 二](https://juejin.cn/post/6844903629246169096)

  - [Jekyll使用教程笔记 三](https://juejin.cn/post/6844903629682376711)

  - [Jekyll使用教程笔记 四](https://juejin.cn/post/6844903629934084109)

  - [Jekyll使用教程笔记 五](https://juejin.cn/post/6844903630001160199)

  - [Jekyll使用教程笔记 六](https://juejin.cn/post/6844903632882630664)

  - [菜鸟级jekyll教程(1)](https://waliblog.com/jekyll/2017/11/21/jekyll(1).html)

  - [jekyll 教程入门](https://wenfengsat.github.io/2018/06/19/jekyll%E6%95%99%E7%A8%8B%E5%85%A5%E9%97%A8/)

  - 

- 用 GitHub Page + Hexo 建立个人网站

  - [GitHub+Hexo 搭建个人网站详细教程](https://zhuanlan.zhihu.com/p/26625249)

- 一些DIY相关blog

  - mo_wang关于GitHub Page搭建blog的系列
    - [【一】Ubuntu14.04+Jekyll+Github Pages搭建静态博客 ](https://www.cnblogs.com/mo-wang/p/5115266.html): 安装方面
    - [【二】jekyll 的使用 ](https://www.cnblogs.com/mo-wang/p/5117408.html): jekyll的配置
    - [【三】用Markdown写blog的常用操作 ](https://www.cnblogs.com/mo-wang/p/5117819.html): Markdown的使用
    - [【四】搭建Markdown的编辑器 ](https://www.cnblogs.com/mo-wang/p/5118144.html) （__不如直接Typora__）
    - [【五】将博客从jekyll迁移到了hexo ](https://www.cnblogs.com/mo-wang/p/5119967.html)

  

