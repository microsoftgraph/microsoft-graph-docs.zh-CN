---
title: policySetItem 资源类型
description: 包含用于 PolicySet 项目的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2701686d9f2f162a6ec01dfb143c2d8652dd098a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422504"
---
# <a name="policysetitem-resource-type"></a>policySetItem 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于 PolicySet 项目的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 policySetItems](../api/intune-policyset-policysetitem-list.md)|[policySetItem](../resources/intune-policyset-policysetitem.md)集合|列出[policySetItem](../resources/intune-policyset-policysetitem.md)对象的属性和关系。|
|[获取 policySetItem](../api/intune-policyset-policysetitem-get.md)|[policySetItem](../resources/intune-policyset-policysetitem.md)|读取[policySetItem](../resources/intune-policyset-policysetitem.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|MobileAppPolicySetItem 的键。|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。|
|payloadId|String|PolicySetItem 的 PayloadId。|
|itemType|String|PolicySetItem 的 policySetType。|
|displayName|String|PolicySetItem 的 DisplayName。|
|状态|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生）。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String 集合|引导部署的标记|

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



