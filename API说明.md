tips: user-id is yige yonghu id d header
# API说明
## 登录注册模块
### /sign/in
登陆，直接用学号登陆，数据由管理员直接导入数据库

+ 学号
+ 密码
+ 验证码

### /sign/up
使用学号注册

+ 学号
+ 密码
+ 验证码

## 用户管理模块
个人信息接口

### /person/:id
+ get：获取用户信息
+ post：修改用户信息

## 公告模块
### /notification
+ get：获取所有公告
+ post：上传新的公告

### /notification/:id
+ get：获取单个公告
+ post：更新单个公告

## 论坛管理模块
论坛板块的接口。  

由id不同指代不同的论坛板块：如工作、读研、出国。    
id由一个统一的配置文件进行设置（前后端均使用该文件）。   

标签的设置与上同理。

### /forum/:id/post
+ get：获取该板块下所有帖子
+ post：上传新的帖子

### /forum/:id/tag
+ get：获取该板块下所有标签
+ post：修改板块所属标签

### /forum/:id/post/:id
+ get：该板块下某个帖子的相关信息
+ post：更新帖子信息

### /forum/:id/post/:id/tag
+ get：该板块下某个帖子的标签
+ post：更新帖子标签

### /forum/:id/post/:id/comment
+ get：获取该帖子下所有回复
+ post：上传新的回复

### /forum/:id/post/:id/comment/:id
+ get：该帖子下某个回复的相关信息
+ post：更新回复信息


## admin模块（暂时不管）
- 用户管理
	- 增删改查
- 公告管理
	- 增删改查
- 分享管理
	- 增删改查
- 提问管理
	- 增删改查
- 评论管理（功能暂时不实现）
	- 增删改查
