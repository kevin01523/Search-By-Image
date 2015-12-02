Search-By-Image
===============

Search By Image | 以图搜图

一个以图搜图的脚本。通过该脚本，你可以快速地搜索图片。

备用下载地址：
> https://greasyfork.org/scripts/2998-search-by-image
> 
> http://ext.ccloli.com/search-by-image/search-by-image.user.js

使用方法：
> * 搜索图片：按住快捷键（默认设置为 Ctrl 键），同时在图片上点击鼠标右键，在菜单中选择欲使用的搜索引擎
> 
> * 上传搜索：按住快捷键（默认设置为 Ctrl 键），同时在非图片上点击鼠标右键，在菜单中上传图片后选择欲使用的搜索引擎（1.4 版本）<br>传输过程中点击进度条取消上传，上传后图片临时保存于中转服务器上供搜索引擎抓取<br>上传方式包括以下几种（仅支持单个文件）
> 
> > * 点击“上传图片并搜索”并选择文件
> > 
> > * 拖拽文件至菜单内
> > 
> > * 按下 Ctrl + V 粘贴剪贴板内图片（暂不支持 Firefox，原因不明）
> > 
> > * 另外搜索 base64 形式图片也需要上传
> 
> * 设置脚本：按住快捷键（默认设置为 Ctrl 键），同时点击鼠标右键，在菜单中选择“Setting”打开设置界面<br>或在用户脚本命令中选择“Search By Image Setting”打开设置界面<br>在设置页面中可以更改、添加、删除搜索引擎，进行“多搜”及快捷键的配置和重置设置
> 
> > * 更改搜索引擎：“名称”栏指定搜索引擎名称，“地址”栏指定搜索引擎调用地图（图片地址以 {%s} 代替）
> > 
> > * 添加搜索引擎：点击“Add Item”按钮可添加搜索引擎
> > 
> > * 删除搜索引擎：点击搜索引擎右侧的“×”可删除该搜索引擎
> > 
> > * 设置多搜　　：勾选“多搜”复选框并保存后，在搜索图片时点击“All”将打开所有勾选“多搜”的搜索引擎
> > 
> > * 更改快捷键　：在左下角的“HotKey”处可修改呼出搜索菜单的快捷键
> > 
> > * 重置设置　　：点击“Reset”按钮可重置所有设置（不可逆）
> > 
> > * 保存设置　　：点击“Save”按钮可保存设置
> 
> * 修改中转服务器：在脚本内 47 行（可能有变动）找到 server_url，按需进行修改（更新后也需重新设置），相关介绍已列在脚本中
> 
> 各界面的使用请参考下面的预览图

默认支持的网站：
> * Google
> * 百度识图
> * 百度图片
> * Bing
> * TinEye
> * Яндекс (Yandex)
> * 搜狗
> * 360
> * SauceNAO
> * IQDB
> * 3D IQDB

内部测试：
> * 864907600cc (ccloli)
> * 文科 (wenketel)

本脚本基于 GPLv3 协议开源 http://www.gnu.org/licenses/gpl.html‎

![搜索菜单](https://cloud.githubusercontent.com/assets/8115912/3623778/b6d76498-0e53-11e4-96a0-09488c053e44.png)
![设置界面](https://cloud.githubusercontent.com/assets/8115912/3623779/b734b490-0e53-11e4-9250-66707699db6e.png)

追加说明：
> 首先，这个脚本只能搜索 img 标签的图片，对 css background-image 什么的话，呵呵 = =
> 
> 其次，由于方便设计，估计有很多网站设计图片翻页或者图片动态效果时，会在图片上方加个透明的层，这样也是获取不到图片的 = =
> 
> 另外，搜索贴吧内图片时，如果出现搜索的 url 为 base64 的情况，请看此贴：http://tieba.baidu.com/p/3145502558

更新历史： 
> 2015.12.02 1.4.10 Fixed GreasyFork feedback [#6806](https://greasyfork.org/en/forum/discussion/6806/x) (not working on old Firefox), update most of default search engines url to HTTPS
> 
> 2015.08.15 1.4.9 添加并没有什么用的多语言支持，添加并没有什么用的自定义上传服务器设定，修复 1.4.6 修复菜单栏错位导致菜单栏错位的问题
> 
> 2015.05.01 1.4.8 修复百度图片搜索不可用的问题（See issue #3 ）
> 
> 2015.04.06 1.4.7 修复在部分可视化编辑器（eg. MDN WYSIWYG editor）中出现遗留菜单的 bug（Thanks to lychichem, see issue http://tieba.baidu.com/p/3682475061 ）
> 
> 2015.04.05 1.4.6 修复当 body 存在 margin 时菜单栏错位的问题，修复上一版本鼠标经过样式并未生效的问题，Яндекс (Yandex) 的默认名称改为 Yandex
> 
> 2014.09.05 1.4.5 添加鼠标经过选项之样式（我承认我懒了 OTL）
> 
> 2014.08.14 1.4.4 修复未呼出面板时仍进行关闭面板的操作，尝试性修复 GM 2.x 下 GM_registerMenuCommand 冲突
> 
> 2014.07.26 1.4.3 添加中转上传服务器（Thanks to Retaker），修改上传服务器设置方式，尝试性修复 Firefox 无法粘贴上传的问题
> 
> 2014.07.18 1.4.2 修复在非图片上呼出搜索菜单时无法点击设置按钮的问题
> 
> 2014.07.06 1.4.1.1 修复无法上传的 bug
> 
> 2014.07.06 1.4.1 去除弹窗通知（在 Firefox 下可能会频繁弹出），添加其他中转上传服务器（需手动修改脚本）
> 
> 2014.07.06 1.4 支持上传图片搜索，支持 base64 图片搜索（中转上传）
> 
> 2014.07.05 1.3.8 规范语法，更改多搜时搜索引擎打开顺序，添加 base64 地址判断并拒绝搜索 base64 形式的图片（因为已知搜索引擎均不支持）
> 
> 2014.07.04 1.3.7 尝试性修复 Chrome Tampermonkey 下与其他监听鼠标操作的脚本的冲突问题
> 
> 2014.07.04 1.3.6 添加 360 和 3D IQDB，修复某标签页修改设置后在其他标签页设置不更新的问题（该版本会覆盖设置）
> 
> 2014.07.04 1.3.5 修改错误的标题
> 
> 2014.07.04 1.3.4 脚本正式发布
> 
> 2014.07.04 1.3.3 修复搜索菜单定位不准确的问题
> 
> 2014.07.04 1.3.2 修复一些 bug
> 
> 2014.07.04 1.3.1 修复因未填写搜索引擎而出现空白选项的问题
> 
> 2014.07.03 1.3 添加设置菜单
> 
> 2014.07.03 1.2.1 修复一些 bug
> 
> 2014.07.03 1.2 添加快捷键设置（需在脚本内修改）
> 
> 2014.07.03 1.1 添加搜索菜单
> 
> 2014.07.03 1.0 脚本开始编写，并完成基本功能