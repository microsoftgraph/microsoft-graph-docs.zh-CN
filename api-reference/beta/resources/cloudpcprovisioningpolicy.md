---
title: cloudPcProvisioningPolicy 资源类型
description: 表示云电脑预配策略。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b16d4a95bf791b387958605b64e7a370e1c3971f
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014283"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>cloudPcProvisioningPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑预配策略。

## <a name="methods"></a>Methods

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|列出 [cloudPcProvisioningPolicy 对象的属性和](../resources/cloudpcprovisioningpolicy.md) 关系。|
|[获取 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|读取 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。|
|[创建 cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[更新 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|更新 [cloudPcProvisioningPolicy 对象](../resources/cloudpcprovisioningpolicy.md) 的属性。|
|[删除 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|无|删除 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[分配 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|无 |将 [cloudPcProvisioningPolicy 分配给](../resources/cloudpcprovisioningpolicy.md) 用户组。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|说明|String|设置策略说明。|
|displayName|String|设置显示名称策略的项。|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|指定云电脑如何加入Azure Active Directory。|
|id|String|云电脑预配策略的唯一标识符。 只读。|
|imageDisplayName|String|显示名称预配的操作系统映像的映像。|
|imageId|String|你想要在云电脑中预配的操作系统映像的 ID。 库类型图像的格式为：{publisher_offer_sku}。 每个参数支持的值如下所示：<ul><li>发布者：Microsoftwindowsdesktop。</li> <li>offer：windows-ent-cpc。</li> <li>sku：21h1-ent-cpc-m365， 21h1-ent-cpc-os、20h2-ent-cpc-m365、20h2-ent-cpc-os、20h1-ent-cpc-m365、20h1-ent-cpc-os、19h2-ent-cpc-m365 和 19h2-ent-cpc-os。</li></ul>|
|imageType|cloudPcProvisioningPolicyImageType|你想要在云 (预配的操作系统映像) 库类型。 可取值为：`gallery`、`custom`。|
|microsoftManagedDesktop|[microsoftManagedDesktop](../resources/microsoftManagedDesktop.md)|云解决方案的特定Microsoft 托管桌面，使客户能够获取云电脑的托管设备体验。 管理员必须先配置Microsoft 托管桌面，然后才能启用此配置。|
|onPremisesConnectionId|String|cloudPcOnPremisesConnection 的 ID。 若要确保云电脑具有网络连接并且它们已加入域，请选择与通过云电脑服务验证的虚拟网络的连接。|

## <a name="relationships"></a>关系

|关系|类型|Description|
|:---|:---|:---|
|assignments|[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 集合|已定义的设置策略分配集合。 表示已分配Microsoft 365策略的Azure AD组和安全组集。 仅在 `$expand` 上返回。 请参阅 [获取](../api/cloudpcprovisioningpolicy-get.md) 分配关系的示例。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "description": "String",
  "displayName": "String",
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  },
  "id": "String (identifier)",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "onPremisesConnectionId": "String"
}
```
