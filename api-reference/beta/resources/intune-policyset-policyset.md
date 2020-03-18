---
title: policySet 资源类型
description: 包含用于 PolicySet 的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d50b59deb24bba2e10e6060a46b41e435b779f4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775203"
---
# <a name="policyset-resource-type"></a>policySet 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于 PolicySet 的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 policySets](../api/intune-policyset-policyset-list.md)|[policySet](../resources/intune-policyset-policyset.md)集合|列出[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。|
|[获取 policySet](../api/intune-policyset-policyset-get.md)|[policySet](../resources/intune-policyset-policyset.md)|读取[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。|
|[创建 policySet](../api/intune-policyset-policyset-create.md)|[policySet](../resources/intune-policyset-policyset.md)|创建新的[policySet](../resources/intune-policyset-policyset.md)对象。|
|[删除 policySet](../api/intune-policyset-policyset-delete.md)|None|删除[policySet](../resources/intune-policyset-policyset.md)。|
|[更新 policySet](../api/intune-policyset-policyset-update.md)|[policySet](../resources/intune-policyset-policyset.md)|更新[policySet](../resources/intune-policyset-policyset.md)对象的属性。|
|[更新操作](../api/intune-policyset-policyset-update.md)|无|尚未记录|
|[getPolicySets 操作](../api/intune-policyset-policyset-getpolicysets.md)|[policySet](../resources/intune-policyset-policyset.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|PolicySet 的键。|
|createdDateTime|DateTimeOffset|PolicySet 的创建时间。|
|lastModifiedDateTime|DateTimeOffset|PolicySet 的上次修改时间。|
|displayName|String|PolicySet 的 DisplayName。|
|说明|String|PolicySet 的说明。|
|状态|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySet 的验证/分配状态。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生）。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|引导部署的标记|
|roleScopeTags|String collection|PolicySet 的 RoleScopeTags|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合|PolicySet 的分配。|
|items|[policySetItem](../resources/intune-policyset-policysetitem.md)集合|PolicySet 的项目，最大计数为100。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "roleScopeTags": [
    "String"
  ]
}
```



