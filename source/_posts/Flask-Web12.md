---
title: 第十二章 关注者
date: 2017-04-26 16:57:22
update: 2017-04-26 16:57:22
categories: 编程
tags: [Python, Flask]
---
# 关注者

解决多对多：添加第三张表，为关联表。

db.backref()参数并不是指定这两个关系之间的引用关系，而是回引Follow模型。
回引的lazy参数指定为joined.这个lazy模式可以实现立即从联结查询中加载相关对象。
如果选为select，那么首次访问follower和followed属性时才会加载相应的用户，而且每个属性都需要一个单独的查询，这就意味着获取全部被关注用户时需要增加100次额外的数据库查询。

联结操作用到两个或更多的数据表，在其中查找满足指定条件的记录组合，再把记录组合插入一个临时表中，这个临时表就是联结查询的结果。