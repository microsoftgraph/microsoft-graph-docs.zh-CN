---
title: privilegedRoleSummary 资源类型
description: 特定角色的统计信息摘要。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 1390804ca0d88eaee823e20ecb226c31609822e1
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454106"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定角色的统计信息摘要。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |读取 privilegedRoleSummary 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|elevatedCount|int32|分配了角色并激活角色的用户数。|
|id|string| 角色的唯一标识符。 只读。|
|managedCount|int32|分配了角色但角色已停用的用户数。|
|mfaEnabled|boolean|`true` 如果角色激活需要 MFA。 `false` 如果角色激活不需要 MFA。|
|状态|roleSummaryStatus| 可取值为：`ok`、`bad`。 值取决于 managedCount / usersCount (的) 。 如果比率小于预定义阈值，则 `ok` 返回 。 否则 `bad` ，将返回 。|
|usersCount|int32|分配了角色的用户数。|

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


