---
title: policySetItem 资源类型
description: 包含用于 PolicySet 项目的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d30c7711bc8c154a112a02ed929093c63bbbdbe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735167"
---
# <a name="policysetitem-resource-type"></a>policySetItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于 PolicySet 项目的属性的类。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 policySetItems](../api/intune-policyset-policysetitem-list.md)|[policySetItem](../resources/intune-policyset-policysetitem.md) 集合|列出 [policySetItem](../resources/intune-policyset-policysetitem.md) 对象的属性和关系。|
|[获取 policySetItem](../api/intune-policyset-policysetitem-get.md)|[policySetItem](../resources/intune-policyset-policysetitem.md)|读取 [policySetItem](../resources/intune-policyset-policysetitem.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|MobileAppPolicySetItem 的键。|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。|
|payloadId|String|PolicySetItem 的 PayloadId。|
|itemType|String|PolicySetItem 的 policySetType。|
|displayName|String|PolicySetItem 的 DisplayName。|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生）。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|引导部署的标记|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```





