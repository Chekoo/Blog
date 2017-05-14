---
title: 第十七章 部署
date: 2017-04-26 16:57:34
update: 2017-04-26 16:57:34
categories: 编程
tags: [Python, Flask]
---
总的来说，部署遇到了许多坑，而且还有好多坑还没有踩。
去Cocode找了许多教程，才踩了一些坑，但是关于数据库的坑，先留着。
所有的db.session.add()后面都加上db.session.commit()才行。记得，这是狗书的问题！！！
[部署教程]http://cocode.cc/t/flasky-heroku/6589

__每次修改后需要一下命令重新部署下__
` git add * `
` git commit -m "update" `
` git push heroku master `
` heroku run python manage.py deploy`
` heroku restart `


关于其他章节，大部分照着书实践，我也就没做笔记了。
这本书到此为止，希望能给你们带来帮助。
