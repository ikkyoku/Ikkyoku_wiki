# 在Tableau中使用Python

>1. [安装TabPy](#安装TabPy "安装TabPy")
1. [启动TabPy](#启动TabPy "启动TabPy")
1. [Tableau连接TabPy](#Tableau连接TabPy "Tableau连接TabPy")
1. [Tableau调用TabPy服务](#Tableau调用TabPy服务 "Tableau调用TabPy服务")
1. [Pytab自定义函数部署](#Pytab自定义函数部署 "Pytab自定义函数部署")
1. [TabPy服务搭建及函数部署汇总](#TabPy服务搭建及函数部署汇总 "TabPy服务搭建及函数部署汇总")
1. [参考](#参考 "参考")


## 安装TabPy
首先安装并升级pip
```
python -m pip install --upgrade pip
```

使用pip安装TabPy
```
pip install tabpy
```
## 启动TabPy

在默认设定下启动TabPy
```
tabpy
```
会显示初始化TabPy Server
```
Call context logging is disabled
Initializing TabPy...
Initializing TabPy Server...
Done initializing TabPy.
Setting max request size to 104857600 bytes
Initializing models...
Web service listening on port 9004
```

## Tableau连接TabPy

打开Help->Settings and Performance->Manage Analytics Extension Connections...

![菜单路径](assets/003/20220323-a47daecd.png=-300)  

选择TabPy

![选择界面](assets/003/20220323-4e76b93f.png=-300)  

由于我们搭建的TabPy服务是建立在本地计算机上，因此服务器填写为“http://localhost”
端口为“9004”（这是默认的端口），如下所示。【全程需要保持tabpy服务一直开启，不要关闭】

![参数界面](assets/003/20220323-1386a1c5.png=-300)  

点击Test Connection 测试是否可以连接TabPy服务，如果出现成功提示即可点击Save

![成功提示](assets/003/20220323-f536d44d.png=-300)  

## Tableau调用TabPy服务

Tableau主要通过在创建计算字段中使用TabPy服务中的函数，即由input通过python函数计算得到output。代码样式如下：
```
SCRIPT_REAL("return tabpy.query('add',_arg1,_arg2)['response']",sum(1),sum(2))
# 注意，这里一定要有return值
# 其中 _arg1和_arg2指要输入的参数
```
上述代码在Python也可直接运行，我觉得可以用来验证函数是否定义正确
```
r = client.query('add',[1,2,3,4],[12,3,4,5])['response']
print(r)
```
除了SCRIPT_REAL外，还有SCRIPT_BOOL，SCRIPT_INT，SCRIPT_STR等函数，对应输出不同的数据类型~

## Pytab自定义函数部署
- 待补充

## TabPy服务搭建及函数部署汇总
- 待补充

## 参考

- TabPy-Github：https://github.com/tableau/TabPy
- 在Tableau中使用Python（TabPy的使用）：https://zhuanlan.zhihu.com/p/65402912
- Tableau 高级 | TabPy使用：https://blog.csdn.net/ganzheyu/article/details/80344732
- TablePy Application：https://www.youtube.com/watch?v=nRtOMTnBz_Y
