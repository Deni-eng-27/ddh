# DDH上的ECS资源计费 {#concept_qrv_tmn_tdb .concept}

本文介绍在专有宿主机DDH上使用ECS实例时，ECS资源如何计费。

在DDH上运行的ECS实例，无论哪种计费方式，您无需再为实例的vCPU、内存和本地盘付费。但是您需要为ECS实例的付费镜像、云盘、公网带宽、快照等资源付费。计费详情，请参见[包年包月](../../../../cn.zh-CN/产品定价/包年包月.md#)、[公网带宽计费](../../../../cn.zh-CN/产品定价/公网带宽计费.md#)、[快照计费方式](../../../../cn.zh-CN/产品定价/快照计费方式.md#)以及[弹性公网IP计费概述](../../../../cn.zh-CN/产品定价/计费概述.md#)。

当包年包月DDH未过期时，处于不同运行状态的ECS实例关联的资源计费情况不同。

## 运行中的实例 {#section_drm_rcw_tdb .section}

无论哪种计费方式，处于**运行中**的实例，所有ECS关联资源都正常计费。

## 已停止的实例 {#section_erm_rcw_tdb .section}

实例停止后，ECS实例的计费方式不同，收费的ECS关联资源不同。

-   包年包月实例

    包年包月ECS实例停止后，所有ECS关联资源都正常计费。

-   按量付费实例

    与共享宿主机上运行的按量付费ECS实例不同，DDH上运行的按量付费ECS实例不完全适用[按量付费实例停机不收费](../../../../cn.zh-CN/产品定价/按量付费实例停机不收费.md#)功能。实例停止后，ECS关联资源收费变化如下：

    -   镜像：保留。如果为付费镜像，则继续计费。
    -   公网带宽：
        -   如果实例分配了公网IP地址，IP地址将被释放，公网带宽不再计费。
        -   如果实例绑定了EIP地址，而且停止前未解绑，则EIP地址保持不变，继续计费。

            **说明：** 实例停止后，私有IP地址保持不变。

    -   云盘：保留。继续计费。

