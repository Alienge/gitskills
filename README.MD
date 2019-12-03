# 职工系统demo
###环境
- vs2017
- win10
- wpf
- sql server2017
- c#
###数据库的格式
一个数据库：UserInfoManage
包含两张表
职工信息表（UserInfo）：注册后，不可修改，可以删除

|   名称  | 类型  |含义|
|  ----  | ----  |-----|
| id   | int |职工号
| nm   | varchar(10) |姓名
| gender   | char(8) |性别
| specialty   | char(30) |专业
| brith   | smalldatetime |出生日期
| mail   | varchar(50) |邮箱
| phone   | varchar（13） |电话

职工职位表（PosiInfo）：只要职工注册，自动生成，存在默认值，可修改，可查看，可以删除

|   名称  | 类型  |含义|
|  ----  | ----  |-----|
| id   | int |职工号
| nm   | varchar(10) |姓名
| position   | char(30) |职位
| Salary   | decimal(18,0) |薪水

###文件类型
文件包含两个部分，一个是在线更新的程序updatePro1.exe,另外一个是职工查询表WpfApp1.exe

###用法
下载对应的zip文件，解压到本地，本地服务器有sql server2016，并且已经创建了数据库和相应的表, 点击WpfApp1.exe运行即可
