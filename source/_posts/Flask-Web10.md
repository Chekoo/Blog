---
title: 第十章 用户资料
date: 2017-04-26 16:57:11
update: 2017-04-26 16:57:11
categories: 编程
tags: [Python, Flask]
---
# 用户资料
WTForms对HTML表单控件< select >进行SelectField进行包装，实现下拉列表，用来在这个表单中选择用户角色。<be>
SelectField 实例必须在 __choices__ 属性中设置各选项

## 用户头像
Gravatar是一个行业领先的头像服务，能把头像和电子邮件关联起来。
生成的头像URL添加到User模型。


