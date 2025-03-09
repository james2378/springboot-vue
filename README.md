#### 介绍
java毕业设计，智慧图书管理系统

#### 3000多套系统，需要联系 
抠：3565014707 微：a13424421017

#### 技术栈
后端框架：Spring Boot（核心框架） + MyBatis（ORM）

前端框架：
管理端：Vue.js + ElementUI（现代化SPA）
用户端：LayUI + jQuery（传统多页面应用）
权限控制：自定义注解@APPLoginUser + 拦截器AuthorizationInterceptor
工具集成：百度API（BaiduUtil）、多线程（MyThreadMethod）
构建工具：Maven（pom.xml）

#### 架构模式
分层架构：Controller → Service → DAO 三层结构

模块化设计：字典管理、配置管理、图书管理等功能模块解耦

前后端分离：管理端（Vue.js）和用户端（LayUI）独立部署

#### 核心功能模块
#### 基础功能

字典管理（dictionary包）
功能：统一管理业务字典（如性别、订单状态等）
实现：DictionaryVO（值对象）、DictionaryDao.xml（MyBatis映射）

配置管理（ConfigEntity）
功能：动态管理系统参数（如开关配置、第三方API密钥）

#### 图书管理
核心实体：
tushu（图书信息）
tushuCollection（图书收藏）
tushuOrder（图书订单）

功能点：图书展示、收藏、借阅/购买、订单管理

#### 用户交互
读者管理（duzhe）

功能：读者注册、信息维护、借阅记录

论坛模块（forum）

功能：发帖、回帖、帖子状态管理（dictionaryForumState）

聊天功能（pages/chat）

实现：WebSocket或轮询（需结合代码确认）

#### 支付与扩展
充值功能（recharge）

集成：可能对接支付宝/微信支付（需结合CommonService实现）

文件上传（static/upload）

支持：图片（.jpg）、视频（.mp4）、压缩包（.rar）上传

#### 权限控制
拦截器：AuthorizationInterceptor（校验登录状态）

注解：@APPLoginUser（标记需要登录的接口）

角色管理：隐含在用户管理（users）模块中
