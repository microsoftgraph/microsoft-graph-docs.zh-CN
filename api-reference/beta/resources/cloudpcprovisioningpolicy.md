---
title: cloudPcProvisioningPolicy 资源类型
description: 表示云电脑预配策略。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3fd07bc2df93e57d6135a3bf7956f931db13c801
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763050"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>cloudPcProvisioningPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑预配策略。

## <a name="methods"></a>方法

|方法|返回类型|说明|
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
|id|String|云电脑预配策略的唯一标识符。 只读。|
|displayName|String|设置显示名称策略的项。|
|说明|String|设置策略说明。|
|onPremisesConnectionId|String|cloudPcOnPremisesConnection 的 ID。 若要确保云电脑具有网络连接并且它们已加入域，请选择与通过云电脑服务验证的虚拟网络的连接。|
|imageId|String|你想要在云电脑中预配的操作系统映像的 ID。 库类型图像的格式为：{publisher_offer_sku}。 每个参数支持的值如下所示：<ul><li>发布者：Microsoftwindowsdesktop。</li> <li>offer：windows-ent-cpc。</li> <li>sku：21h1-ent-cpc-m365， 21h1-ent-cpc-os、20h2-ent-cpc-m365、20h2-ent-cpc-os、20h1-ent-cpc-m365、20h1-ent-cpc-os、19h2-ent-cpc-m365 和 19h2-ent-cpc-os。</li></ul>|
|imageDisplayName|String|适用于显示名称的操作系统映像的映像。|
|imageType|cloudPcProvisioningPolicyImageType|你想要在云 (预配的操作系统映像) 库类型。 可取值为：`gallery`、`custom`。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|assignments|[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 集合|已定义的设置策略分配集合。 表示已分配Microsoft 365 Azure AD 中的安全组和安全组集。 仅在 `$expand` 上返回。 请参阅 [获取](../api/cloudpcprovisioningpolicy-get.md) 分配关系的示例。 |

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
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "onPremisesConnectionId": "String",
  "imageId": "String",
  "imageDisplayName": "String",
  "imageType": "String"
}
```
