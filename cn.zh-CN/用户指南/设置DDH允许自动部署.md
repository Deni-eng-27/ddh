# 设置DDH允许自动部署 {#task_1096342 .task}

创建DDH后，您可以将DDH设置为允许自动部署，由系统自动在DDH上部署ECS实例。本文介绍设置DDH允许自动部署的操作步骤。

已创建DDH。具体步骤，请参见[创建DDH](../cn.zh-CN/快速入门/创建包年包月DDH.md#)。

DDH设置为允许自动部署后，您创建ECS实例时，可以不指定DDH，由系统从允许自动部署的DDH中自动选择DDH部署实例。自动部署功能详情，请参见[自动部署功能介绍](../cn.zh-CN/产品简介/功能介绍.md#)。

1.  登录[ECS管理控制台](https://ecs.console.aliyun.com)。
2.  在左侧导航栏，单击**实例与镜像** \> **专有宿主机 DDH**。
3.  在顶部状态栏处，选择地域。
4.  选中目标DDH。
5.  单击**操作** \> **修改主机信息**。
6.  在修改宿主机信息对话框，打开**允许自动部署**开关。
7.  单击**确定**。

目标DDH的**允许自动部署**列，更新为**打开**。

您可以选择自动部署功能创建ECS实例，由系统自动选择DDH部署ECS实例。具体步骤，请参见[使用向导创建实例](../../cn.zh-CN/实例/创建实例/使用向导创建实例.md#)。

