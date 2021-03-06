# ChargerSharingSystem
## 课程期末作业 模拟共享充电宝系统 Spring MVC + Spring + Mybatis
- 要求如下
> ##### 共享充电宝平台平台包括以下基本功能模块：
> * 前台：查看充电宝、借还、订单管理
> * 充电宝查看模块让用户根据手机定位查找最进行充电宝投放点，查询投放点可借用的充电宝数量
> * 租借模块让用户实现对充电宝的借用与归还
> * 订单管理模块，用户能够对订单进行付款，查询历史订单
> ##### 后台：用户管理，充电宝投放点管理，充电宝管理，订单管理
>	* 用户管理模块，提供用户注册、用户信息维护等公功能
>	* 充电宝投放点管理模块，提供对充电宝投放点的增删改查
>	* 充电宝管理，提供对充电宝的增删改查
> *	订单管理，提供对用户订单的查询

## 实现
* 用前后端分离的方式，后端提供API实现各种功能。鉴权方式没有使用token，仅仅使用了session放user或者admin对象的方式。
* API的设计是希望符合RESTful规范的，实际写的不算好但还算清晰。
#### 前端 
* 前台使用了jquery-weui以及高德的JS插件中地图显示、云图数据显示、云图数据搜索、定位功能。
* 后台使用了阿里飞冰的 IceWorks，管理页面使用的是Vue的各种物料修改的。由于不懂Vue，所以改的一塌糊涂。
#### 后端
* Spring MVC + Spring + Mybatis搭配使用。
* 使用maven进行依赖管理
* JDK8,Tomcat 8.5,MySQL 5.7 数据库SQL在files文件夹里

**如要运行，有两个地方需要自定义**
> * 数据库连接的配置
> * Yuntu.java 高德云图key，tableId

## 建议
* 课程需要完成模拟系统的，可参考。十八流编码水平。
* 需要使用高德地图的定位、云图的定位搜索、云图数据查询的，可以参考。官方云图数据的示例有所欠缺。
* 其他人就不用看了。。。

## 效果图
![前台](https://github.com/KonsonChow/ChargerSharingSystem/blob/master/files/01.JPG)
![后台](https://github.com/KonsonChow/ChargerSharingSystem/blob/master/files/02.JPG)
![数据库](https://github.com/KonsonChow/ChargerSharingSystem/blob/master/files/table.png)
