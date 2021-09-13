---
title: policySet 资源类型
description: 一个包含用于 PolicySet 的属性的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3216acbfaf03e0edc61eb87cbe8419c22227f9b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074883"
---
# <a name="policyset-resource-type"></a>policySet 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个包含用于 PolicySet 的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 policySets](../api/intune-policyset-policyset-list.md)|[policySet](../resources/intune-policyset-policyset.md) 集合|列出 policySet 对象 [的属性和](../resources/intune-policyset-policyset.md) 关系。|
|[获取 policySet](../api/intune-policyset-policyset-get.md)|[policySet](../resources/intune-policyset-policyset.md)|读取 policySet 对象 [的属性和](../resources/intune-policyset-policyset.md) 关系。|
|[创建 policySet](../api/intune-policyset-policyset-create.md)|[policySet](../resources/intune-policyset-policyset.md)|创建新的 [policySet](../resources/intune-policyset-policyset.md) 对象。|
|[删除 policySet](../api/intune-policyset-policyset-delete.md)|无|删除 [policySet](../resources/intune-policyset-policyset.md)。|
|[更新 policySet](../api/intune-policyset-policyset-update.md)|[policySet](../resources/intune-policyset-policyset.md)|更新 [policySet 对象](../resources/intune-policyset-policyset.md) 的属性。|
|[更新操作](../api/intune-policyset-policyset-update.md)|无|尚未记录|
|[getPolicySets 操作](../api/intune-policyset-policyset-getpolicysets.md)|[policySet](../resources/intune-policyset-policyset.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySet 的键。|
|createdDateTime|DateTimeOffset|PolicySet 的创建时间。|
|lastModifiedDateTime|DateTimeOffset|PolicySet 的上次修改时间。|
|displayName|String|PolicySet 的 DisplayName。|
|说明|String|PolicySet 的说明。|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySet 的验证/分配状态。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生了任何错误）。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|引导式部署的标记|
|roleScopeTags|String collection|PolicySet 的 RoleScopeTags|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|assignments|[policySetAssignment](../resources/intune-policyset-policysetassignment.md) 集合|PolicySet 的分配。|
|items|[policySetItem](../resources/intune-policyset-policysetitem.md) 集合|最大计数为 100 的 PolicySet 项目。|

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



