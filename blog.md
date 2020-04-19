---
layout: default
title: blog
---
<h2>创建自定义自己的博客</h2>
<h3>之前有其他的博客但是很少去写东西所以就没去打理，但是突发奇想的想自定义一个自己的园子，由于自己写博客挂在外网需要申请服务器，感觉有点浪费，然后就想到了 github的托管网页，由于github的静态网页是基于jekyll生成的所以只要本地搭建一个jekyll环境，如果写的文章可以跑的话，基本在github的静态网页就没问题了。自己要做的事情就是把自己的站点git到github的仓库就可以了。</h3>

<h2>jekyll教程</h2>
<ul>windows下搭建jekyll环境
  <li>首先需要下载ruby,适合windows系统的<em><a href="https://rubyinstaller.org/downloads/" style="text-decoration:none" target="_blank">RubyInstaller</a></em>下载安装2.4和比较新的版本+dev的，使用默认安装进行安装.</li>
  <li>安装玩最后一步不要勾选运行安装dev,因为程序自动安装的比较慢，这里需要更换源；安装完ruby之后 命令行键入<code>ruby -v</code>或者<code>gem -v</code>如果显示版本信息说明安装成功;打开命令行键入<code>gem sourcer</code>会出现ruby包管理器安装源的列表
  删除国外的源添加国内的源，添加源 <code>gem source -a http://gems.ruby-china.com</code>  删除源 <code>gem source -r url</code>(源地址)；
  </li>
  <li>之后在命令行安装 jekyll 和 boundler:<code>gem install jekyll boundler</code>（如果不安装boundler jekyll不能成功安装）
  如何出现错误提示或者没有安装成功请参考官方文档 添加缺少的步骤<a href="https://jekyllrb.com/docs/step-by-step/01-setup/" target="_blank" style="text-decoration:none">https://jekyllrb.com/docs/step-by-step/01-setup/</a>
  </li>
  <li>
    环境搭建好以后就是建站了，可以从github git clone别人的库；也可以自己在本地搭建<br/>
    <code>jekyll new PATH --blank</code>在指定的路径下创建一个新的空白网站；目录下面的文件如下：
    <br/>
    <img src="../createsite.png"/><br/>
    现在还没有建站点 需要<code>cd your have site</code>执行<code>jekyll build</code><br>
    目录下面就多了一个<code>_site</code>文件，这个目录就是你类似于web站点下面的文件

  </li>
</ul>
