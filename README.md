# 基于 Vue 和 SpringBoot 的医院门诊预约挂号系统

## 软件简介

本软件是《基于 Vue 的医院门诊预约挂号管理系统》，主要包含数据中心、科室医生模块、预约挂号模块、医院时政这四大模块。

预约挂号系统采用了**基于角色的访问控制**，角色和菜单关联，一个角色可以配置多个菜单权限；然后再将用户和角色关联，一位用户可以赋予多个角色。这样用户就可以根据角色拿到该有的菜单权限，更方便医院管理人员进行权限管控。

![输入图片说明](image/39.png)

患者去医院都是排队挂号，但随着科技的发展，预约挂号脱颖而出，医院门诊预约挂号管理系统操作简单明了与互联网紧密相关、适应时代发展的潮流。通过医院门诊预约挂号系统，可以极大的方便挂号者进行预约挂号，同事还能是医院更加合理的安排排号者就医并提供更优质的医疗服务。既能适当解决当前中国面临的医院门诊挂号排队时间长、挂号环境乱的问题，又能方便广大预约者挂号预约自己相对满意的医生和专家。

本系统前端采用了国内流行的 Vue 技术，采用了 View UI 作为组件库；后端采用 Java 语言编写，采用 SpringBoot 整合 MybatisPlus，采用 maven 构建项目，采用 Mysql 数据库，使用了 Redis 用于缓存加密的用户临时数据。

《医院门诊预约挂号管理系统》的登陆界面如下图所示。

![输入图片说明](image/2.png)

《医院门诊预约挂号管理系统》的主页如下图所示。

![输入图片说明](image/3.png)

## 技术栈

### 前端

Vue：Vue 是构建前端界面的核心框架，本系统采用 2.6.14 版本。

View UI：基于 Vue.js2.0 的组件库，本系统采用 4.7.0 版本。

### 后端

Spring Boot：构建系统核心逻辑的后端框架，本系统采用 2.7.0 版本。

MyBatis / MyBatis Plus：后端连接数据库的框架，本系统采用 3.5.2 版本。

### 数据库

MySQL：本项目的主数据库，本系统采用 8.0.29 版本。

Redis：本系统采用基于 Windows 版本的 Redis，用于图形验证码和用户菜单权限的临时存储，采用了 5.0.14 版本。

### 开发环境

VsCode：项目前端的开发工具，使用版本为 1.68.0。

IntelliJ IDEA ：项目后端的开发工具，使用版本为 2021.3.2。

Jdk：Java 的开发环境，使用版本为 17.0.3.1。

Maven：后端项目的打包工具，使用版本为 3.6.2。

NodeJs：前端项目的开发环境，使用版本为 16.13.0。

![输入图片说明](image/1.png)

## 开发模板

《基于 Vue 和 SpringBoot 的假日旅社管理系统》是基于《基于 Vue 和 SpringBoot 的通用管理系统》（<https://gitee.com/yyzwz/template>）开发的，模板包含了**登陆注册、用户管理、部门管理、文件管理、权限管理、日志管理、个人中心、数据字典和代码生成**这九个功能模块，另外还有两张样例数据表和五张样例数据图，是一个很好的前后端分离开发模板，开发者可以在这个模板上进行二次开发，只需要实现需求方的业务逻辑，即可快速成型甲方的业务需求。

模板采用了**基于角色的访问控制**，角色和菜单关联，一个角色可以配置多个菜单权限；然后再将用户和角色关联，一位用户可以赋予多个角色。这样用户就可以根据角色拿到该有的菜单权限，更方便管理者进行权限管控。

模板还**封装了文件管理功能**，在其他模块如若要实现图片/文件上传预览时，前端只需导入现成的 Vue 组件即可实现（使用 viewerjs 依赖实现），后端只需定义 String 类型的实体类变量即可，无需再去研究文件上传预览的相关功能，简化了开发者的工作量。

模板还自带**基于 beetl 代码生成器**功能，开发者只需要输入类名（如 Student）和类备注（如学生），运行 main 函数即可自动生成后端的所有 MVC 结构代码，无需开发增删改查的 API 接口。对于前端，开发者只需输入后端实体类的完整路径，利用 Java 的反射原理，拿到后端实体类的字段，即可自动生成前端所有代码，生成的模块代码包含基础的增删改查功能，简化开发者的工作量。

## 项目背景

预约挂号，挂专家号更是“一号难求”,这是当前许多大型医院的普遍现象。预约挂号是各地近年来开展的一项便民就医服务，旨在缩短看病流程，节约患者时间。这种预约挂号大多通过医疗机构提供的电话或者网络进行，基本上是免费或者只收取很少的手续费。由于预约挂号需要事先登记患者的信息，并且可以减少在医院挂号窗口排队等待之苦，因此它一定程度上也有利于改善就医环境，促进“实名制”的推行，受到了不少患者的肯定和欢迎。

自从有了医生这个职业，医生预约就一直存在。从古代君王豪吏，富贾商户到如今医生预约走进社会各基层，走进千家万户，医生预约经历了从特权到普遍，滞后到高速发展的不同时期。这是近几年新兴的挂号方式。通过网络可以完成在医院或者在电话预约中完整的服务，方便快捷，加以医生门诊预约系统强大的系统管理功能，使医院方面在经营管理方面拥有了新的发展方向。

