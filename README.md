# UCES（原名PicRoll）
辅导员考核系统 University Counsellor Examination System

## 项目介绍 Introduction

- 平台辅助老师进行辅导员考核，提供按条件查询学生信息、滚动学生照片抽取考查学生并异步更新页面显示其信息等功能
- 采用J2EE架构（JSP + Servlet + JDBC），系统部署在Tomcat上

- The platform is used to assist teachers to conduct counselor assessment, to provide conditions for the queried student information, roll student photo and asynchronously update pages display.
- Using J2EE architecture (JSP + Servlet + JDBC), the system deployed in Tomcat

## 前端介绍 User Interface

<p align="center">
<img src="http://i.imgur.com/TZgqSi0.png"/>
<div align="center">
Fig. 首页 | HomePage
</div>
</p>

 - 由于界面包含学校信息及较多个人信息，故在这里不展示前端其他界面。
 - Ajax+json 实现学生信息查询及异步显示
 - js 中借助计时器图片的滚动、暂停滚动及随机抽取显示
 
 - As the interface contains school information and more personal information, so we do not show the other front-end interface.
 - Ajax+json implements student information query and display asynchronously
 - In js we used timer to roll pictures, pause rolling and extract display randomly
 
## 后台介绍 Back-end

- 由 Servlet 处理表单提交、页面导航、已封装数据库操作函数的调用、json字符串的封装等
- 通过 JDBC 访问和操作 MySQL 数据库
- 使用 DAO 设计模式来封装数据库持久层的操作

- Using Servlet to deal with form submission, page navigation, encapsulated database operation function called, json string encapsulation, etc.
- Access and manipulate MySQL databases via JDBC
- Use the DAO design pattern to encapsulate the operation of the database persistence layer
