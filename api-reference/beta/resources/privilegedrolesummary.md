---
title: privilegedRoleSummary 资源类型
description: 为特定的角色摘要统计信息。
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047984"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

为特定的角色摘要统计信息。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |读取属性和 privilegedRoleSummary 对象的关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|elevatedCount|int32|激活已分配的角色和角色的用户数。|
|id|string| 角色的唯一标识符。 只读。|
|managedCount|int32|停用已分配的角色的用户，但该角色的数量。|
|mfaEnabled|boolean|如果为**true**的角色激活需要 MFA。 **false**如果角色激活不需要 MFA。|
|status|string| 可取值为：`ok`、`bad`。 值取决于的比率 (managedCount / usersCount)。 如果此比率小于预定义的阈值，`ok`返回。 否则为`bad`返回。|
|usersCount|int32|与角色分配的用户数。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->