---
title: privilegedRoleSummary 资源类型
description: 特定角色的统计信息摘要。
localization_priority: Normal
ms.openlocfilehash: 3e7b447f63c5f8545021508ae2dc137bef845210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344260"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定角色的统计信息摘要。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |读取 privilegedRoleSummary 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|elevatedCount|时会|已分配角色并激活角色的用户数量。|
|id|string| 角色的唯一标识符。 只读。|
|managedCount|时会|已分配角色但角色被停用的用户数量。|
|mfaEnabled|boolean|**如此**如果角色激活需要进行 MFA。 **假**如果角色激活不需要进行 MFA。|
|状态|string| 可取值为：`ok`、`bad`。 值取决于 (managedCount/usersCount) 的比率。 如果该比率小于预定义的阈值, `ok`则返回。 否则, `bad`将返回。|
|usersCount|时会|为角色分配的用户数。|

## <a name="relationships"></a>关系
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
