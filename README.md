# WeiboSpider
**@ Zeng Ying, Pan Ziyang, Zhong Shanshan, Huang Zhishan, Yu Yixia, Chen Lehua**

<br>

## 前言：
> 微博用户拥有唯一的用户id，每一条微博也有唯一的博文id。本项目旨在利用[移动端微博网页](http://m.weibo.cn)，获取公开微博的相关数据。并进行相关的数据分析和可视化工作。

<br>

## 目录
0. [前言](##前言)
1. [模块介绍](##模块介绍)
2. [如何安装python依赖？](##如何安装python依赖)

<br>

## 模块介绍：
1. `search_uid.py`, 用于获取指定query的用户id，返回用户相关信息的字典
2. `get_wbid.py`,用于获得用户id下的微博id（来自用户主页）
3. `relationship.py`,用于获取用户之间的转发关系，以[用户id，用户微博id，粉丝id，粉丝微博id]存储
4. `get_topic.py`用于获取实时热搜主题以及相应热度，提供两种方式存储：csv, json.具体格式[index, topic, score].生成文件命名为 **爬取热搜时间.csv /.json.**

## 如何安装python依赖？
我们提供了专门的依赖文档供您一键安装所有python依赖，只需使用
`pip install -r requirements.txt`
就能完成python库的依赖安装