## 项目意义

网络挂号更加方便快捷，只需注册账号进行登录，便可以在家中或者其他任何地方通过电脑进行预约挂号操作，可以根据需要查询科室、医生的相关信息，用户也可以随时根据需要修改自己的资料，轻松地预先了解医院以及医生的情况，来选定医生，通过简便的操作，完成挂号预约方便快捷；网络挂号有利于缓解医院窗口挂号排队拥挤的现状。患者大量扎堆在清晨排队挂号，其没有计划的挂号导致等候就诊时间较长，致使大量患者滞留在医院，耽误患者治疗时间。而且财务窗口人力紧张，压力大，不利于服务质量的提高。针对这一问题，医院预约挂号系统有利于减少患者在候诊区无效的等待时间，减轻患者和家属的挂号难度，在一定程度上缓解改善了挂号窗口的紧张状。

根据对预约挂号的平台需求进行分析，将系统分为前台和后台。前台主要由用户使用，主要功能包括：注册与登录、科室医生的浏览/检索、预约、新闻展示、留言板留言等等。后台则由管理员使用，主要功能包括：科室医生的信息管理、预约订单管理、患者信息管理、留言板管理等等。

## 系统预览

### 登陆界面

进入系统，首先看到登入界面，用户可以输入自己的账号、密码，进行登入操作。

超级管理员的登陆账号为 admin，密码为 123456。

测试患者的登陆账号为 user1，密码为 123456。

登陆分为账户密码登录和手机短信登陆两种模式。

手机短信登陆因为需要付费，所以暂不开放短信登陆的功能，只是做了一个静态界面。

图片验证码为随机的 4 位阿拉伯数字，用户输入图片中的四位验证码，即可完成登陆。

![输入图片说明](image/2.png)

![输入图片说明](image/38.png)

用户登陆功能，系统首先会效验验证码，验证码有效期为 60 秒，如果超过有效期，系统会提示需要重新登陆，如下图所示：

![输入图片说明](image/4.png)

如果遇到看不清楚的验证码，可以点击验证码图片可以完成刷新。

为了保证系统安全，不被频繁请求访问，如果用户输入错误的验证码，系统将提示“图形验证码输入错误”，不给与登陆，用户需要重新输入验证码。

![输入图片说明](image/5.png)

当输入的验证码正确后，系统第二步会验证用户输入的账号密码，若账号密码输入错误，系统给与提示，告知密码不正确。

![输入图片说明](image/6.png)

当用户输入的账号密码、图形验证码都正确后，系统给与登陆，进入到系统首页，如下图所示：

![输入图片说明](image/3.png)

### 注册界面

系统开放了用户注册的功能，患者可以自助注册患者账户，进入系统后，点击登陆按钮上方的“注册账号”绿色超链接，跳转到注册界面。

![输入图片说明](image/7.png)

注册界面如下图所示，用户需要输入自己的手机号、用户名、密码和图形验证码，完成患者用户注册。然后使用注册时填入的手机号和密码，完成系统登陆。

![输入图片说明](image/8.png)

### 科室管理模块

管理员登陆系统后，可以进入科室管理模块，查询科室档案的详细数据，如下图所示：

![输入图片说明](image/9.png)

用户可以浏览医院新闻资讯等信息，并能查询科室、医生等相关信息。

科室的信息包括：

- 科室名称
- 科室代码
- 科室人数
- 主任医师人数
- 科室介绍
- 责任医师
- 备注

管理员可以单击顶部的“添加”按钮，进入科室的添加界面，后输入科室的名称、科室代码、科室介绍、科室成立日期、责任医师、备注，完成科室的添加。

![输入图片说明](image/10.png)

管理员可以点击每一行的“编辑”按钮，进入科室编辑模块，如下图所示：

![输入图片说明](image/11.png)

进入科室编辑模块后，完成现有数据的修改，点击“提交并保存”按钮即可完成编辑操作。

![输入图片说明](image/12.png)

同理，点击每一行科室的“删除”按钮，即可完成对科室的删除功能。

![输入图片说明](image/13.png)

管理员可以点击顶部的“导出”按钮，完成科室的 Excel 导出功能。

导出结果如下图所示：

![输入图片说明](image/14.png)

医院科室的数据库设计如下图所示：

![输入图片说明](image/15.png)

### 医生管理模块

管理员登陆系统后，可以进入医生管理模块，查询医生档案的详细数据，如下图所示：

![输入图片说明](image/16.png)

医生的信息包括

- 医生姓名

- 医生年龄

- 学历学位

- 开始工作时间

- 毕业院校

- 职称

- 专业

- 所属科室

- 医生介绍

医生档案的增加、编辑、删除、导出操作步骤同科室模块。

可以根据科室查询医生，如在科室搜索框内输入“口腔”，点击搜索按钮，即可查询口腔科的医生列表，如下图所示：

![输入图片说明](image/17.png)

医生的数据库设计如下图所示：

![输入图片说明](image/18.png)

