## 修改说明
本修改版本对ThinkCMFX核心文件有改动，如果你已经在使用ThinkCMFX，请核对好之后再进行覆盖。
2016.4.22
* 添加阿里云OSS存储方式

> 添加的文件
> simplewind/Core/Library/Think/Upload/Driver目录下添加了Aliyun.class.php及Aliyun目录，主要为阿里云OSS的THINKPHP驱动文件。

> 修改的文件
> 1. admin/themes/simplebootx/Admin/Storage/index.html
> 2. application/Admin/Controller/StorageController.class.php
> 3. application/Admin/Lang/zh-cn/storage.php
> 4. application/Admin/Lang/en-us/storage.php


以下为THINKCMF官方信息

## README
ThinkCMF是一款基于PHP+MYSQL开发的中文内容管理框架。ThinkCMF提出灵活的应用机制，框架自身提供基础的管理功能，而开发者可以根据自身的需求以应用的形式进行扩展。每个应用都能独立的完成自己的任务，也可通过系统调用其他应用进行协同工作。在这种运行机制下，开发商场应用的用户无需关心开发SNS应用时如何工作的，但他们之间又可通过系统本身进行协调，大大的降低了开发成本和沟通成本。
官网:http://www.thinkcmf.com
文档:http://www.thinkcmf.com/document

## UPDATE
X2.1.0
* 修复前台导航缓存问题
* 修复个人中心mysql5.7下保存失败
* 文章评论插件化
* 增加系统评论插件
* 修复simplebootx模板config文件变量不对应
* 优化用户激活流程，防止已激活用户和被禁用用户两次发送激活邮件
* 更正数据库前台导航分类active注释
* 修复手机模板开启时跳转页面模板路径判断错误
* 修复重置密码后，重置密码链接仍可打开问题
* 增加后台评论管理查看原文功能
* 增强后台登录接口安全性
* 修复前台分页当前页选中问题
* 增加全局路由,强化URL美化功能
* 修复导航添加时导航分类选择问题

祝新年愉快，合家欢乐！

X2.0.0
* 更改HomeBaseController.class.php文件名为HomebaseController.class.php
* 移动Common里的Portal model到Portal下；
* 规范前后台模板目录，themes ,admin/themes；
* **注意以上升级，有助于您升级到最新版本**
* 增加对PHP7的支持
* 增强验证码易识别性；
* 增加后台从菜单栏点击立即刷新选项卡功能；
* 增加前台模板多语言，插件多语言；
* 增加后台多语言基础功能，语言包稍后升级完善；
* 优化后台模板文件；
* 优化后台登录界面；
* 优化前台登录、注册、找回密码界面；
* 优化common.js,frontend.js,规范一系列js-xxx-xxx命名和功能实现；
* 优化文章编辑页布局和css；
* 修复模板中U方法大小写错误；
* 修复ip获取，防止代理访问；
* 修复success,error跳转页无手机模板问题；
* 升级百度编辑器；
* 去除前台各处同意网站条款；
* 去除文章访问次数统计的ip限制；

X1.6.1
* 修复登录时仍然可以打开登录和注册界面
* 修复后台文章分类列表，点添加子类到添加分类界面父级分类选择错误
* 修复后台文章分类模板修复后不更新问题
* 修复编辑器里图片上传， 在文件存储选择七牛时，图片title,alt属性不对
* 增加对php格式模板文件的支持
* 优化sp_get_menu方法,id为空时，默认为主菜单
* 修复后台模板缺失</head>问题
* 修复Portal应用下文章，页面，和分类不存在时，无404状态码
* 增加对模板继承标签tc_extend的支持
* 优化会员的拉黑起用功能，改为实时验证
* 增加url模式更改后出现不能访问问题的提示和解决方法
* 修复文章，幻灯片添加重复提交问题

X1.6.0
* 增加静态缓存
* 增加form提交状态判断，防止连续提交
* 增加后台被禁用角色和用户登录提示
* 增加文章可以添加到多个分类    
* 增加管理员停用启用功能
* 增加文章来源版权申明 
* 增加文章内容页面二维码
* 增加验证码统一判断方法
* 优化验证码自动刷新     
* 优化后台样式
* 修复邮件配置更新时，不会立刻更新问题
* 修复后台手动新加的菜单时没有同步到auth_rule表
* 修复角色禁止后登陆报错
* 修复角色无法删除问题
* 修复后台视频上传出错！请注意上传大小限制,php.ini post_max_size,upload_max_filesize
* 修复后台菜单过多不显示
* 修复后台管理登录可能会被暴力破解
* 修复后台菜单列表层级问题
* 修复启用后被删除的插件执行报错

