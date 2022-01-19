---
title: virtualEndpoint 资源类型
description: virtualEndpoint 资源表示云电脑管理功能的容器。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c616d3894b5c9efaf356e28879edc067d7d3ffcd
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072255"
---
# <a name="virtualendpoint-resource-type"></a>virtualEndpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于管理云电脑的 API 的容器。

使用云电脑 API 为组织的员工预配和管理虚拟桌面。 将它与 [Intune API](../resources/intune-graph-overview.md) 结合使用，以管理物理和虚拟终结点。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[获取有效权限](../api/virtualendpoint-geteffectivepermissions.md)|字符串集合|查看当前经过身份验证的用户的有效权限。|
|[列出 cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。|
|[列出 deviceImages](../api/virtualendpoint-list-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。|
|[List galleryImages](../api/virtualendpoint-list-galleryimages.md)|[cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) 集合|列出 [cloudPcGalleryImage 对象的属性和](../resources/cloudpcgalleryimage.md) 关系。|
|[创建 cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[列出 onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[创建 cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。|
|[列出 provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|列出 [cloudPcProvisioningPolicy 对象的属性和](../resources/cloudpcprovisioningpolicy.md) 关系。|
|[创建 cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[列出 userSettings](../api/virtualendpoint-list-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合|从 userSettings 导航属性获取 cloudPcUserSetting 资源。|
|[创建 cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|创建新的 cloudPcUserSetting 对象。|
|[列出 auditEvents](../api/virtualendpoint-list-auditevents.md)|[cloudPcAuditEvent](../resources/cloudpcauditevent.md) 集合|列出 [cloudPcAuditEvent 对象的属性和](../resources/cloudpcauditevent.md) 关系。|
|[列出 supportedRegions](../api/virtualendpoint-list-supportedregions.md)|[cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) 集合|列出 [cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) 对象的属性和关系。|
|[List servicePlans](../api/virtualendpoint-list-serviceplans.md)|[cloudPcServicePlan](../resources/cloudpcserviceplan.md) 集合|列出 [cloudPcServicePlan 对象的属性和](../resources/cloudpcserviceplan.md) 关系。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|虚拟终结点 ID 的唯一标识符。只读。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|cloudPCs|[cloudPC](../resources/cloudpc.md) 集合|云托管虚拟桌面。|
|deviceImages|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|云电脑上的图像资源。|
|galleryImages|[cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) 集合|云电脑上的库图像资源。|
|onPremisesConnections|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|一个定义的 Azure 资源信息集合，可用于为云电脑建立本地网络连接。|
|provisioningPolicies|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|云电脑预配策略。|
|userSettings|[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合|云电脑用户设置。 |
|auditEvents|[cloudPcAuditEvent](../resources/cloudpcauditevent.md) 集合|云电脑审核事件。|
|supportedRegions|[cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) 集合|云电脑支持的区域。|
|servicePlans|[cloudPcServicePlan](../resources/cloudpcserviceplan.md) 集合|云电脑服务计划。|
|organizationSettings|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) |租户的云电脑组织设置。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