### 医生放号模块

为了模拟真实的预约挂号流程，本系统设计了医生放号模块。

管理员进入医生放号模块，界面如下图所示：

![输入图片说明](image/19.png)

点击每一行医生的“放号”按钮，系统弹出放号交互弹框，如下图所示：

![输入图片说明](image/20.png)

管理员需要填入放号日期、放号时段、放号个数，完成放号功能。

如填入放号日期为“2022-09-12”，放号时段为上午，放号个数为 10 个，点击“确认放号”按钮，即可完成对罗文文医生的放号操作。

管理员可点击每一行医生的“查询”按钮，完成对放号结果的查询，如下图所示：

![输入图片说明](image/21.png)

医生号源的数据库设计如下图所示：

![输入图片说明](image/22.png)

### 预约挂号模块

患者账号登陆系统后，可以进入到预约挂号模块，如下图所示：

![输入图片说明](image/23.png)

在预约挂号模块中，可以查询需要挂号的医生。

可以根据科室查询，可以筛选是否今日的号，可以搜索医生的姓名、职称，该搜索功能在左上角顶部的搜索框实现。

如筛选了口腔科的科室，点击搜索按钮，即可完成口腔科医生的搜索，如下图所示：

![输入图片说明](image/24.png)

患者点击每一行医生的红色的“挂号”按钮，系统弹出挂号弹框，患者可以查询该为医生的号源，如下图所示：

![输入图片说明](image/25.png)

点击每一行的橙色“挂号”按钮，系统弹出再次确认弹框。

![输入图片说明](image/26.png)

点击“确定”按钮，即可完成预约挂号操作。

挂号的数据库设计如下图所示：

![输入图片说明](image/27.png)

### 我的挂号模块

患者登陆系统后，可以进入我的挂号模块。

该模块用于展示个人的挂号详情，界面如下图所示：

![输入图片说明](image/28.png)

患者可以点击每一行红色的“取消点我”按钮，取消该次预约挂号，取消后号源恢复为未挂号状态。

患者可以点击红色的“付款”按钮，完成预约订单的付款功能。付款仅为模拟，支付宝/微信/银联支付必须要企业认证，个人没权限测试开发支付功能。

患者预约到医生的号后，可在我的订单模块模拟付款。付款后预约订单状态为已付款。

患者点击“付款”后，系统将弹出二次确认弹框，如下图所示：

![输入图片说明](image/29.png)

### 用户留言模块

医院的预约挂号标准化流程，一定会存在有需要改进的点，或者现有功能不能被患者理解学会，所以需要设计留言板功能，实现患者和医院的信息交互功能。

患者进入到用户留言模块，界面如下图所示：

![输入图片说明](image/30.png)

患者可点击顶部蓝色的“添加”按钮，打开添加留言弹框，如下图所示。

![输入图片说明](image/31.png)

患者点击弹框底部的“确认留言”按钮后，完成留言操作。

留言完成后界面如下图所示：

![输入图片说明](image/32.png)

管理员可以对留言进行回复操作，如下图所示。

![输入图片说明](image/33.png)

回复成功后，管理员可以双击每一条评论行，查看该条评论的回复列表，如下图所示：

![输入图片说明](image/34.png)

### 医院新闻模块

管理员可以进入医院新闻模块，界面如下图所示：

![输入图片说明](image/35.png)

新闻的信息包括：

- 新闻名称

- 新闻描述

- 图片

- 新闻时效

- 是否公开

- 是否置顶

支持对医院的新闻进行添加、编辑、删除、公开、置顶，操作过程同科室管理模块。

系统采用了 ViewerJs 依赖，对指定 URL 的图片进行预览。

系统采用了 View UI 组件库，在表格内嵌了 Switch 开关组件。

普通患者只能进入的医院新闻留言模块，只保留了新闻的查看功能，界面如下图所示：

![输入图片说明](image/36.png)

医院新闻的数据库设计如下图所示：

![输入图片说明](image/37.png)

## 免责声明

- 本项目开源，仅供个人学习使用，遵循 GPL-3.0 开源协议，**转发 / 商用授权请联系作者，否则后果自负**。
- 作者拥有本软件构建后的应用系统全部内容所有权及独立的知识产权（**软件著作权登记号：2022SR0369372**）。
- 如有问题，欢迎在仓库 Issue 留言，看到后会第一时间回复。相关意见会酌情考虑，但没有一定被采纳的承诺或保证。

下载本系统代码的用户，**必须同意以下内容，否则请勿下载**！

1. 出于自愿而使用/开发本软件，了解使用本软件的风险，且同意自己承担使用本软件的风险。
2. 利用本软件构建的网站的任何信息内容以及导致的任何版权纠纷和法律争议及后果和作者无关，作者对此不承担任何责任。
3. 在任何情况下，对于因使用或无法使用本软件而导致的任何难以合理预估的损失（包括但不仅限于商业利润损失、业务中断与业务信息丢失），作者概不承担任何责任。
4. 必须了解使用本软件的风险，作者不承诺提供一对一的技术支持、使用担保，也不承担任何因本软件而产生的难以预料的问题的相关责任。