X1.5.0
* 增加插件机制
* 增加编辑器附件上传功能
* 核心升级至thinkphp 3.2.3，必须开启php_pdo_mysql扩展
* 优化系统权限管理，增加auth+rbac混合认证模式
* 增加文件存储扩展支持，默认支持本地和七牛云存储
* 增加手机模板支持
* 增加手机模板侦测后台开启关闭功能，默认关闭手机模板侦测
* 增加MUI手机开发框架
* 增加评论时间间隔设置
* 增加视频插入
* 增加去除模板文件里面的html空格与换行
* 增加后台管理员列表分页
* 增加文章页上一篇、下一篇功能
* 优化菜单管理方式，采用增加文件方式菜单管理，方便程序升级
* 优化导航鼠标划过下拉菜单
* 优化管理员信息编辑,增加字段过滤
* 优化非后台入口登录跳转到首页
* 修复simplebootx搜索链接错误
* 修复ucenter各种问题
* 修复后台邮件发件人无法设置
* 修复入口文件SITE_PATH常量部分服务器异常
* 修复sae头像裁剪
* 修复分类编辑时层级出错
* 修复备份还原数据为空
* 统一所有模块模板路径分割符为/
* 删除thinkphp Vendor目录第三方类库
* 移除SendMail方法
* 替换scandir方法为sp_scan_dir
* 统一SAE判断方法
* 统一ajaxReturn为thinkphp 3.2.*以后用法，如果一直用thinkphp  3.0以前的用法，扩展时注意用sp_ajax_return()做一下升级

注：后台模板分割符已经统一为/，原来的类似Admin/Main.index.html文件已经改为Admin/Main/index.html请后台开发时注意
ThinkCMF全体贡献者祝大家2015年大吉大利，开心幸福！《给你一个吻》


X1.3.0
* 统一Action为Controller
* 增加文章搜索功能
* 增加前台编辑器
* 增加模板常量__STATICS__
* 增加最后评论时间写入
* 修复leuu bug 
* CommonModel _before_write 数据过滤bug
* 后台评论管理,默认所有评论
* 文章分类path更新优化
* simplebootx模板文章页css样式优化
* 修复分页类bug
* 后台文章编辑所有文章链接错误
* 修复bug#4验证码不显示
* 优化bug#3页面使用LEUU函数后每个页面都查询
* 优化公共模型的调用方法，以兼容php5.3.0-5.3.2
* 修复sp_sql_posts_bycatid和sp_sql_posts_paged_bycatid两个方法where语句问题
* 修复bluesky主题分页样式问题
* 修复文章推荐，置顶bug

X1.2.0
* url美化
* 特殊用户名过滤
* 增加推荐，置顶功能
* 幻灯片隐藏显示功能
* 广告隐藏显示功能
* 友情链接隐藏显示功能
* 评论计数

X1.1.0

全新的ThinkPHP 3.2.2架构，使用php命名空间，让开发快起来吧！

* 统一Member应用为User,合并前台会员和后台管理员
* 完善用户中心，会员登录注册
* 增加编辑头像，绑定账号，我的评论，我的收藏
* 增加文章点赞，收藏，查看功能，可与其它应用共用
* 增强文章评论功能，方便多应用共用
* 优化留言功能，增强安全性
* 优化前台模板，增加多个实用组件，方便以后复用
* 增加后台风格切换功能；
* 增加后台风格bluesky
* 优化后台菜单使用方式
* 优化数据库中一些不规范字段
* 增加前台标签库TagLibHome，统一include标签为tc_include

X1.0.0

全新的ThinkPHP 3.2.2架构，使用php命名空间，让开发快起来吧！

* 统一前后台UI框架为simpleboot(bootstrap 2.3.2 ThinkCMF优化版)
* 集成Ucenter
* 增加文章评论功能
* 增加留言功能
* 全面支持SAE云平台
* 增加文章内分页功能
* 升级后台编辑器到Ueditor最新版本
* 优化后台ajax提交，未登陆时自动退出
* 优化后台所有文章按发布时间递减排序
* 修复后台密码会偶然不对的错误
* 修复SAE，linux下类库加载失败
* 修复ueditor chrome模板功能bug
* 修复文件上传bug

X1.0.0 alpha2

* 修复SAE，linux下类库加载失败
* 修复ueditor chrome模板功能bug
* 修复文件上传bug


X1.0.0 alpha

全新的ThinkPHP 3.2.2架构，使用php命名空间，让开发快起来吧！
* 集成Ucenter
* 增加文章评论功能
* 增加留言功能
* 全面支持SAE云平台
* 增加文章内分页功能
* 升级后台编辑器到Ueditor最新版本
* 优化后台ajax提交，未登陆时自动退出
* 优化后台所有文章按发布时间递减排序
* 修复后台密码会偶然不对的错误


## INSTALL
安装请执行http://yourdomain/install/index.php

安装完成后请删除或改名install/index.php

## ThinkCMF 免责声明
  1、利用 ThinkCMF 构建的网站的任何信息内容以及导致的任何版权纠纷和法律争议及后果，ThinkCMF 官方不承担任何责任。
  
  2、您一旦安装使用ThinkCMF，即被视为完全理解并接受本协议的各项条款，在享有上述条款授予的权力的同时，受到相关的约束和限制。
 
## ThinkCMF 使用建议

请在您的网站首页加上ThinkCMF相关链接，O(∩_∩)O~ ！
  
## 捐赠ThinkCMF
http://www.thinkcmf.com/donate/index.html
  
您的每一份帮助都将支持ThinkCMF做的更好，走的更远！
  
  
ThinkCMF 正在为你开放更多....