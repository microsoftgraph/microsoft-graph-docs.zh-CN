---
title: cloudPcProvisioningPolicy 资源类型
description: 表示云电脑预配策略。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 58fa7ff74086d39d124f3d4701f5951636fd8eda
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563756"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>cloudPcProvisioningPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑预配策略。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|列出 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。|
|[获取 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|读取 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。|
|[创建 cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[更新 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|更新 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性。|
|[删除 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|无|删除 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[分配 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|无 |将 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 分配给用户组。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑预配策略的唯一标识符。 只读。|
|displayName|String|设置策略的显示名称。|
|说明|String|设置策略说明。|
|onPremisesConnectionId|String|CloudPcOnPremisesConnection 的 ID。 若要确保云电脑具有网络连接且它们加入域，请选择与云电脑服务验证的虚拟网络的连接。|
|imageId|String|要在云电脑上预配的 OS 映像的 ID。 库类型图像的格式为： {publisher_offer_sku}。|
|imageDisplayName|String|您正在设置的 OS 映像的显示名称。|
|imageType|cloudPcProvisioningPolicyImageType|要在云电脑上预配的 OS 映像 (自定义或库) 的类型。 可取值为：`gallery`、`custom`。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|assignments|[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 集合|已定义的设置策略分配的集合。 仅在 `$expand` 上返回。 请参阅获取工作分配关系的 [示例](../api/cloudpcprovisioningpolicy-get.md) 。 |

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
