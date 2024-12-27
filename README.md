# utools_flomo
在[utools](https://u.tools/)中调用[flomo](https://v.flomoapp.com)


需要配置[flomoapp api](https://v.flomoapp.com/mine/?source=incoming_webhook) 这个是付费功能

# 使用

## 配置api

安装插件后 复制flomoapp api 再打开utools,即可识别,配置

## 指令

### 1 `memo`,`uflomo:memo`
**flomo 的最小单位是 memo，一条简短的内容。**

添加一条笔记,

可以包含标签:`#tag`,标签可以是多级的: `#tag/sub_tag`.标签后需要跟空格才能写正文,不然会算到标签里.

在`memo`指令中出现的标签会被记录,下次再使用`memo`指令时可以进行选择.

记录到memo会记录在本地目录中.这个插件不支持查看历史memo.

不支持图片

### 2 `uflomo:管理本地标签`, `uflomo:grlibfdibnqm`, `uflomo:custom_local_tag`
编辑和删除本地的标签,不会影响到flomo中的标签


### 3 `uflomo:打开本地文件目录`, `uflomo:dakdbfdiwfjmmulu`, `uflomo:open_local_dir`
打开本地文件目录


本插件唯一的网络请求是调用flomoapp api.除此之外没有其他网络请求.

所有memo都存储在用户本地.

flomoapp api和tag信息存储在[utools.db](https://u.tools/docs/developer/api-reference/db/local-db.html)中,
可以在个人中心我的数据中查看和删除.
